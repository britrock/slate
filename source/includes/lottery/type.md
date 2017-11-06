## 彩票类型列表：lottery-type

返回可用彩票类型列表

### 请求URI

`GET/POST http://{domain}/api/lottery/type`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
 
```json
{
    "code": 200,    //状态码
    "data": [
            {
                "isSale": 1,                    //是否在售，0：暂停销售；1:在售
                "isHot": 1,                     //是否热门，0：不是热门；1：热门彩种
                "isHigh":1,                     //是否高频彩，0：不是高频彩；1：是高频彩
                "isLocal":0,                    //是否是地方彩，0：不是地方彩；1：是地方彩
                "description": "Hmp Bwcwcaab Suuvtkyt",//描述信息
                "lotteryCode": "fc3d",          //彩票代码
                "lotteryName": "福彩3D"         //彩票名称
            },
            {
                "isSale": 0,
                "isHot":0,
                "isHigh":0,
                "isLocal":1,
                "description": "Lrlyki Mxxpavlxql Bqdj Pnzkfkm Wde",
                "lotteryCode": "fc3d",
                "lotteryName": ""
            }
        ]

}
```