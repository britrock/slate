##  我的帐户明细：member-bill

返回帐户明细列表

### 请求URI

`POST http://{domain}/api/bill/list`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token | - | String | Y | 令牌
page | - | Int | Y | 第几页
 
```json
{
    "code": 200, //状态码
    "data": [
        {
            "gmtCreate": 1508728401000, //明细时间
            "id": 120,// 明细ID
            "money": 2,//金额
            "title": "双色球",// 明细标题
            "type": 2, // 记录类型，0：充值；1：中奖；2：购彩
            "lotteryCode":"ssq"       //彩票代码
        }
    ],
    "msg": null,
    "page": {
        "draw": 0,// 无用
        "offset": 0, // 无用
        "page": 1, // 当前页
        "pages": 1,// 总页数
        "size": 10, // 页大小
        "total": 1 // 总记录数
    }
}
```
