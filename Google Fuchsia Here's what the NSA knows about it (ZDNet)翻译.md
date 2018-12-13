# Google Fuchsia:美国国家安全局了解到的消息

​	前不久，谷歌明确了Fuchsia不是基于Linux内核的消息，议论谣言遍布，谁也没有确凿的证据能够证明它将能取代Android。但是包括美国国家安全局(NSA)在内的一些组织正在一直调查Fuchisa并且在加拿大温哥华的北美Linux安全峰会公布了调查结果。

### Fuchsia是一个模块化的操作系统。

​	詹姆斯·卡特和斯蒂芬·斯莫利对美国国家安全局透露了一些Fushsia的消息。他们将目光聚集在Fushsia的安全和Zircon的底层微核问题上。 

​	Zircon最开始被作为Android的引导程序，是一个小内核。不过它现在已经被修改成了一个微内核操作系统。它现在包括一小部分用户空间服务、驱动程序和库。这些程序仅仅用于引导系统、与硬件对话、加载用户空间进程并运行它们。内核管理着几种不同的对象类型，从而可通过系统调用直接访问C++类。Fuchsia 就是以此基础建立的。

​	Zircon是个模块化的操作系统，这意味着不仅在PC能够运行，在低功耗、最低资源的设备上也能使用它。只需添加对象模块即可获得更多功能。

### Fuchsia看起来像Unix/Linux

​	Fuchsia还支持便携式操作系统接口(POSIX)协议。

​	这意味着，从开发人员的角度来看，它看起来像unix/linux。Fuchsia 使用谷歌的Flutter框架作为软件开发工具包(SDK)。有了它，你可以构建Chrome OS和Android应用程序。Fuchsia也支持苹果的Swift语言。

### Fuchsia面临许多安全问题

​	斯莫利和卡特的工作是调查操作系统和软件在国家安全工作中的潜在隐患。简而言之，看它是否容易被破坏。美国国家安全局不希望政府使用脆弱的系统。

​	卡特还帮助美国国家安全局创造了运行最安全的Linux系统——SELinux。在查看Zircon和Fuchsia时，他们分享了关于操作系统的发现。

​	首先，他们发现Zircon是Fuchsia唯一以管理模式运行的部分。其他一切的驱动程序、文件系统、网络等都是在用户模式下运行的。这意味着有关Fuchsia的程序将采取与大多数操作系统程序不同的方法。

​	在深入研究的同时，他们也发现了许多安全问题。例如，Carter说，“你可以系统工作的任何地方获得句柄，”自然地，“句柄的泄漏对安全是致命的。”

### Fuchsia还有许多工作要做

​	Fuchsia的问题很大，到今年夏天，它还远远没有准备好生产。正如卡特所解释的，Fuchsia在很大程度上是一个“正在进行中的工作”系统，在 Fuchsia足够安全之前“需要做很多工作”。

​	与Linux相比，Fuchsia仍然不成熟，安全也远远不够。

​	但是，卡特说，虽然“许多工作”需要做，但它会变得更安全，他鼓励开源开发人员帮助谷歌锁定在Fuchsia的安全上。

​	不管成熟与否，Fuchsia可能很快就会用在谷歌的Home Hub上

### Fuchsia是否会应用在谷歌的Home Hub上？

​	Home Hub是一种新型的物联网设备，它本质上是一个7英寸触摸屏。它包括一个全距离扬声器，一个光传感器，和两个远场麦克风，不包括摄像机。但是，在底层上，它将使用Amlogic S905D2的CPU，而不是高通SD 624 SoC。

 	一些人在*9to5Google*疯狂报道Fuchsia，并且不断挖掘GoogleHome Hub的源代码。他们发现了Fuchsia的踪迹。这意味着Home Hub可能会在圣诞时就会运行着Fuchsia！

Will you want to? No, based on what the NSA found, I'd say not. But, if you want to tinker with Fuchsia, it might be worth getting the new Google Home Hub.

​	不过根据国安局的发现，Fuchsia还有很多问题。但是，如果你想体验Fuchsia，新的Home Hub是值得期待的。



****

本文作者为社区成员：VicZ，题图及内容翻译自

https://www.zdnet.com/article/google-fuchsia-heres-what-the-nsa-knows-about-it/