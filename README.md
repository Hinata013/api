# 产品需求
|  发布时间  | 2019年12月5日  |
|  ----  | ----  |
| 产品名称  | 在线证件照图片制作APP |
| 完成进度  | 完成核心价值主张部分与原型设计 |
| 文件主人  | 林泽伟 |
| 设计师  | 林泽伟 |
| 开发者  | 林泽伟 |

# 背景
- 在过去电子产品不发达的时期，只需要用到实体的证件照，去到实体店拍摄裁剪，而现在信息发达，越来越多的线上资料需要用到电子图片形式的证件照，这时，在线上在线制作证件照图片的需求也就不断增加，人工智能API的发展，给我们提供了更多方便的渠道，方便快捷的去在线上制作证件照图片。





# 核心价值主张
## 加值宣言
使证件照图片制作简单便捷，规范。
- 在拍照时通过百度的人脸检测API中的人脸关键点检测功能，可以检测人脸旋转角度，帮助用户拍出更加符合规范的正面照片；
- 拍照结束后，通过百度人像分割API，识别人体的轮廓范围，取得透明背景的人像图，取最重要的部分；
- 结束背景与人像分离后，通过百度拉伸图像恢复API，在用户截取完合适大小的人像后，自动识别过度拉伸的图像，将图像内容恢复成正常比例，使证件照图片更加规范。

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
|  需求  | API |
|  ----  | ----  |
| 使拍出来的人像处于正面，更加符合规范  | 百度人脸检测API |
| 分割人像与背景 | 百度人像分割API |
| 自动识别过度拉伸的图像，将图像内容恢复成正常比例，使证件照图片更加规范  | 百度拉伸图像恢复API |

# 原型
## 交互及界面
- ![首页](https://github.com/Hinata013/api/blob/master/11.png)
- ![一页](https://github.com/Hinata013/api/blob/master/22.png)
- ![二页](https://github.com/Hinata013/api/blob/master/3.png)
- ![三页](https://github.com/Hinata013/api/blob/master/4.png)
- ![四页](https://github.com/Hinata013/api/blob/master/5.png)
- ![五页](https://github.com/Hinata013/api/blob/master/6.png)
- ![六页](https://github.com/Hinata013/api/blob/master/7.png)






