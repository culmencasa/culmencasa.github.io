## Flutter笔记

### 2022-08-15
在Windows下安装Flutter 3.1, 一直无法编译成功
```
flutter run -d windows
```
报NO CMAKE_CXX_COMPILER could be found.

本地安装的是Visual Studio 2022, 网上的解决方法都是安装VS2019, 重新安装"使用C++的桌面开发"组件.


后来发现本地的Windows 10 SDK(10.0.1.19041.0), 在Viusal Studio Installer里安装单个组件Windows 10 SDK(10.0.20348.0), flutter就能正常编译了.


### 2022-08-16
发现在Windows环境下无法编译linux程序, 需要到linux环境下编译. 



在虚拟机里安装了flutter, 一直无法编译成功. 


```
 throwToolExit (package:flutter_tools/src/base/common.dart:10:3)
```

折腾一天都没有找到原因. 猜测是flutter预览版的bug. 


使用snapd重新安装flutter(之前是手动安装).


问题解决.
