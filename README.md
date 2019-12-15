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

## 原型文档

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

request_url = "https://aip.baidubce.com/rest/2.0/face/v3/detect"

params = "{\"image\":\"027d8308a2ec665acb1bdf63e513bcb9\",\"image_type\":\"FACE_TOKEN\",\"face_field\":\"faceshape,facetype\"}"
access_token = '[调用鉴权接口获取的token]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/json'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
- 输出
```
{	
  "face_num": 1,
  "face_list": [
        {
            "face_token": "35235asfas21421fakghktyfdgh68bio",
            "location": { 
                "left": 117,
                "top": 131,
                "width": 172,
                "height": 170,
                "rotation": 4
            },
            "face_probability": 1,
            "angle" :{
                 "yaw" : -0.34859421849251
                 "pitch" 1.9135693311691  
                 "roll" :2.3033397197723  
            }
            "landmark": [  
                {
                    "x": 161.74819946289,
                    "y": 163.30244445801
                },
                ...
            ],
            "landmark72": [ 
                {
                    "x": 115.86531066895,
                    "y": 170.0546875
                }，
                ...
            ],
            "age": 29.298097610474,
            "beauty": 55.128883361816,
            "expression": {
                "type": "smile",
                "probability" : 0.5543018579483
            },
            "gender": {
                "type": "male",
                "probability": 0.99979132413864
            },
            "glasses": {
    			"type": "sun",
                "probability": 0.99999964237213
            },
            "race": {
                "type": "yellow",
                "probability": 0.99999976158142
            },
            "face_shape": {
                "type": "triangle",
                "probability": 0.5543018579483
            }
            "quality": {
                "occlusion": {
                    "left_eye": 0,
                    "right_eye": 0,
                    "nose": 0,
                    "mouth": 0,
                    "left_cheek": 0.0064102564938366,
                    "right_cheek": 0.0057411273010075,
                    "chin": 0
                },
                "blur": 1.1886881756684e-10,
                "illumination": 141,
                "completeness": 1
            }
        }
    ]
}
```
- 测试
- ![首页](https://github.com/Hinata013/api/blob/master/11.png)




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
f = open('[本地文件]', 'rb')
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '[调用鉴权接口获取的token]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
- 输出
```
{
	"log_id": 716033439,
	"labelmap": "xxxx",
	"scoremap": "xxxx",
	"foreground": "xxxx"
}

```

- 测试

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
f = open('[本地文件]', 'rb')
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '[调用鉴权接口获取的token]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
- 输出
```
{
	"log_id": "6876747463538438254",
	"image": "处理后图片的Base64编码"
}
```








