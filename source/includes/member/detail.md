##  会员基本资料：member-detail

返回会员信息

### 请求URI

`GET/POST http://{domain}/api/member/detail`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token  | - |  String  | 是 |登录令牌  

```json
{
    "code": 200, // 非200表示错误
    "data": {
            "id": 103, // 用户ID
            "nickname": "wx00000000103",// 昵称
            "imageUrl": "",// 头像
            "money": "", // 余额,
            "token": "CWkHzABxohXl24zcSv4wiVm2XWPze20f" // 令牌
        }
}
```
