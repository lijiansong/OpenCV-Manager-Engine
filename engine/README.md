Engine Architecture Design
============================
This archive is the integral architecture design of the engine, which is like a library manager. Not only can it manager the opencv libs, but also it is able to manage any other libs, such as *face detection, voice recognition* and so on. 

## Content

* [AIDL Service Client](#aidl-service-client)
  * [Modules](#modules)
  * [Benefits](#benefits)
* [Code generator](#code-generator)
  * [Features](#features)

## AIDL Service Client
The AIDL Service Client is based on AIDL (Android Interface Definition Language) which is similar to other IDLs you might have worked with. It allows you to define the programming interface that both the client and service agree upon in order to communicate with each other using interprocess communication (IPC) which is based on the underlying *Binder* mechanisms.

### Modules
The technical architecture of the AIDL Service Client is shown below.

![image](https://github.com/lijiansong/OpenCV-Manager-Engine/blob/master/screenshot/arch.png)

### Benefits
Obviously, we can see from the above picture that the AIDL Service Client has the following benefits:
- Less memory usage. All apps use the same binaries from service and do not have to keep the native libs inside themselves;
- Hardware specific optimizations for all supported platforms, such as the different CPU-Arch of Android platform;
- Once the Engine is released, all the Service Libraries will be trusted library source. All packages with OpenCV should be published on Google Play market or Apple's App Store;
- Regular updates and bug fixes;

## Code Generator
Besides the AIDL Service Client, the engine also contains a code generator.

### Features

