##  走势图

> 返回彩票最近开奖历史记录

### 请求URI

`GET/POST http://{domain}/api/lottery/trend/{code}`

### 请求参数
参数 | 默认值 | 描述
--------- | ------- | -----------
 code| '' |  彩票代码

```json
{
  "code": 200,
  "data": [
    {
      "code": "ssq",//彩票代码
      "issueNumber": "2017104",//开奖期号
      "name": "",//彩票名称
      "openCode": "01,14,15,20,23,30+14",//开奖号码
      "openTime": 1504617500000 //开奖时间
    },
    {
      "code": "ssq",
      "issueNumber": "2017103",
      "name": "",
      "openCode": "01,21,23,25,31,33+01",
      "openTime": 1504444700000
    }
   ]
}
```
