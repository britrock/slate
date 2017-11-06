##  会员登录：member-login

返回会员信息

### 请求URI

`GET/POST http://{domain}/api/member/login`

### 请求参数

参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
mobile  | 必填 |  | 是 |手机号  
password  | 必填 |  | 是 |密码  
osType  | 必填 |  | 是 |手机系统类型  

```json
{
    "code": 200, // 非200表示错误
    "data": {
            "id": 103, // 用户ID
            "nickname": "wx00000000103",// 昵称
            "imageUrl": "", // 头像,
            "money": "", // 余额,
            "couponNum": 2, // 优惠券数量
            "token": "CWkHzABxohXl24zcSv4wiVm2XWPze20f" // 令牌
        }
}
```
