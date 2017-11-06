##  短信-发送验证码：sms-sendcode

返回发送信息

### 请求URI

`GET/POST http://{domain}/api/sms/sendcode`

### 请求参数
参数 | 默认值 | 描述
--------- | ------- | -----------
mobile  | - | 手机号
osType  | - | 手机系统类型：iOS/Android
deviceId  | - | 手机设备序列ID  

```json
{
    "code": 200,         // 200成功，其它失败
    "msg": "验证码已发送" // 消息s
}
```
