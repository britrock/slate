## 彩票类型：lottery-type

返回可用彩票类型列表

### 请求URI

`GET/POST http://{domain}/api/lottery/type`

###  请求参数

参数 | 默认值 | 描述
--------- | ------- | ----------- 

```json
{
  "code": 200,
  "data": [
    {
      "area": "",//地区
      "code": "dlt",//彩票代码
      "high": false,//是否为高频彩
      "hot": false,//是否热门
      "issuer": "体彩",//发行方
      "name": "超级大乐透",//彩票名称
      "nodes": "每周一、三、六的20:30开奖",//开奖时间
      "series": "",//类型、体彩
      "times": "1"//开奖次数
    },
    {
      "area": "",
      "code": "fc3d",
      "high": false,
      "hot": true,
      "issuer": "福彩",
      "name": "福彩3d",
      "nodes": "每天的21:20开奖",
      "series": "",
      "times": "1"
    }
  ],
  "msg": null
}
```