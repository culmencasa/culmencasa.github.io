---
layout: post
title:  "RDP Wrapper INI for termsrv.dll 10.0.18362.836"
date:   2021-01-10 10:34:0
categories: 随记
tags: [windows,system]
---
#### 远程桌面多用户连接18362.836 INI配置文件

以前用过[RDP Wrapper](https://github.com/stascorp/rdpwrap/releases)，直接安装就好了，今天在公司电脑上发现不支持当前Windows版本。 

在Winver中看到我的版本是*1909(内部版本18363.1256)*,  
在RDP Wrapper程序中显示的版本号则是**10.0.18362.836**,  
应该是termsrv.dll文件的版本号吧。


运行Update.bat也找不到对应的配置文件。  

后来找到[这篇文章](https://blog.csdn.net/az9996/article/details/109406102)，
才在github的[issue#1187](https://github.com/stascorp/rdpwrap/issues/1187)里找到答案


- 可以直接[下载INI](https://raw.githubusercontent.com/affinityv/INI-RDPWRAP/master/rdpwrap.ini)
- 或者百度网盘：
[链接地址](https://pan.baidu.com/s/1W5e-vqvdMin9ubX4-AnIlw) 
提取码：099f 


替换C:\Program Files\RDP Wrapper下的rdpwrap.ini，再运行RDPConf.exe可以是看到fully supported了。
