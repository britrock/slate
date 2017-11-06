##  会员注销：member-logout

返回成功消息

### 请求URI

`GET/POST http://{domain}/api/member/logout`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token  | - |  String  | 是 | 登录令牌  

```json
{
    "code": 200, // 非200表示错误
    "msg": "success"
}
```
