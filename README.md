# 产品需求
|  发布时间  | 2019年12月5日  |
|  ----  | ----  |
| 产品名称  | 在线证件照图片制作APP |
| 完成进度  | 最后修改部分 |
| 文件主人  | 林泽伟 |
| 设计师  | 林泽伟 |
| 开发者  | 林泽伟 |

# 背景
- 在过去电子产品不发达的时期，只需要用到实体的证件照，去到实体店拍摄裁剪，而现在信息发达，越来越多的线上资料需要用到电子图片形式的证件照，这时，在线上在线制作证件照图片的需求也就不断增加，人工智能API的发展，给我们提供了更多方便的渠道，方便快捷的去在线上制作证件照图片。





# 核心价值主张
## 加值宣言
使证件照图片制作简单便捷，规范。
### 主要
- 在拍照时通过百度的人脸检测API中的人脸关键点检测功能，可以检测人脸旋转角度，帮助用户拍出更加符合规范的正面照片；
- 拍照结束后，通过百度人像分割API，识别人体的轮廓范围，取得透明背景的人像图，取最重要的部分；
### 辅助
- 结束背景与人像分离后，用户有可能在调整人像大小是过渡拉伸图片，这时可以通过百度拉伸图像恢复API，在用户截取完合适大小的人像后，自动识别过度拉伸的图像，将图像内容恢复成正常比例，使证件照图片更加规范。

## 核心价值	
- 为用户在线提供方便快捷，而且清晰的证件照图片制作平台。



## 核心价值与用户痛点
 很多人去店里拍证件照的时候，会取到实体的照片，并不会留意，或者专门跟老板要电子版的证件照图片，但时有些时候却需要用到线上的证件照，例如线上的简历投递，学生作业需要等等情况，用户会遇到以下几个问题：
- 专门前往实体店找老板拍摄电子照片没有必要，找回之前拍摄的记录又麻烦又耽误老板时间；专门去实体店拍照电子版照片时也需要等待排队，花费较多时间。
- 突然需要图片的，时间比较赶，来不及去实体店拍摄，或者参与店家休息时段。
- 现在已经有的在线证件照制作产品不会在用户拍照时给予角度的检测，可能导致拍摄的证件照不规范。
- 同样是同类产品，选择用户想要的证件照尺寸后，用户人像大小靠用户自己截取，可能导致人像过大，或者人像拉伸失衡。
## 人工智能概率性与用户痛点
- 人脸检测api：access_token的有效期为30天，切记需要每30天进行定期更换，或者每次请求都拉取新token；不支持GIF图片。
- 人像分割api：请求图片需经过base64编码：图片的base64编码指将一副图片数据编码成一串字符串，使用该字符串代替图像地址。

## 需求列表与人工智能API加值
|  需求  | API | 重要程度 |
|  ----  | ----  | ---- |
| 使拍出来的人像处于正面，更加符合规范  | 百度人脸检测API | 重要|
| 分割人像与背景 | 百度人像分割API | 重要 |
| 自动识别过度拉伸的图像，将图像内容恢复成正常比例，使证件照图片更加规范  | 百度拉伸图像恢复API | 次要 |

## 具体产品
- 场景一：就业指导课上，老师布置了模拟简历的作业，在老师给出的模板上修改填写自己的信息，其他的工作进行得都很顺利，但是就是找不到证件照的电子图片，手头上是有实体证件照，但是无法使用，有不想要专门去实体店拍摄网上使用的图片，于是使用在线证件照制作，制作一张线上使用的证件照图片。
- 场景二：A同学参加了从化创新就业大赛，需要每个参赛小组的成员都填写基本信息，其中就需要证件照图片，而A同学在学校，无法去找原先拍摄证件照的店家取线上的照片，使用使用在线证件照制作，完成了证件照图片制作。

