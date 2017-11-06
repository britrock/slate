##  资讯详细：news-detail

返回资讯详细信息

### 请求URI

`POST http://{domain}/api/news/detail/{newsId}`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
newsId| - |  int  | 是 | 资讯id

```json
{
    "code": 200,                                   //状态码
    "data": {
           "imageUrl": "www.baidu.com",          //资讯图片url
           "content": "主队贝西克上轮首战做客3:1,战胜波尔图，球队与波尔图、莱比锡、摩纳哥同组",  
                                                   //正文内容
           "publishTime": 1506388007998,           //发表时间
           "title": "冷门直击：莱比锡不宜追捧 多特主场不惧皇马"   //资讯标题
       }
}
```
