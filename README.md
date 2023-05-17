﻿
# 跨平台屏幕共享演示DEMO（Windows Android）

本仓库通过屏幕共享DEMO演示了点对点弱网传输SDK的使用。

## SDT点对点弱网传输SDK介绍
本SDK依托QOS-FEC-NACK传输层内核，用于解决3G、4G、WIFI网络时面临的丢包、乱序、重复、抖动等问题。SDK采用极简的接口设计，让用户快速集成。具体接口文档请参考：https://mediapro.apifox.cn


## DEMO说明
本投屏windows端使用SDT点对点内置编解码SDK开发，UI使用Duilib，DEMO实现了投屏发送、投屏播放一体化，操作简易。

1. 投屏发送时，输入远端投屏码（投屏码由远端IP和端口转化而来）
![1.png](https://api.apifox.cn/api/v1/projects/2558265/resources/382263/image-preview)


2. 投屏播放时，启动后画面如下

![4.png](https://api.apifox.cn/api/v1/projects/2558265/resources/382265/image-preview)

3. 可通过UI设置投屏参数
 
![3.png](https://api.apifox.cn/api/v1/projects/2558265/resources/382270/image-preview)

4. 跟多高级参数可通过配置文件ScreenShareDemo.ini中手工设置，比如
AutoResolutionEnable用于控制是否使能分辨率自适应，允许码率降低到一定程度时降低分辨率以降低块效应。
LongTimeRefEnable用于控制是否使能长期参考帧机制，目前仅在软编码时支持长期参考帧机制，该机制可以提高弱网下画面的流畅性，但对编码画质有较大副作用。

5. 本投屏Windows端可以与Android端互通

![Alt](http://www.mediapro.cc/wp-content/uploads/2019/04/1-1.png)
![Alt](http://www.mediapro.cc/wp-content/uploads/2019/04/5.png)




