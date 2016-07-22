# OpenCV-Manager-Engine
===
This archive is the source code of OpenCV Manger which refer to OpenCV tutorial,implemented by Java,on the android platform.

I have been coding an platform recently,which can manage library binaries on end users devices,such as android,iOS and so on.

The platform is a Service Store,which just like the app store in android,where delelopers develop their own apps and deploy them
onto the app store,and users can download the app that they like and install it on his or her devices.Therefore,android's app 
store can be treated as an ecological system.

However,our Service Store is also an ecological system,where the Service Manufacture or Lib Developers can develop their own Cloud Services or Native Services,and users can connect to the service they like on their end devices,such as *Voice Recognition Service*,*Face Detection Service* and so on.The technical architecture of the platform is shown below.

** Technical Architecture**

![image](https://github.com/lijiansong/OpenCV-Manager-Engine/blob/master/screenshot/arch.png)

Introduction
---
Refer to the OpenCV Manager Mauual.

OpenCV Manager is an Android service targeted to manage OpenCV library binaries on end users devices. It allows sharing the OpenCV dynamic libraries between applications on the same device. The Manager provides the following
benefits:
- Less memory usage. All apps use the same binaries from service and do not keep native libs inside themselves;
- Hardware specific optimizations for all supported platforms;
- Trusted OpenCV library source. All packages with OpenCV are published on Google Play market;
- Regular updates and bug fixes;



