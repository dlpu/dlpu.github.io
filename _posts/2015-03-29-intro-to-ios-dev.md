---
layout: post
title: iOS开发介绍
tags : [iOS,Swift]
published: true
---
这篇文章主要是针对iOS零基础入门的同学，介绍一下iOS开发相关的知识体系。给A406研究室的同学学习iOS开发提供一个引导。

###操作系统

Mac OS X 10.10 Yosemite

推荐尽量更新到最新版本的操作系统，苹果发布iOS8以来，针对移动和电脑端的系统都做了进一步的优化，加上iCloud同步云，以淡化iPhone和MacBook笔记本之间的界限，提高整体的用户体验，比如短信和电话在特定情况下可以在电脑端接收。

###终端

Linux命令行

OS X基于UNIX系统的内核，然后进一步开发，在终端的操作命令基本同Linux一致。另外在其他各种基础开发环境的配置过程中，基本和Linux一致，包括使用的开发包，安装的第三方库等，都与Linux兼容。比如pip，npm，homebrew，easy_install等。

###IDE

Xcode（官方）或者 Appcode（三方Jetbrains）

Xcode是苹果官方提供的IDE，功能强大，更新的也快，文档齐全。
同时也有很多开发者喜欢Jetbrains公司开发的Appcode这款IDE，智能提示，debug强大，总之两者各有千秋，可以尝试一下。

###开发语言

Objective-c，swift，兼容C、C++；其他：前端语言HTML+CSS+javascript及其衍生框架如Jquery、PhoneGap

其中Objective-c用于最基础的iOS应用开发，网上现在有着成熟的第三方库，最齐全的视频教程和活跃的开发者社区。另外去年苹果发布iOS8的同时也发布了一门编程语言:swift，在我看来swift降低了编程的难度，不需要去掌握objective-c那么多蹩脚的语法，同时提供了更强大的功能和性能（apple官方宣称swift性能比oc要好）。

Objective-C和swift都与这个LLVM相关，以后可能会看到。在去年发布swift的时候就是那位LLVM创始人`克里斯·拉特纳(Chris Lattner)`展示的swift，他同时也是Clang编译器的作者，膜拜Orz

![Chris Lattner](https://dn-eastio.qbox.me/image/3/1f/a063fab01453450c90b7c87ad5eb7.png?imageView/2/h/400)

###应用开发接口

了解Cocoa及其框架Foundation、UIkit

Cocoa是OS X和iOS操作系统的程序运行环境，基于objective-c。iOS中，Cocoa的框架中最重要最基本的两个框架是Foundation和UIkit，和界面无关的基本类的属于Foundation框架，uikit框架是和界面相关的框架。 

###数据库

一个的本地应用程序sqlite足够，有服务器后台的应用程序在服务器端一般也有很多选择，MySQL，SQL server等等，看具体需求而定，有时本地应用可能需要打通与这些数据库的交互，这样一来又需要网络通信相关的知识。

###开发模式

MVC，稍微复杂一点的应用基本都采用这个架构

> MVC全名是Model View Controller，是模型(model)－视图(view)－控制器(controller)的缩写，一种软件设计典范，用一种业务逻辑、数据、界面显示分离的方法组织代码，将业务逻辑聚集到一个部件里面，在改进和个性化定制界面及用户交互的同时，不需要重新编写业务逻辑。MVC被独特的发展起来用于映射传统的输入、处理和输出功能在一个逻辑的图形化用户界面的结构中。----百度百科

###网络通信

HTTP协议，POST/GET，request/response等，理解之后至少会调用接口。
数据文件：XML，Json

###代码版本控制

Git，Github。

学会使用github的必要性有很多，你可以在github上面学习别人的开源代码，你可以通过github开源自己的项目找到好的工作，甚至你可以向优秀的项目提交你的合并请求，通过Github是最直接最高效的学习方式。

参考廖雪峰的[Git教程](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)

###游戏开发库

Cocos2d，Cocos2d-x，Unity等

游戏开发需要更多的计算机技能，这三个library对应三门语言，分别是Objective-C，C++，C#，具体开发我不是很懂，但基本是这个方向，其中cocos2d和cocos2d-x是免费的。

###制作demo

Facebook开源的origami，社区反映很好，可以尝试一下https://facebook.github.io/origami/

###推荐链接

- [http://objc.io](http://objc.io) ，[中文版](http://objccn.io)
- [猫叔博客](http://onevcat.com) 
- [swift官方文档](https://developer.apple.com/swift/)，[中文版](https://www.gitbook.com/book/numbbbbb/-the-swift-programming-language-/details)
- [官方objective-c文档](https://developer.apple.com/library/ios/documentation/Cocoa/Conceptual/ProgrammingWithObjectiveC/Introduction/Introduction.html#//apple_ref/doc/uid/TP40011210)
- [iOS开发--知乎主题](http://www.zhihu.com/topic/19555404)
- [Code4App](http://code4app.com/)，很多实例代码展示
- [CocoaChina](http://www.cocoachina.com/)，中文Cocoa开发的社区
- [iOS Developer Library](https://developer.apple.com/library/ios/navigation/)，iOS开发官方文档
- [斯坦福大学公开课：iOS7应用开发](http://v.163.com/special/opencourse/ios7.html)，这门课程在iTunes上有最新的iOS8课程。
- 更多直接[戳这](https://github.com/Aufree/trip-to-iOS)

虽然不全，但相信你通过以上链接肯定会发现一个更大的iOS开发的世界。

###推荐书籍

应用程序开发类的书推荐不多，以官方文档为主，同时开源社区有大量代码可以学习，比如github上面，另外特别推荐一个完整的coding.net的iOS客户端[https://coding.net/u/coding/p/Coding-iOS/git](https://coding.net/u/coding/p/Coding-iOS/git)

- 《objective-c程序设计》objective-c的入门语法书。
- 《iOS开发进阶（唐巧）》还有他的博客http://blog.devtang.com

慢慢更新，但不推荐以书籍为主要学习渠道。

###需要联网的应用

服务器后台与Android联网相通：PHP，Java，Python。重点在通过服务器上运行的程序与移动客户端交互。

###苹果开发者账号
iOS和OS X开发需要分别付费，都是$99，折合￥688。

###总结
对于初学者，前半部分介绍就够了，后面多是提供一种学习路线，但就当下来讲，仅仅objective-c和Cocoa就够折腾的了，搭建好环境就从这里着手吧，上手之后善用github等开源社区从代码里和官方文档里学习。

是时候祭出这张图了[https://dn-eastio.qbox.me/iOS-dev.png](https://dn-eastio.qbox.me/iOS-dev.png)




