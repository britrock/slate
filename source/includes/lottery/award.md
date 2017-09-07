## 彩票开奖：lottery-award

返回当天及昨天所有开奖结果

### 请求URI

`GET/POST http://{domain}/api/lottery/award`

###  请求参数

参数 | 默认值 | 描述
--------- | ------- | ----------- 

```json
{
  "code": 200,
  "data": [
    {
      "code": "dlt", //彩票代码
      "issueNumber": "2017104",//彩票期号
      "name": "超级大乐透",//彩票名称
      "openCode": "09,11,22,27,30+09,11",//开奖号码
      "openTime": 1504701200000 //时间截
    },
    {
      "code": "fc3d",
      "issueNumber": "2017242",
      "name": "福彩3d",
      "openCode": "2,3,7",
      "openTime": 1504704000000
    }
  ],
  "msg": null
}
```