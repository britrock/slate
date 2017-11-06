##  短信-验证验证码：sms-verifycode

返回验证信息

### 请求URI

`GET/POST http://{domain}/api/sms/verifycode`

### 请求参数
参数 | 默认值 | 描述
--------- | ------- | -----------
code  | - | 验证码
osType  | - | 手机系统类型：iOS/Android
deviceId  | - | 手机设备序列ID  

```json
{
    "code": 200,  // 200成功，其它失败
    "msg": "成功",  // 消息
    "data": "35f0827e-1157-442e-bd20-e59a929113f3" // 密钥，用于后续操作时传递参数
}
```
```json
{
    "code": 400,
    "msg": "验证码" // 消息
}
```