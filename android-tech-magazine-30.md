---
title: Android技术周刊第30期
date: 2016-08-28
tags: Android 周刊
author: liuwenhui
---
####本周重点是 Android 7.0正式版本发布。 [Google Releases Android 7.0 with Over 250 New Features](https://www.infoq.com/news/2016/08/android-7-nougat)﻿

<!-- more -->

### BestArticle

- [Managing Your App's Memory﻿ RAM](http://blog.csdn.net/qq_27258799/article/details/51072588) 在任何软件开发环境中都弥足珍贵，而在内存吃紧的移动操作系统中，它就显得更加宝贵。尽管安卓虚拟机控制着日常垃圾收集工作，但我们不能忽视自己的app何时何地分配和销毁内存。
- [你还在写麻烦的 Adapter 么？](https://zhuanlan.zhihu.com/p/22146783) 推荐一个类库 itemPool ，它能很大程度上减少你的 Adapter 数量，它是一个解耦实现，能把 ViewHolder/ItemView 解耦出来。请记住，这让所有 ItemView 变得可复用。
- [使用DiffUtil高效更新RecyclerView﻿](http://blog.chengdazhi.com/index.php/231) DiffUtil是recyclerview support library v7 24.2.0版本中新增的类，根据Google官方文档的介绍，DiffUtil的作用是比较两个数据列表并能计算出一系列将旧数据表转换成新数据表的操作。这个概念比较抽象，换一种方式理解，DiffUtil是一个工具类，当你的RecyclerView需要更新数据时，将新旧数据集传给它，它就能快速告知adapter有哪些数据需要更新。
- [26款优秀的Android逆向工程工具](http://mp.weixin.qq.com/s?__biz=MzAwNDY1ODY2OQ==&mid=2649286341&idx=1&sn=054d595af6e824cbe4edd79427fc2706&scene=1&srcid=0804GUswANrDEWYVWRryYJbE#rd) 工欲善其事必先利其器，好的Android逆向工程工具在逆向破解工程中起到事半功倍的作用。

﻿
### FantasticLibs
- [ItemPool](https://github.com/nekocode/ItemPool) It can help you reduce a lot of code but it lose the flexibility of the recyclerview's adapter. In some cases you still need to create an adapter.


### HotNews
- [爆料：第一个通过Twitter来控制的Android僵尸网络﻿](http://www.cnbeta.com/articles/526883.htm) 近日，来自 ESET 公司（一家世界知名的电脑软件安全公司）的安全研究人员发现，一名专门制作 Android 恶意软件的黑客正通过使用 Twitter 社交网络来控制一些 Twitter 用户的 Android 智能手机。毫无疑问，这些 Android 智能手机都遭到了恶意软件的感染。
- [Google Releases Android 7.0 with Over 250 New Features](https://www.infoq.com/news/2016/08/android-7-nougat) Google has started updating certain devices to the latest Android 7.0 dubbed Nougat. Usually, a new version of Android would start to be pushed to devices during the fall, in late September or even October. But this year, they changed the pace, making available a preview in March and the GA in August.
