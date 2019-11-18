# intro

目前 2019-11-18 暂时没有找到纯python实现的识别二维码的程序

于是决定自己动手写一个

发现需要解析二维码的结构，有点麻烦(至今没人写出来，说明还是有点原因的)

本着能用就行的策略

使用草料二维码的api来解析二维码内容

使用过程中需要联网，一共调用两个api

# 使用方法

传入图片即可
```python
from qrdecode import qrdecode

r = qrdecode('aa.jpg')
print(r)
```

如果想要识别的二维码是一个url的话，可以
```python
from qrdecode import get_qrdata
img_url = "http://example.com/qrcode.png"
data = get_qrdata(img_url)
```
# 跋

~~等我有空了我就去手写一个python解析二维码的库 :)~~

太难了，放弃


Les1ie

2019-11-18 21:49:54