---
layout: post
title:  "Ubuntu20.04 访问Vmware共享文件夹"
date:   2020-07-23 22:39:0
categories: 随记
tags: [ubuntu,system]
---

Windows 10 Vmware下安装Ubuntu20.04后，设置共享文件夹后，在Terminal里执行
```
sudo vmhgfs-fuse .host:/ /mnt/hgfs/ -o allow_other -o uid=1000
```

然后
```
ln -s /mnt/hgfs/HostDownload/ ~/MappedDownload
```
