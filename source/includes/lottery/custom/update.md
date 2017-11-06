## 定制更新：lottery-custom-update

返回更新结果

### 请求URI

`GET/POST http://{domain}/api/lottery/custom/update`

###  请求参数

参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token| - | String | 是 | 会话id
lotteryCode| - |  String  | 是 | 重新拼接后的定制信息，例："ssq,dlt,cqssc"

```json
{
  "code": 200,
  "msg":"成功"//更新结果，成功、失败
}
```