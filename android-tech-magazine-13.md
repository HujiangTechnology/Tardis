---
title: Android技术周刊第13期
date: 2016-04-25 06:00:00
tags: Android 周刊
author: YYDroid
---
曾经我们喜欢乔丹，是因为篮球；今天我们再一次爱上了乔丹，因为突然意识到``Just DO IT``这句话还有另外一层含义：just do information technology！可能也正是因为这句话，才让广大有志青年踏入IT行业，太伟大了，乔丹！科比退役了，不知道为什么，一看到科比就想起了乔丹！

<!-- more -->

### BestArticle
- 	[Optimizing Android bytecode with ReDex](https://code.facebook.com/posts/998080480282805/open-sourcing-redex-making-android-apps-smaller-and-faster/) This blog provides an overview of the Redex project.
-  [Kotlin Post-1.0 Roadmap](http://blog.jetbrains.com/kotlin/2016/04/kotlin-post-1-0-roadmap/) Kotlin的特性是在向F#在靠拢吗？
-  [2015中国移动应用性能管理白皮书](https://mp.weixin.qq.com/s?__biz=MzA3MzYwNjQ3NA==&mid=2651296451&idx=2&sn=479b8700ec8f2e6c930bcf797aab7edc&scene=1&srcid=0423tOLBtOpPPVC5uaXdIOVv&key=b28b03434249256b889b77f74a66a54cc3e53187c3bb6de83a022079bb93f9049854600266ced1815bd0d61bc4e2982f&ascene=0&uin=MjM2NDM0ODgyMA%3D%3D) 2015 年，可以说是移动应用生态系统发展史上的一座里程碑。从技术上看，不断增加的屏幕分辨率，64位处理器，到支持所有平台开发的HTML5技术逐步成熟，硬件性能的提升，新技术的出现都是影响移动应用发展的重要因素，每个方面都不容小觑。从类型上看，在线视频、在线音乐和交友类应用的订阅盈利模式大获成功；游戏、拼车和移动商务应用的下载量和使用量也都持续增长
-  [Android 全局异常捕获之CrashHandler](https://mp.weixin.qq.com/s?__biz=MzA4NDM2MjAwNw==&mid=2650575743&idx=1&sn=1b027970e82863c9fe1b13dbe7ecea2b&scene=1&srcid=0424mVlVTCIJ1mZ5Pg0C9F1K&key=b28b03434249256b9ed220df37b117d5c82a5679c1e7e5050f167152d449cf494f865ed171a3a2488a5f62a2ddc18bdc&ascene=0&uin=MjM2NDM0ODgyMA%3D%3) 使用Java的Thread的UncaughtExceptionHandler接口来捕获全局异常，这个方法，你应该用过吧！！
 
### DevTools
- [ReDex](https://github.com/facebook/redex) ReDex is an Android bytecode (dex) optimizer originally developed at Facebook. It provides a framework for reading, writing, and analyzing .dex files, and a set of optimization passes that use this framework to improve the bytecode. An APK optimized by ReDex should be smaller and faster than its source.

### FantasticLibs
- [TurboDex](https://github.com/asLody/TurboDex) It is generally known that load an unoptimized Dex file at runtime in Android (especially in ART mode) would take a long time. When your App is using MultiDex or PluginFramework, You will find that this problem is hard to bear.
TurboDex was born to solve this problem, Like to opens the god mode for AndroidVM, after using TurboDex, no matter how much Dex file your need to load, it will be finished in a very short time.

### HotNews
- [音乐版的阿里巴巴——阿里星球](http://www.huxiu.com/article/143256/1.html) 阿里剧透音乐平台“阿里星球”，这就是一个音乐版的阿里巴巴！
- [如何看待“天天动听”改名“阿里星球"](https://www.zhihu.com/question/41664635)
- [Android N 终于肯为 VR 做优化](http://www.geekpark.net/topics/215241) 即将到来的 Android 7.0，代号为 Android N。在其预览版里，我们发现了些许端倪——内置应用中多了「VR Helper」和「VR Listener」，权限管理中还多出「是否允许应用运行 VR 模式」的选项。
- [Osmo](http://36kr.com/p/212261.html) 让孩子动手操作，连接iPad游戏与现实世界的Osmo可能成为下一个杀手级APP

