---
layout: page
title: 关于DR模式下设置ARP参数的原理
tags : [linux, LVS, 负载均衡, 术]
---
{% include JB/setup %}

####引子
在LVS的DR模式下，我们通常会在RS上设置两个ARP参数，下面我们详细解析设置它们的意义。

####关于arp_ignore



