##  会员注册：member-register

返回会员信息

### 请求URI

`POST http://{domain}/api/member/register`

### 请求参数
参数 | 默认值 | 类型 | 必填 | 描述
--------- | ------- | ------- | ------- | -----------
mobile  | - | String | 是 | 手机号  
code  | - |  String | 是 | 验证码，如果是手机注册需要  
password  | - |  String | 是 | 密码，只允许英文和数字 
osType  | - |  String | 是 | 手机类型，iOS/ANDROID

```json
{
    "code": 200, //非200表示错误
    "data": {
            "id": 103, // 用户ID
            "nickname": "wx00000000103",// 昵称
            "imageUrl": "",// 头像
            "money": "", // 余额,
            "token": "CWkHzABxohXl24zcSv4wiVm2XWPze20f" // 令牌
        }
}
```
