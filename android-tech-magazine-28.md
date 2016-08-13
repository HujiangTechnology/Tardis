---
title: Android技术周刊第28期
date: 2016-08-14
tags: Android 周刊
author: YYDroid
---
有的时候，周刊只要一篇就够了！

<!-- more -->

获取JNI库里的版本号
================


## 为毛会有这么个奇葩的话题

其实起因很简单，因为我们有一个项目是在 JNI 库里面写了版本号的，而且该版本号将会影响编译过程。

具体说来，就是 JNI 库太大，为了在编译项目时节省时间，只有当版本号发生变化时才进行 JNI 的编译，否则就只编译 APK 了。

听起来挺靠谱的，但是到了真正写编译脚本的时候，就懵逼了，这个版本号写进去容易，但是怎么读出来呢... 最终的目的是要比对版本号嘛...

## 分析

再次重新审视现状，版本号是作为全局静态变量被写在```.cpp```文件内，而事后该```.cpp```被编译进```.so```文件，变得不可读。

而我们的判断是要判断```.cpp```内的版本号，和```.so```内的版本号，若是不一致才进行编译，这个问题就变为了如何从一个 JNI 库内读取一个指定的静态变量的值。

到了这里其实答案已经出来了，我们必须借助```objdump```，用它来对```.so```进行逆向，获取内部的数据。由此写下一个命令：

```
$ objdump -DS libsample.so
```

恩，直接悲剧了，程序报错，提示格式不对。你要问为毛，原因是这个 JNI 库是 ARM 指令集的，所以就必须找到跨平台工具，即作用于 ARM 的 ```objdump```命令。

幸运的是，我们并不需要走太远，NDK 内已经提供了这一工具，就拿 Mac 版的 NDK 来说，这一工具位于：

```
${NDK_HOME}/toolchains/arm-linux-androideabi-4.9/prebuilt/darwin-x86_64/bin/arm-linux-androideabi-objdump
```

只需要使用这一工具即可，于是有了以下脚本代码：

```
$ export BINUTIL_HOME=${NDK_HOME}/toolchains/arm-linux-androideabi-4.9/prebuilt/darwin-x86_64/bin
$ ${BINUTIL_HOME}/arm-linux-androideabi-objdump -DS libsample.so
```

命令的执行需要比较长的时间，取决于这个 JNI 库有多复杂。完成后会打印出一大堆东西，当然大部分内容我们不需要关心。

直接找到```Disassembly of section .data```这个部分，你会发现几乎所有的全局变量都在此处列出（说『几乎』是因为还有部分全局变量会放在```section .rodata```，决定这个的是变量的类型）。

好了，往下稍微翻一下，就能找到我们定义的版本号了，此处是：

```
00015004 <jniVersionCode>:
```

此处的```000000f1 ```转换成 10 进制就是我们要的版本号了，至此分析完毕。

## 解决问题

既然已经通过分析得到了想要的结果，那么解决问题就变得无比简单了，请出 CodeTyphon 写一段小程序搞定之，废话不多直接上代码：

```
program sover;
```

随便编译一下就成了，接着就可以欢乐的玩耍啦，命令很简单：

```
$ export BINUTIL_HOME=${NDK_HOME}/toolchains/arm-linux-androideabi-4.9/prebuilt/darwin-x86_64/bin
$ ./sover libsample.so
```

执行命令后打印出 241，这就是 JNI 库的版本号。

设置 ```BINUTIL_HOME``` 这个环境变量是为了跨平台，每个平台下可能配置的命令路径都不一样，**不能写死**！

* 如果觉得每次都 export 很麻烦，可以直接将 ```BINUTIL_HOME``` 写进 .bash_profile 内，以后就无需再输入了。

* 如果你使用 Ubuntu 或是它的衍生版本，可以直接 apt 安装 ```binutils-arm-linux-gnueabihf```，这样无需安装 NDK，也可以执行这个命令了。