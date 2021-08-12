# WearDevice
关于穿戴设备绑交通卡的一些记录

设备和app之前的数据交互通过蓝牙
## TLV
数据的格式为TLV -- tag length value tag指一种标记 length指后面value的长度
## 绑定交通卡
穿戴设备中有一个eSE芯片 就是安全芯片
1. 在eSE芯片中创建一块安全的区域SSD
2. app向卡商服务器申请一个applet（java应用程序） 每张卡对应一个applet
3. 通过数据传输 把这个applet传入到硬件设备中
4. 向卡商服务器（TSM）请求数据包（余额、行程信息）下载到applet中进行交互
