# intro
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
由于本人太菜并且太懒，不想去解析二维码的结构，只有用现成的api

等我有空了我就去手写python解析二维码 :)