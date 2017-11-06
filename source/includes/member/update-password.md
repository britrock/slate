##  会员修改密码：member-update-password

返回会员信息

### 请求URI

`GET/POST http://{domain}/api/member/password/update`

### 请求参数
参数 | 类型 | 必填 |默认值 | 描述
--------- | ------- | ------- | ------- | -----------
oldPassword  | string | Y | - | 旧密码  
newPassword  | string | Y | - | 新密码  
token  | string | Y | - | 令牌，从短信验证码验证返回的data获取  

```json
{
    "code": 200, // 非200表示错误
    "msg": "Success!" // 省 
 }
```
