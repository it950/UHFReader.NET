# UHFReader.NET

本项目为 UHFReader18.dll 的 CSharp 版本。

## 从入门到放弃

最开始接触这一块的时候，是因为公安项目需要连接几十台标签读写设备，原本打算用厂家 SDK 进行封装，然后调用即可；

后来发现厂家官方的 SDK 其实是个大大大大坑：内存高（一台大概 2M 左右）、CPU高、易崩溃、无源码不可控、只支持 Windows x86 平台；

连接单台设备还可以接受，若是连接数十台，CPU 跑满还要动不动崩溃，那岂不是要命……

于是弃坑。

## 资料包

对于厂家官方的资料，我做了一些收集，存放在此仓库：<https://github.com/wi1dcard/RFID-Toolkit>

## 基于此扩展的「Rfid Client」项目

为了让这个「弃坑」项目能够发挥一点余热，我还是写了个名叫「Rfid Client」的玩意儿，用于 Web 应用连接 USB 标签读写设备，可用于发行标签的业务场景。

此项目已开源：<https://github.com/wi1dcard/RfidClient>

## 基于设备原始协议的「Rfid Server」项目

弃坑之后，和设备通信的重任，交给了 SuperSocket 身上，真是逼我撸协议...

此项目已开源：<https://github.com/wi1dcard/RfidServer>