# 原型
## 交互及界面
- ![首页](https://github.com/Hinata013/api/blob/master/11.png)
- ![一页](https://github.com/Hinata013/api/blob/master/22.png)
- ![二页](https://github.com/Hinata013/api/blob/master/3.png)
- ![三页](https://github.com/Hinata013/api/blob/master/4.png)
- ![四页](https://github.com/Hinata013/api/blob/master/5.png)
- ![五页](https://github.com/Hinata013/api/blob/master/6.png)
- ![六页](https://github.com/Hinata013/api/blob/master/7.png)
## 信息设计
- ![产品结构图](https://github.com/Hinata013/api/blob/master/111.png)
- ![信息结构图](https://github.com/Hinata013/api/blob/master/222.png)
- ![使用流程图](https://github.com/Hinata013/api/blob/master/333.png)

## 原型文档
[原型](http://nfunm053.gitee.io/api_passport_photo/#id=pfqphn&p=%E9%A6%96%E9%A1%B5)
[原型文档下载](https://github.com/Hinata013/api/blob/master/%E5%9C%A8%E7%BA%BF%E8%AF%81%E4%BB%B6%E7%85%A7%E5%88%B6%E4%BD%9Capp.rp)

## 口头操作说明
- 在线证件照制作产品主要用于需要使用到证件照电子图片的时候，使用普通人使用手机拍摄出来的照片肯定是不然实体店专业是摄影师拍摄出来的规范，使用在制作过程中，产品使用API来辅助用户，百度人脸关键点检测api可以检测用户人脸角度，反馈准确的角度偏差，无论是仰俯视角度，还是正侧脸角度，精准的数据反馈更加能辅助用户拍摄角度的规范性，而人像分割则是能直接分割出人像，在选取背景颜色之后就基本上完成制作了，在产品最开始使用是，还会提供各个尺寸规格供用户选择，在用户分割完人像之后，产品还会使用到百度拉伸图像恢复API，经常图片人像是否拉伸过度，这些都是为了制作出来的证件照图片更加规范，实体的证件照绝大多数人都有，但是当某些时候需要线上图片时，却发现平常不太留意，就可以使用本产品，花费不到10分钟的时间制作一张。

# API 产品使用关键AI或机器学习之API的输出入展示
## 使用水平
### 百度人脸检测API
- 接口描述：如果需要判断一张图片中的人脸，是否符合后续识别或者对比的条件，可以使用此接口，在请求时在face_field参数中请求quality。基于返回结果quality中，以下字段及对应阈值，进行质量检测的判断，以保证人脸质量符合后续业务操作要求。
- 输入
```
# encoding:utf-8
 import requests

 '''
 人脸检测与属性分析
 '''

import urllib.request,sys,base64
import urllib.parse
request_url = "https://aip.baidubce.com/rest/2.0/face/v3/detect"

f = open('q3.jpg', 'rb')
image = base64.b64encode(f.read())
image64 = str(image,'utf-8')
image_type = "BASE64"




params = {'image': image64,'image_type':"BASE64",'face_field': 'faceshape,facetype'}

params = urllib.parse.urlencode(params).encode("utf-8")


access_token = '[24.b5ff1af7ad57860f4a47b0972dd0560f.2592000.1579764577.282335-18098227]'
request_url = request_url + "?access_token=" + access_token

request = urllib.request.urlopen(url=request_url, data=params)   

content = request.read()  
print(content) 

```
- 输出
```
(b'{"error_code":0,"error_msg":"SUCCESS","log_id":19955551594,"timestamp":15771'
 b'72758,"cached":0,"result":{"face_num":1,"face_list":[{"face_token":"3d44d56f'
 b'3d2d41190368b2697023d5f2","location":{"left":235.97,"top":819.91,"width":426'
 b',"height":446,"rotation":0},"face_probability":0.95,"angle":{"yaw":-7.9,"pit'
 b'ch":-5.58,"roll":-4.76},"face_shape":{"type":"square","probability":0.52},"f'
 b'ace_type":{"type":"human","probability":1}}]}}')

```
- 测试
- ![测试1](https://github.com/Hinata013/api/blob/master/c1.png)
- ![测试2](https://github.com/Hinata013/api/blob/master/c2.png)




### 百度人像分割API
- 接口描述：对于输入的一张图片（可正常解码，且长宽比适宜），识别人体的轮廓范围，与背景进行分离，适用于拍照背景替换、照片合成、身体特效等场景。输入正常人像图片，返回分割后的二值结果图、灰度图、透明背景的人像图（png格式）。
- 输入
```
# encoding:utf-8

import requests
import base64

'''
人像分割
'''

request_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/body_seg"
# 二进制方式打开图片文件
f = open('A.jpg', 'rb')
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '[24.98a36d5af188e07b1dd272e73f7c3856.2592000.1579526413.282335-18081421]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
- 输出部分过长，用截图方式体现

- 测试
- ![测试3](https://github.com/Hinata013/api/blob/master/c3.png)
- ![测试4](https://github.com/Hinata013/api/blob/master/c4.png)
- ![测试5](https://github.com/Hinata013/api/blob/master/77.jpg)


### 百度拉伸图像恢复API
- 接口描述：自动识别过度拉伸的图像，将图像内容恢复成正常比例。
- 输入
```
# encoding:utf-8

import requests
import base64

'''
拉伸图像恢复
'''

request_url = "https://aip.baidubce.com/rest/2.0/image-process/v1/stretch_restore"
# 二进制方式打开图片文件
f = open('A.jpg', 'rb')
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '[24.05e223be25d6ed71278879f33b6626f5.2592000.1579524842.282335-18081330]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
- 输出部分过长，用截图方式体现

- 测试
- ![测试5](https://github.com/Hinata013/api/blob/master/c5.png)
- ![测试6](https://github.com/Hinata013/api/blob/master/c6.png)
- ![测试7](https://github.com/Hinata013/api/blob/master/88.jpg)

## 使用比较分析 
### 与百度人像分割API对比
#### 阿来云智能人像分割（抠图）API：
- 优点： 1、分割精度高，准确率高，速度快。 2、支持软分割，可返回每个像素判为人像的概率，适合在图像合成中应用。
- 缺点：免费只有试用套餐，收费使用价格较高，头发处理有瑕疵。
#### 选择百度云的原因：
- 人像分割算法业界领先，评测IoU 90%以上，并基于应用反馈和场景数据持续迭代优化；可提供企业级稳定、精确的大流量服务，拥有毫秒级识别响应能力及99.9%的可靠性保障；性价比更高。
#### 价格对比
- ![百度](https://github.com/Hinata013/api/blob/master/baidu3.png)
- ![百度22](https://github.com/Hinata013/api/blob/master/baidu4.png)
- ![face](https://github.com/Hinata013/api/blob/master/al.png)
### 与百度人脸检测API对比
#### FACE++人脸检测API：
- 优点：高效准确，获得国际多项大奖
- 缺点：对使用的图片要求相对较高，如果一个 face_token 在 72 小时内没有存放在任一 FaceSet 中，则该 face_token 将会失效。
#### 选择百度云的原因：
- 百度人脸检测API算法在最权威的公开评测比赛中排名世界领先，也有着很高的准确率，而且使用更加方便，对图片要求跟低，更有利于普通人，而且access_token的有效期为30天，更加有利。
#### 价格对比
- ![百度11](https://github.com/Hinata013/api/blob/master/baidu1.png)
- ![阿里](https://github.com/Hinata013/api/blob/master/face.png)
### 百度拉伸图像恢复API暂时找不到其他竞品API


## 使用后风险报告 
### 百度人像分割API:
- 对输入图片质量要求较高，对清晰度有一定要求；
- 最短边至少50px，最长边最大4096px；
- 要求base64编码和urlencode后大小不超过4M。
### 价格
- ![baidu](https://github.com/Hinata013/api/blob/master/baidu3.png)
- ![百度222](https://github.com/Hinata013/api/blob/master/baidu4.png)
### 百度人脸检测API：
- 准确率达到99.99%，对用户体验的负面影响不会压过正面影响的机率；
- access_token的有效期为30天，切记需要每30天进行定期更换，或者每次请求都拉取新token；
- 请求的图片需经过Base64编码，图片的base64编码指将图片数据编码成一串字符串，使用该字符串代替图像地址。需要注意图片的base64编码是不包含图片头，如data:image/jpg;base64；
- 不支持GIF图片；
- 竞争对手较多，如FACE++,腾讯云，Azure，阿里云
### 价格
- ![baid2](https://github.com/Hinata013/api/blob/master/baidu1.png)
### 百度拉伸图像恢复API：
- 请求图片需经过base64编码；
- base64编码后大小不超过4M，最短边至少64px，最长边最大4096px，长宽比3:1以内；
- 属于新的API项目，暂无竞争对手，越来越多的工作对图片的规格，规范性有很高的要求，恢复拉伸的前景加优良；
- 新产品暂无合作项目，对比不明显。
### 价格
- 每个账户一次性共3000次免费使用机会
- 0<月调用量<=300	 时8万元1000次
- 300<月调用量 时4.8万元1000次
### 使用情况
- 通过百度搜索，bing，搜狗搜索发现，百度API相比于其他竞品应用更加规范，而且提供了更加详细的使用教程，具更加广泛的市场。
## 加分项
- 使用了百度人脸检测API，人像分割API，拉伸图像恢复API









