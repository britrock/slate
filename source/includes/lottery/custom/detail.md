## 定制彩种：lottery-custom-detail

返回用户定制彩种信息

### 请求URI

`GET/POST http://{domain}/api/lottery/custom/detail`

###  请求参数

参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token| - |  String  | 是 | 会话id

```json
{
  "code": 200,
  "data": 
    {
      "lotteryCode":["ssq","dlt","cqssc"]    //获取用户定制彩种内容
    }
}
```