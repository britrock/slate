##  会员手机绑定：member-bind-mobile

返回结果

### 请求URI

`GET/POST http://{domain}/api/member/mobile/bind`

### 请求参数
参数 | 类型 | 必填 |默认值 | 描述
--------- | ------- | ------- | ------- | -----------
mobile  | string | Y | - | 手机号  
code  | string | Y | - | 验证码  
token  | string | Y | - | 令牌，从短信验证码验证返回的data获取  

```json
{
    "code": 200, // 非200表示错误
    "msg": "Success!" // 消息
 }
```
