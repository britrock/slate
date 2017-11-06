##  资讯列表：news-list

返回资讯列表信息

### 请求URI

`POST http://{domain}/api/news/list/{newsType}-{page}-{size}`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
 newsType| - | String | 是 | 资讯类别(tt:头条，ssq:双色球),-1时返回全部
 page| - | int | 是 | 页码
 size| - | int | 是 |  每页数量

```json
{
    "code": 200,
    "data": {
            "topNews":{                                               //头条资讯内容
                        "imageUrl": "www.baidu.com",          //资讯图片url
                       "content": "主队贝西克上轮首战做客3:1,战胜波尔图，球队与波尔图、莱比锡、摩纳哥同组",  
                                                               //正文内容
                       "publishTime": 1506388007998,           //发表时间
                       "title": "冷门直击：莱比锡不宜追捧 多特主场不惧皇马"   //资讯标题
            },
            "newsList":[{
                "id": 1,                              //资讯id
                "title": "Ymeifdux Duwl Lxg Hkqkkn",  //资讯标题
                "isHot": 0,                           //是否火爆资讯，1:是；0:不是
                "publishTime": 1506388880579          //发表时间
            },
            {
                "id": 2,
                "title": "Bbvd Yteuflz Qkjvjit Uveecu Btuilyc",
                "isHot": 1,
                "publishTime": 1506388880579
            }]
       },
        "page": {
                "draw": 0,
                "offset": 0,
                "page": 1,
                "pages": 1,
                "size": 10,
                "total": 3
            }
}
```
