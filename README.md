
[TOC]
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
| 使拍出来的人像处于正面，更加符合规范  | 百度人脸检测API | 重要
| 分割人像与背景 | 百度人像分割API | 重要 |
| 自动识别过度拉伸的图像，将图像内容恢复成正常比例，使证件照图片更加规范  | 百度拉伸图像恢复API | 次要 |

## 具体产品
- 场景一：就业指导课上，老师布置了模拟简历的作业，在老师给出的模板上修改填写自己的信息，其他的工作进行得都很顺利，但是就是找不到证件照的电子图片，手头上是有实体证件照，但是无法使用，有不想要专门去实体店拍摄网上使用的图片，于是使用在线证件照制作，制作一张线上使用的证件照图片。
- 场景二：A同学参加了从化创新就业大赛，需要每个参赛小组的成员都填写基本信息，其中就需要证件照图片，而A同学在学校，无法去找原先拍摄证件照的店家取线上的照片，使用使用在线证件照制作，完成了证件照图片制作。


# 原型
## 交互及界面
- 1、登录页面
- ![登录](https://github.com/Hinata013/api/blob/master/a.png)
- 1.1、取消授权返回页面
- ![登录返回](https://github.com/Hinata013/api/blob/master/b.png)
- 2、首页
- ![首页](https://github.com/Hinata013/api/blob/master/11.png)
- 2.1、尺寸选择页面
- ![一页](https://github.com/Hinata013/api/blob/master/22.png)
- 3、在相册选择图片1
- ![相册](https://github.com/Hinata013/api/blob/master/c.png)
- 3.1、拍摄图片
- ![二页](https://github.com/Hinata013/api/blob/master/3.png)
- 4、去除背景完成
- ![三页](https://github.com/Hinata013/api/blob/master/4.png)
- 5、拉伸修复完成
- ![四页](https://github.com/Hinata013/api/blob/master/5.png)
- 6、制作完成
- ![五页](https://github.com/Hinata013/api/blob/master/6.png)
- 7、我的界面
- ![六页](https://github.com/Hinata013/api/blob/master/7.png)
## 信息设计
- 1、产品结构图
- ![产品结构图](https://github.com/Hinata013/api/blob/master/111.png)
- 2、信息结构图
- ![信息结构图](https://github.com/Hinata013/api/blob/master/222.png)
- 3、使用流程图
- ![使用流程图](https://github.com/Hinata013/api/blob/master/333.png)
- 4、产品原型流程图
- ![流程图](https://github.com/Hinata013/api/blob/master/d.png)
- 4.1、产品原型流程图2
- ![流程图1](https://github.com/Hinata013/api/blob/master/e.png)

## 原型文档
- [原型](http://nfunm053.gitee.io/api_passport_photo/#id=pfqphn&p=%E9%A6%96%E9%A1%B5)
- [原型文档下载](https://github.com/Hinata013/api/blob/master/%E5%9C%A8%E7%BA%BF%E8%AF%81%E4%BB%B6%E7%85%A7%E5%88%B6%E4%BD%9Capp.rp)

## 口头操作说明
- 在线证件照制作产品主要用于需要使用到证件照电子图片的时候，使用普通人使用手机拍摄出来的照片肯定是不然实体店专业是摄影师拍摄出来的规范，使用在制作过程中，产品使用API来辅助用户，百度人脸关键点检测api可以检测用户人脸角度，反馈准确的角度偏差，无论是仰俯视角度，还是正侧脸角度，精准的数据反馈更加能辅助用户拍摄角度的规范性，而人像分割则是能直接分割出人像，在选取背景颜色之后就基本上完成制作了，在产品最开始使用是，还会提供各个尺寸规格供用户选择，在用户分割完人像之后，产品还会使用到百度拉伸图像恢复API，经常图片人像是否拉伸过度，这些都是为了制作出来的证件照图片更加规范，实体的证件照绝大多数人都有，但是当某些时候需要线上图片时，却发现平常不太留意，就可以使用本产品，花费不到10分钟的时间制作一张。

# API 产品使用关键AI或机器学习之API的输出入展示
## 使用水平
### 百度人脸检测API
- [百度人脸检测API文档](https://ai.baidu.com/ai-doc/FACE/yk37c1u4t)
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
- 在线测试结果图
- ![测试1](https://github.com/Hinata013/api/blob/master/c1.png)
- ![测试2](https://github.com/Hinata013/api/blob/master/c2.png)




### 百度人像分割API
- [ 百度人像分割API文档](https://ai.baidu.com/ai-doc/BODY/Fk3cpyxua)
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

- 在线测试结果图测试
- ![测试3](https://github.com/Hinata013/api/blob/master/c3.png)
- ![测试4](https://github.com/Hinata013/api/blob/master/c4.png)
- 自行测试输出结果
- ![测试5](https://github.com/Hinata013/api/blob/master/77.jpg)


### 百度拉伸图像恢复API
- [百度拉伸图像恢复API文档](https://ai.baidu.com/ai-doc/IMAGEPROCESS/Rk3bclp97)
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

- 在线测试结果图
- ![测试5](https://github.com/Hinata013/api/blob/master/c5.png)
- ![测试6](https://github.com/Hinata013/api/blob/master/c6.png)
- 自行测试输出结果
- ![测试7](https://github.com/Hinata013/api/blob/master/88.jpg)

## 使用比较分析 
### 与百度人像分割API对比
#### 主要竞争者-阿里云智能人像分割（抠图）API：
- 优点： 1、分割精度高，准确率高，速度快。 2、支持软分割，可返回每个像素判为人像的概率，适合在图像合成中应用。
- 缺点：免费只有试用套餐，收费使用价格较高，头发处理有瑕疵。
#### 阿里云代码测试
- 输入
```
# -*- coding: utf8 -*-
import requests, os
import json
import hashlib, base64, hmac

app_key = 'LTAI4FhaXP4Te7bz2myVCJAX'
secret = 'oduJHNWG7qsI4w3mOebWfpxZp7AhNT'
file_name = '31313.jpg'

stage = 'RELEASE' # 正式环境
#stage = 'TEST' # 测试环境

host = 'https://aliapi.aisegment.com'  # 抠图接口
uri = '/segment/matting'

#host = 'https://alidphoto.aisegment.com' # 证件照接口
#uri = '/idphoto/make'

#host = 'https://ecimage.market.alicloudapi.com' # 商品裁剪接口
#uri = '/commodity/crop'


def params_of_matting(photo_base64, photo_type):
    return {
        'photo': photo_base64,
        'type': photo_type
    }


def params_of_idphoto(photo_base64, photo_type):
    return {
        'photo': photo_base64,
        'type': photo_type,
        'spec': '2',
        'bk': 'white'
    }


def params_of_crop(photo_base64):
    return {
        'photo': photo_base64,
        'output_size': [600, 800], #
        'object_ratio': 0.9
    }


def test_segment():

    api = host + uri

    with open(file_name,'rb') as fp:
        photo_base64 = base64.b64encode(fp.read())

    _, photo_type = os.path.splitext(file_name)
    photo_type = photo_type.lstrip('.')

    #body_json = params_of_matting(photo_base64, photo_type)
    body_json = params_of_idphoto(photo_base64, photo_type)
    #body_json = params_of_crop(photo_base64)

    body = json.dumps(body_json)
    md5lib = hashlib.md5()
    md5lib.update(body)
    body_md5 = md5lib.digest()
    body_md5 = base64.b64encode(body_md5)

    method = 'POST'
    accept = 'application/json'
    content_type = 'application/octet-stream; charset=utf-8'
    date_str = ''
    headers = ''

    string_to_sign = method + '\n' \
                    + accept + '\n' \
                    + body_md5 + '\n' \
                    + content_type + '\n' \
                    + date_str + '\n' \
                    + headers \
                    + uri
    signed = hmac.new(secret, string_to_sign, digestmod=hashlib.sha256).digest()
    signed = base64.b64encode(signed)

    headers = {
        'Accept': accept,
        'Content-MD5': body_md5,
        'Content-Type': content_type,
        'X-Ca-Key': app_key,
        'X-Ca-Stage': stage,
        'X-Ca-Signature': signed
    }
    #print signed

    resp = requests.post(api, data=body, headers=headers)
    try:
        res = resp.content
        res = json.loads(res)
        print ('res:', res)
        if str(res['status']) == '0':
            print ('成功!')
        else:
            print ('失败!')
    except:
        print('failed parse:', resp)


if __name__ == "__main__":
    test_segment()
```
- 输出
```
{'status': 0, 'data': {'result': https://photogallery.oss.aliyuncs.com/photo/1372101300429605/undefined/0b41c8e0-93a1-4e94-adec-1b3e272a71fd.jpg'}}
```
#### 选择百度云的原因：
- 人像分割算法业界领先，评测IoU 90%以上，并基于应用反馈和场景数据持续迭代优化；可提供企业级稳定、精确的大流量服务，拥有毫秒级识别响应能力及99.9%的可靠性保障；性价比更高。
- 通过输出效果图对比发现，百度的api相比阿里云的人像边缘部分处理的略好一些，相对没那么生硬，自然一些。
#### 价格（性价比）对比
##### 百度价格
- ![百度](https://github.com/Hinata013/api/blob/master/baidu3.png)
- ![百度22](https://github.com/Hinata013/api/blob/master/baidu4.png)
- 按QPS（并发量）计费： 调用量免费，免费QPS默认为2，如果您通过百度云的企业认证，接口的免费QPS将扩充至5。同时您可以根据业务需求随时购买扩充QPS，QPS可包月购买，也可按天单独购买，灵活多样，适应多场景需求。 当前人体关键点识别、人体检测与属性识别、人流量统计、人像分割、手势识别5个接口支持在线购买QPS。 注意：同一个账号下多个应用共享接口QPS。
- 按调用量计费： 免费调用量限额用完后，可选择购买次数包 或开通 按调用量后付费 两种计费方式付费使用，两种付费方式均可在 控制台 直接开通或购买，开通付费后默认按量后付费的方式进行阶梯计费，如有购买对应服务的次数包，则优先消耗次数包额度，抵扣完毕后自动转为按量后付费方式。 当前驾驶行为分析接口采用按调用量计费的方式。
##### 阿里云价格
- ![face](https://github.com/Hinata013/api/blob/master/al.png)
### 与百度人脸检测API对比
#### 主要竞争者-FACE++人脸检测API：
- 优点：高效准确，获得国际多项大奖
- 缺点：对使用的图片要求相对较高，如果一个 face_token 在 72 小时内没有存放在任一 FaceSet 中，则该 face_token 将会失效。
#### Face++代码测试
- 输入
```
# -*- coding: utf-8 -*-
import urllib.request
import urllib.error
import time

http_url = 'https://api-cn.faceplusplus.com/facepp/v3/detect'
key = "1xZt600gnMyz6dVd0BWOlwyRBNsrUbbT"
secret = "vIXKcdwlvJf6nhtMNct0mim9LisJeO66"
filepath = r"31313.jpg"

boundary = '----------%s' % hex(int(time.time() * 1000))
data = []
data.append('--%s' % boundary)
data.append('Content-Disposition: form-data; name="%s"\r\n' % 'api_key')
data.append(key)
data.append('--%s' % boundary)
data.append('Content-Disposition: form-data; name="%s"\r\n' % 'api_secret')
data.append(secret)
data.append('--%s' % boundary)
fr = open(filepath, 'rb')
data.append('Content-Disposition: form-data; name="%s"; filename=" "' % 'image_file')
data.append('Content-Type: %s\r\n' % 'application/octet-stream')
data.append(fr.read())
fr.close()
data.append('--%s' % boundary)
data.append('Content-Disposition: form-data; name="%s"\r\n' % 'return_landmark')
data.append('1')
data.append('--%s' % boundary)
data.append('Content-Disposition: form-data; name="%s"\r\n' % 'return_attributes')
data.append(
    "gender,age,smiling,headpose,facequality,blur,eyestatus,emotion,ethnicity,beauty,mouthstatus,eyegaze,skinstatus")
data.append('--%s--\r\n' % boundary)

for i, d in enumerate(data):
    if isinstance(d, str):
        data[i] = d.encode('utf-8')

http_body = b'\r\n'.join(data)

# build http request
req = urllib.request.Request(url=http_url, data=http_body)

# header
req.add_header('Content-Type', 'multipart/form-data; boundary=%s' % boundary)

try:
    # post data to server
    resp = urllib.request.urlopen(req, timeout=5)
    # get response
    qrcont = resp.read()
    # if you want to load as json, you should decode first,
    # for example: json.loads(qrount.decode('utf-8'))
    print(qrcont.decode('utf-8'))
except urllib.error.HTTPError as e:
    print(e.read().decode('utf-8'))
```
- 输出
```
{"time_used": 319, "faces": [{"landmark": {"mouth_upper_lip_left_contour2": {"y": 365, "x": 652}, "mouth_upper_lip_top": {"y": 360, "x": 681}, "mouth_upper_lip_left_contour1": {"y": 358, "x": 671}, "left_eye_upper_left_quarter": {"y": 226, "x": 597}, "left_eyebrow_lower_middle": {"y": 195, "x": 607}, "mouth_upper_lip_left_contour3": {"y": 371, "x": 659}, "right_eye_top": {"y": 220, "x": 741}, "left_eye_bottom": {"y": 245, "x": 612}, "right_eyebrow_lower_left_quarter": {"y": 186, "x": 723}, "right_eye_pupil": {"y": 230, "x": 743}, "mouth_lower_lip_right_contour1": {"y": 372, "x": 703}, "mouth_lower_lip_right_contour3": {"y": 385, "x": 698}, "mouth_lower_lip_right_contour2": {"y": 379, "x": 712}, "contour_chin": {"y": 454, "x": 685}, "contour_left9": {"y": 448, "x": 649}, "left_eye_lower_right_quarter": {"y": 243, "x": 629}, "mouth_lower_lip_top": {"y": 373, "x": 682}, "right_eyebrow_upper_middle": {"y": 169, "x": 742}, "left_eyebrow_left_corner": {"y": 195, "x": 566}, "right_eye_bottom": {"y": 241, "x": 743}, "contour_left7": {"y": 412, "x": 597}, "contour_left6": {"y": 388, "x": 578}, "contour_left5": {"y": 361, "x": 564}, "contour_left4": {"y": 331, "x": 554}, "contour_left3": {"y": 302, "x": 547}, "contour_left2": {"y": 272, "x": 541}, "contour_left1": {"y": 240, "x": 538}, "left_eye_lower_left_quarter": {"y": 242, "x": 597}, "contour_right1": {"y": 231, "x": 811}, "contour_right3": {"y": 292, "x": 807}, "contour_right2": {"y": 262, "x": 811}, "mouth_left_corner": {"y": 374, "x": 636}, "contour_right4": {"y": 322, "x": 802}, "contour_right7": {"y": 403, "x": 765}, "right_eyebrow_left_corner": {"y": 188, "x": 702}, "nose_right": {"y": 312, "x": 715}, "nose_tip": {"y": 299, "x": 681}, "contour_right5": {"y": 351, "x": 794}, "nose_contour_lower_middle": {"y": 324, "x": 682}, "left_eyebrow_lower_left_quarter": {"y": 194, "x": 586}, "mouth_lower_lip_left_contour3": {"y": 386, "x": 664}, "right_eye_right_corner": {"y": 230, "x": 770}, "right_eye_lower_right_quarter": {"y": 237, "x": 759}, "mouth_upper_lip_right_contour2": {"y": 363, "x": 709}, "right_eyebrow_lower_right_quarter": {"y": 183, "x": 765}, "left_eye_left_corner": {"y": 235, "x": 585}, "mouth_right_corner": {"y": 371, "x": 724}, "mouth_upper_lip_right_contour3": {"y": 369, "x": 702}, "right_eye_lower_left_quarter": {"y": 240, "x": 727}, "left_eyebrow_right_corner": {"y": 192, "x": 651}, "left_eyebrow_lower_right_quarter": {"y": 196, "x": 629}, "right_eye_center": {"y": 232, "x": 742}, "nose_left": {"y": 315, "x": 647}, "mouth_lower_lip_left_contour1": {"y": 373, "x": 659}, "left_eye_upper_right_quarter": {"y": 226, "x": 630}, "right_eyebrow_lower_middle": {"y": 182, "x": 744}, "left_eye_top": {"y": 222, "x": 613}, "left_eye_center": {"y": 235, "x": 613}, "contour_left8": {"y": 432, "x": 621}, "contour_right9": {"y": 445, "x": 719}, "right_eye_left_corner": {"y": 237, "x": 712}, "mouth_lower_lip_bottom": {"y": 387, "x": 682}, "left_eyebrow_upper_left_quarter": {"y": 181, "x": 584}, "left_eye_pupil": {"y": 232, "x": 619}, "right_eyebrow_upper_left_quarter": {"y": 173, "x": 719}, "contour_right8": {"y": 425, "x": 744}, "right_eyebrow_right_corner": {"y": 187, "x": 786}, "right_eye_upper_left_quarter": {"y": 225, "x": 724}, "left_eyebrow_upper_middle": {"y": 180, "x": 607}, "right_eyebrow_upper_right_quarter": {"y": 172, "x": 767}, "nose_contour_left1": {"y": 239, "x": 661}, "nose_contour_left2": {"y": 292, "x": 655}, "mouth_upper_lip_right_contour1": {"y": 358, "x": 692}, "nose_contour_right1": {"y": 238, "x": 697}, "nose_contour_right2": {"y": 290, "x": 706}, "mouth_lower_lip_left_contour2": {"y": 382, "x": 649}, "contour_right6": {"y": 378, "x": 782}, "nose_contour_right3": {"y": 320, "x": 700}, "nose_contour_left3": {"y": 321, "x": 664}, "left_eye_right_corner": {"y": 239, "x": 643}, "left_eyebrow_upper_right_quarter": {"y": 182, "x": 630}, "right_eye_upper_right_quarter": {"y": 223, "x": 757}, "mouth_upper_lip_bottom": {"y": 371, "x": 682}}, "attributes": {"emotion": {"sadness": 2.22, "neutral": 88.815, "disgust": 0.081, "anger": 0.081, "surprise": 8.246, "fear": 0.475, "happiness": 0.081}, "beauty": {"female_score": 83.897, "male_score": 81.629}, "gender": {"value": "Female"}, "age": {"value": 23}, "mouthstatus": {"close": 80.669, "surgical_mask_or_respirator": 0.0, "open": 19.331, "other_occlusion": 0.0}, "glass": {"value": "None"}, "skinstatus": {"dark_circle": 7.112, "stain": 4.466, "acne": 0.769, "health": 82.282}, "headpose": {"yaw_angle": -1.7968067, "pitch_angle": 1.5823805, "roll_angle": 0.29426557}, "blur": {"blurness": {"threshold": 50.0, "value": 0.822}, "motionblur": {"threshold": 50.0, "value": 0.822}, "gaussianblur": {"threshold": 50.0, "value": 0.822}}, "smile": {"threshold": 50.0, "value": 0.001}, "eyestatus": {"left_eye_status": {"normal_glass_eye_open": 0.192, "no_glass_eye_close": 0.0, "occlusion": 0.001, "no_glass_eye_open": 99.807, "normal_glass_eye_close": 0.0, "dark_glasses": 0.0}, "right_eye_status": {"normal_glass_eye_open": 0.112, "no_glass_eye_close": 0.0, "occlusion": 0.005, "no_glass_eye_open": 99.882, "normal_glass_eye_close": 0.0, "dark_glasses": 0.002}}, "facequality": {"threshold": 70.1, "value": 93.684}, "ethnicity": {"value": ""}, "eyegaze": {"right_eye_gaze": {"position_x_coordinate": 0.509, "vector_z_component": 0.997, "vector_x_component": 0.025, "vector_y_component": 0.079, "position_y_coordinate": 0.429}, "left_eye_gaze": {"position_x_coordinate": 0.533, "vector_z_component": 0.985, "vector_x_component": 0.174, "vector_y_component": 0.019, "position_y_coordinate": 0.432}}}, "face_rectangle": {"width": 283, "top": 170, "left": 534, "height": 283}, "face_token": "870d8c2f6d576f0118a1ec468d22caeb"}], "image_id": "It6XAUdpehC1X7GLWxvQaA==", "request_id": "1577201638,2d671729-2fab-4b70-b8a1-5155daceef55", "face_num": 1}
```
#### 选择百度云的原因：
- 百度人脸检测API算法在最权威的公开评测比赛中排名世界领先，也有着很高的准确率，而且使用更加方便，对图片要求跟低，更有利于普通人，而且access_token的有效期为30天，更加有利（Face++只有7天）；
- 通过二者之间的使用对比，发现百度的输出值只是输出默认部分，需要自己添加需要的检测点，而Face++这输出全部数据，对于本产品而已，人脸检测需要用到的值只有角度朝向，所以使用百度更加方便。
#### 价格（性价比）对比
##### 百度价格
- ![百度11](https://github.com/Hinata013/api/blob/master/baidu1.png)
##### face++价格
- ![阿里](https://github.com/Hinata013/api/blob/master/face.png)

按量计费时，人脸识别API组（除人脸稠密关键点API）整组保障10QPS，开通企业认证后可翻倍至20QPS。
### 百度拉伸图像恢复API暂时找不到其他竞品API


## 使用后风险报告 
### 百度人像分割API输出限制及其他问题:
- 返回的二值图像需要进行二次处理才可查看分割效果
- 对输入图片质量要求较高，对清晰度有一定要求；
- 最短边至少50px，最长边最大4096px；
- 要求base64编码和urlencode后大小不超过4M。
#### 价格
- ![baidu](https://github.com/Hinata013/api/blob/master/baidu3.png)
- ![百度222](https://github.com/Hinata013/api/blob/master/baidu4.png)
### 百度人脸检测API输出限制及其他问题：
- 准确率达到99.99%，对用户体验的负面影响不会压过正面影响的机率；
- access_token的有效期为30天，切记需要每30天进行定期更换，或者每次请求都拉取新token；
- 请求的图片需经过Base64编码，图片的base64编码指将图片数据编码成一串字符串，使用该字符串代替图像地址。需要注意图片的base64编码是不包含图片头，如data:image/jpg;base64；
- face_field参数，默认只返回人脸框、概率和旋转角度
- 不支持GIF图片；
- 竞争对手较多，如FACE++,腾讯云，Azure，阿里云
#### 价格
- ![baid2](https://github.com/Hinata013/api/blob/master/baidu1.png)
### 百度拉伸图像恢复API：
- 请求图片需经过base64编码；
- base64编码后大小不超过4M，最短边至少64px，最长边最大4096px，长宽比3:1以内；
- 属于新的API项目，暂无竞争对手，越来越多的工作对图片的规格，规范性有很高的要求，恢复拉伸的前景加优良；
- 新产品暂无合作项目，对比不明显。
#### 价格
- 每个账户一次性共3000次免费使用机会
- 0<月调用量<=300	 时8万元1000次
- 300<月调用量 时4.8万元1000次
### 使用情况
- 通过百度搜索，bing，搜狗搜索发现，百度API相比于其他竞品应用更加规范，而且提供了更加详细的使用教程，具更加广泛的市场。
## 加分项
- 使用了百度人脸检测API，人像分割API，拉伸图像恢复API









