---
title: Android技术周刊第25期
date: 2016-07-22
tags: Android 周刊
author: Conquer
---
本周持续高温，既然不敢出门，还是在家写写代码看看书、抓抓小精灵。本期推荐：

* `Djinni`

> A tool for generating cross-language type declarations and interface bindings.

<!-- more -->

### AwesomeSource

- 这次文章终于没有被外星人劫持了
- 再次墙裂推荐：我司的[AspectjX](https://github.com/HujiangTechnology/gradle_plugin_android_aspectjx) 还有很多外国开发哥们在用它
- [贝塞尔曲线开发的艺术](http://blog.csdn.net/eclipsexys/article/details/51956908)
- [PathMeasure之迷径追踪](http://blog.csdn.net/eclipsexys/article/details/51992473)

### BestArticle

- [Tinker_imitator 原理篇](http://www.jianshu.com/p/620c2b0490ec?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)，之前微信分享过他们的热补丁实现原理，现在MarkZhai模仿原理实现了它，一起来看看吧
- [面向切面编程之疯狂的 Aspects](https://mp.weixin.qq.com/s?__biz=MzAxMzE2Mjc2Ng==&mid=2652154714&idx=1&sn=da44e8ec13bf4ef445e3270e4e80a3e3&scene=1&srcid=0722gcvmYvIDt066zQ8rxBcJ&key=77421cf58af4a6531f89446f4132dd04df83818b1710a84ade064c5b772e230ac57d196cfb51bc12605e95879e68df3f&ascene=0&uin=MjkxNzIxMDMwMA%3D%3D&devicetype=iMac+MacBookPro9%2C2+OSX+OSX+10.11.1+build(15B42)&version=11020201&pass_ticket=Fa25HkL%2BST0gekuLxX2fMfXSzPXn4cW0kNlo3PX5JFh%2BOkozdvr4zt78jnGNa%2BlC)，`AOP`还是很有用的，我们已经有了自己的`Aspect`方案：`AspectJ`.
- [代码审查要点](http://www.techug.com/code-review-3),我们也一直在用`gerrit`做`code review`, 可以一起来看看这篇文章，我们有哪些可以学习的点。
- [程序员需要把好椅子](http://kb.imakewebsites.ca/2014/04/27/chairs-for-programmers/)，为了健康，大家还是关注下吧……


### FantasticLibs

- 微信热更新方案实践
：[Tinker_imitator
](https://github.com/zzz40500/Tinker_imitator)，热修复，需要重启，只是代码级别的热修复. 不支持资源的替换.修改代码的时候不能新增资源id.如果改变了两个dex里面的东西的话,那么占得内存就有点大了。

- [`Djinni`](https://github.com/dropbox/djinni)，本周`YYDroid`为我们带来了关于`Djinni`的分享，在`JNI`开发中很有用的一个库。
- [Using JNI in Swift to put an app into the Android Play Store](https://medium.com/@ephemer/using-jni-in-swift-to-put-an-app-into-the-android-play-store-732e542a99dd#.sm877gsnx)，这个大家可以尝试尝试。
- [Android NDK in Android Studio with SWIG](http://www.sureshjoshi.com/mobile/android-ndk-in-android-studio-with-swig/) `SWIG`是个帮助使用`C`或者`C++`编写的软件能与其它各种高级编程语言进行嵌入联接的开发工具。

### HotNews

- [美图M6 手机众测](http://test.smzdm.com/pingce/p/32192/)，不想吐槽，实在是太厚了。
- [全球首款iOS+安卓双系统硬件机甲在北京震撼上市](http://toutiao.com/i6309750657515520514/?tt_from=weixin&utm_campaign=client_share&from=groupmessage&app=news_article&utm_source=weixin&isappinstalled=0&iid=4912916087&utm_medium=toutiao_ios&wxshare_count=1),苹果皮的新进化。还真有公司一直做这个……
- [按键精灵手机版](http://coolapk.com/apk/com.cyjh.mobileanjian)，可以开发手机脚本工具，模拟手动实现屏幕点击、滑动、图色识别等操作，让您放飞双手，轻松游戏。大家可以考虑下是不是可以直接用来录制脚本自动化测试程序呢。
