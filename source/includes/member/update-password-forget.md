##  会员忘记密码：member-update-password-forget

返回会员信息

### 请求URI

`GET/POST http://{domain}/api/member/password/update-forget`

### 请求参数
参数 | 类型 | 必填 |默认值 | 描述
--------- | ------- | ------- | ------- | -----------
mobile  | string | Y | - | 手机号  
password  | string | Y | - | 密码  
token  | string | Y | - | 令牌，从短信验证码验证返回的data获取  

```json
{
    "code": 200, // 非200表示错误
    "msg": "Success!" // 省 
 }
```
