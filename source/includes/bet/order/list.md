##  我的订单列表：bet-order-list

返回我的订单列表

### 请求URI

`POST http://{domain}/api/bet/order/list`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token| - | String | 是 | 会话id
page| - | int | 是 | 页码
size | - | int | 是 | 每页记录数
status | - | int | 是 | 列表类型，0:未中奖；1：已中奖；2：等待开奖；-1：全部

```json
{
    "code": 200,                                 //状态码
    "data": [
        {
            "orderId":"20170929001",        //订单id
            "code":"ssq",                 //投注彩种彩票代码
            "name":"双色球",               //投注彩种彩票名称
            "issueNumber":"20170929001",  //投注期号
            "betNums":4,                   //投注注数
            "betTimes":6,                 //投注倍数
            "totalAmount":48.00,          //支付总金额
            "status":0,                   //订单状态，0：未中奖；1：已中奖；2：等待开奖
            "payTime":150234231,          //支付时间
            "winMoney":100.00,             //中奖金额
            "openCode":[[1,2,3,4,5,6],[3]]    //开奖号码
        },
        {
            "orderId":"20170929001",
            "code":"dlt",
            "name":"大乐透",
            "issueNumber":"20170929001",
            "betNums":2,
            "betTimes":4,
            "totalAmount":16.00,
            "status":1,
            "payTime":150234231,
            "winMoney":100.00,
             "openCode":[[1,2,3,4,5,6],[3]]    //开奖号码
        }
    ],
    "page": {
            "draw": 0,
            "offset": 0,      //当前查询偏移量
            "page": 1,        //当前页
            "pages": 0,       //总页数
            "size": 10,       //页大小
            "total": 0        //总记录数
        }
}
```
