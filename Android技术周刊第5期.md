---
title: Android技术周刊第5期
date: 2016-02-29 06:00:00
tags: Android 周刊
---
Linux问他的父亲：你曾经是不是说了一句很牛的话——"talk is cheap,show me the code"? 可是，网络上有那么多好文章，难道都是cheap？

### KnowledgePool

* [R语言（02）绘图](http://dannylee1991.github.io/2016/03/06/R%E8%AF%AD%E8%A8%80%EF%BC%8802%EF%BC%89%E7%BB%98%E5%9B%BE/) 以数据为例，来展示R是如何绘制一些图表的。

### BestArticle
* [Facebook如何采集其Android应用性能数据](https://mp.weixin.qq.com/s?__biz=MzA3ODg4MDk0Ng==&mid=401955288&idx=1&sn=cd6e26f8ccecdde318f873b681e33526&scene=1&srcid=0221Ph4me1lUtzTlCrWZr9Qd&key=710a5d99946419d96f6bad88b3d9b42148af956828a1ab147360005f1d8ce222141b3075441ad6914e4e03aae1c61e08&ascene=0&uin=MjI1NTE5NDA2Mw%3D%3D&devicetype=iMac+MacBookPro11%2C2+OSX+OSX+10.10.5+build\(14F1021\)&version=11020201&pass_ticket=QVvjp5rfSGeK1B2IUW9ztD%2FG3DNqK1OP1Mf132T8IbEt5mmj8dgTKQegO6igLQl%2B) 数据采集一般都离不开埋点插桩，本文介绍了Facebook的插桩方法，他们在考察了Android内建的Debug以及另一些方法后，选择了字节码重写技术，避免了手工插桩的劳动，且性能损失降到最低。

* [在Android中使用反射到底有多慢？](http://blog.nimbledroid.com/2016/02/23/slow-Android-reflection-zh.html?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io) 反射（Reflection）在Java和安卓开发过程中非常有用，但是反射的使用往往是APP严重性能问题的根本原因。本文通过分析几个真实的案例来帮助我们更直观的理解这个问题。

* [那些开发者需要了解的设计基本原则](https://m.flipboard.cn/share?url=http%3A%2F%2Fwww.woshipm.com%2Fpd%2F288577.html&social=wechat&deviceType=iphone&udid=1a7e888b83c9d71f07661d96cbcefc6d4cee48ae&userid=9485132&item_id=flipboard-zqeL0MIJQdyQ4ZDB8TeZUQ%3Aa%3A184483403-1456458776&section_id=flipboard%2Fcurator%252Fmagazine%252FcqZO7hBRSyar44MVxPeEGw%253Am%253A184483403&from=groupmessage&isappinstalled=1) 
干净的 UI 和干净的代码一样。 它是组织好的、一致的而且进无止境。一个设计师的好言劝告，墙裂推荐认真阅读
* [Android Support Library 23.2](http://android-developers.blogspot.jp/2016/02/android-support-library-232.html) Design Lib又更新了，这次更新的不少，鼓掌~~~

* [Android 开发的那些坑和小技巧](https://mp.weixin.qq.com/s?__biz=MzI3MTEzMDI2MA==&mid=405597000&idx=1&sn=5c86631ff95644fdbefa36c4f57ee71d&scene=1&srcid=03010lwFKKs4GuGWyDPZxAvL&key=710a5d99946419d91ed1eea3be59088184f016b794b9c83c7f70d1f63ff0f375ea90497700ca962c987af51fa4cb68e6&ascene=0&uin=MjI1NTE5NDA2Mw%3D%3D&devicetype=iMac+MacBookPro11%2C2+OSX+OSX+10.10.5+build\(14F1021\)&version=11020201&pass_ticket=3OhJ6Q6jZNaO%2BrWN1brtamVLFosGdEWQnoDQYiw2Kj09Xd0QE1EDLJX2aj4vyhJq)  知道一些坑，了解一些小技巧，会让你的开发事半功倍

* [Android APK终极瘦身21招](https://mp.weixin.qq.com/s?__biz=MzA3ODg4MDk0Ng==&mid=402380504&idx=1&sn=7013f0842867a21555adcf445c7c03ee&scene=1&srcid=0302DAWQ0vmV7ZGLuIEspz3a&key=710a5d99946419d953f7ab50fbe10d553fe0056e641560956a071c0399784f002970d8240a67c3044ffd60e747b17498&ascene=0&uin=MjI1NTE5NDA2Mw%3D%3D&devicetype=iMac+MacBookPro11%2C2+OSX+OSX+10.10.5+build\(14F1021\)&version=11020201&pass_ticket=3OhJ6Q6jZNaO%2BrWN1brtamVLFosGdEWQnoDQYiw2Kj09Xd0QE1EDLJX2aj4vyhJq) Android安装包瘦身指南


### DevTools
* [Jenkins 2.0 要来了](http://www.cnblogs.com/wzy5223/p/5249135.html#rd?sukey=a76cdd086edb4fce9caa869883652f46cb9f65f1b7d189c32ea134656985a193edfde760d0453ffb5f7310b0036ca2ca) Jenkins 在2016/02/29日发布了2.0 alpha版本

### FantasticLibs

* [开源 Mac 微信客户端](https://github.com/geeeeeeeeek/electronic-wechat)  纯js手工打磨:A better WeChat client on Mac OS X and Linux.(同一作者下，WeChatLuckyMoney微信抢红包插件)

