---
layout: page
title: 从0开始学习架构呼叫中心系统（三）
tagline: 软交换：Asterisk与FreeSWITCH
tags : [呼叫中心,电话客服]
comments: true

---
{% include JB/setup %}

####PBX
Private Branch Exchange，电话交换机。在企业应用场景，公司不同部门有很多个分机，而电信公司接入的电话线路是有限的且昂贵的，PBX就是为了解决这个问题而生。它依靠电路交换技术，可以接入多个分机、传真机，控制他们的呼入呼出，分机内部免费拨打。

当然，这个东西是相当贵的，纯硬件，扩展都靠各种板卡，功能比较有限。

![img](https://github.com/kusix/kusix.github.com/raw/master/img/pbx.png)

####IP-PBX时代
可以简单理解为基于TCP/IP的PBX，可以同时接入IP网络和PSTN网络，功能非常强大。例如，可以通过互联网拨打电话（VoIP），IP电话拨不通能自动换用PSTN拨，收发电子传真、邮件，支持IVR、电话录音。支持网络路由、插块GSM扩展卡甚至能接入移动电话。

<!--summary-->

一般它的成本比传统PBX要低些，有两种形式，纯硬件用嵌入式系统的，和基于服务器使用开放操作系统的。

![img](https://github.com/kusix/kusix.github.com/raw/master/img/ip-pbx.png)

####IP-PBX + CTI 构建的呼叫中心
IP-PBX的功能其实已经非常强大，具备基本的呼叫中心的功能，如果在此基础上再加入软件系统去控制电话交换，并接入外围业务系统，那么就可以作为呼叫中心的解决方案了。

下图是用avaya PBX构建的呼叫中心架构，可以看到其中除了语音网关和多媒体服务器，大部分已经软件化，这事实上也是呼叫中心等所有系统发展的趋势，即从昂贵的硬件产品向低廉的软件产品的转移，在实现纯SIP接入后，所有的硬件都会被PC服务器所代替。

![img](https://github.com/kusix/kusix.github.com/raw/master/img/avaya-pbx-cti.png)




####参考

* [《FreeSWITCH与Asterisk的比较》](http://mp.weixin.qq.com/s?__biz=MjM5MzIwMzExMg==&mid=200009467&idx=1&sn=6404aabdce4caba436a71691c89f5607&3rd=MzA3MDU4NTYzMw==&scene=6#rd)   
