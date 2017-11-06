##  我的优惠券列表：coupon-list-member

返回优惠券列表

### 请求URI

`POST http://{domain}/api/coupon/list-member`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token | - | String | Y | 令牌
page | - | Int | Y | 第几页
status | - | Int | Y | 状态，0未使用，1使用/过期
 
```json
{
    "code": 200,
    "data": [
        {
            "action": "member", //操作类型，APP使用
            "description": "新用户注册1", //说明
            "endTime": 1513180800000,//结束日期，时间截
            "icon": "http://xxx.com/t.pn",// icon
            "id": 1, // 优惠券ID
            "isGet": 1, // 使用状态，0未使用，1已使用，2已过期
            "money": 10,// 金额
            "name": "新用户注册" // 优惠券名称
        }
    ],
    "msg": null,
    "page": {
        "draw": 0,
        "offset": 0,
        "page": 1,
        "pages": 1,
        "size": 10,
        "total": 3
    }
}
```
