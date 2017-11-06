##  天天分钱免费领取：share-receive

返回天天分钱免费领取结果

### 请求URI

`POST http://{domain}/api/share/receive`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token| - | String | 是 | 令牌
planId| - | String | 是 | 方案id

```json
{
    "code": 200,                                 //状态码
   "msg":"0.01"                                 //领取成功则返回金额，最少0.01，若为0则领取失败
}
```
