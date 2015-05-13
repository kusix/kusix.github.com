---
layout: page
title: 从0开始学习架构呼叫中心系统（一）
tagline: 呼叫中心系统相关术语解释
tags : [呼叫中心,电话客服]
comments: true

---
{% include JB/setup %}

![hj-esp8266](https://github.com/kusix/kusix.github.com/raw/master/img/call-center-1.png)

####PSTN
Public Switched Telephone Network，公共交换电话网络，即我们生活中的`电话网`，一种以模拟技术为基础的用于语音通信的电路交换网络。一条通路自建立直至释放，其全部带宽仅能被通路两端的设备使用，即使他们之间并没有任何数据需要传输。

####PBX
Private Branch Exchange，电话交换机，完成企业内部之间以及与公共电信网络的电话交换，并将电话，传真等功能合并，处理分机之间的通话同时再通过主干线与公共交换电话网（PSTN）连接。

####IP-PBX
Private Branch Exchange，电话交换机，完成企业内部之间以及与公共电信网络的电话交换，并将电话，传真，调制解调器等功能合并，处理分机之间的通话同时再通过主干线与公共交换电话网（PSTN）连接。

####CTI
Computer Telephony Integration，计算机电话集成。CTI技术是以电话语音为媒介，用户可以通过电话机上的按键来和呼叫中心的系统交互，基于CTI的呼叫中心使用TDM交换网络传输语音，其核心是基于传统电话交换机和自动呼叫分配系统。

<!--summary-->

####TDM
Time-Division Multiplexing，时分复用，一种数字的或者模拟（较罕见）的多路复用技术。使用这种技术，两个以上的信号或数据流可以同时在一条通信线路上传输，其表现为同一通信信道的子信道。但在物理上来看，信号还是轮流占用物理信道的。时间域被分成周期循环的一些小段，每段时间长度是固定的，每个时段用来传输一个子信道。

####VoIP
Voice over Inertnet Protocol，即指在 IP 网络上使用 IP协议以数据包的方式传输语音。使用 VOIP协议，不管是因特网、企业内部互连网还是局域网都可以实现语音通信。一个使用 VOIP 的网络中，语音信号经过数字化，压缩并转换成 IP 包，然后在 IP 网络中进行传输。

存在一些 VOIP协议栈，它们源于各种标准团体和提供商，如H.323、SIP、MEGACO和MGCP。

####SIP
Session Initiation Protocol，是建立 VOIP 连接的 IETF 标准。一种应用层控制协议，用于和一个或多个参与者创建、修改和终止会话。SIP 的结构与 HTTP （客户－服务器协议）相似。客户机发出请求，并发送给服务器，服务器处理这些请求后给客户机发送一个响应。该请求与响应形成一次事务。

####Trunk
一般指“主干网络、电话干线”，即两个交换局或交换机之间的连接电路或信道，它为两端设备之间进行转接，作为信令和终端设备数据传输链路。

####VoIP Gateway
又称Voip网关、语音网关（Voice Gateway）、多媒体网关（Media Gateway），作用是将传统的电话、传真机或PBX连接到IP网络，将PSTN与IP网络连接起来，从而实现通过Internet网络进行语音通话的功能。


####ACD
Automatic Call Distribution，自动呼叫分发，电话上的路由系统。接受呼叫路由请求，按照一定的分配算法（例如轮询、最长等待时间、第一空闲等）为呼叫分配坐席，记录坐席状态，协助完成转接、抢答、三方通话等业务。

####IVR
Interactive Voice Response，互动式语音应答，在呼叫中心中用于语音导航，使用人工合成的语音，引导用户自助解决问题、输入、或接入指定的坐席组。IVR一般是较为独立的子系统或产品，例如Genesys GVP。

####OCS
Office Communications Server，企业即时通讯服务。Microsoft OCS则专指微软的企业级即时通讯解决方案，提供即时消息 (IM)、状态、Web 会议、音频/视频 (A/V) 会议及电话服务。2010年后被Lync取代。

####参考

* 百度百科
* [《基于SIP的分布式呼叫中心系统设计与实现》作者:安占新](http://www.doc88.com/p-0186174210911.html )   
 

