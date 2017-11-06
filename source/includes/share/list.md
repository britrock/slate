##  天天分钱方案列表：share-list

返回天天分钱方案列表

### 请求URI

`POST http://{domain}/api/share/list`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token| - | String | 是 | 会话id
page| - | int | 是 | 页码
size | - | int | 是 | 每页记录数

```json
{
    "code": 200,                                 //状态码
    "data": {
          "totalBonus":123.00,          //用户活动累积奖金
          "planList":[
                    {
                        "planId":"2017101000000006",  //方案id（订单id）
                        "planTime":15230403240,   //方案日期，时间戳
                        "lotteryCode":"dlt",      //彩票代码
                        "lotteryName":"大乐透",    //彩票名称
                        "betMoney":2.00,           //方案投注金额
                        "betWinMoney":10.00,      //方案中奖金额
                        "openTime":1523212331,    //开奖时间，时间戳
                        "status":0,                //方案状态，0：未参与，1：等待参与，2：等待分钱，3：待领取，4：已领取
                        "bonus":0.01            //我的奖金
                    },
                     {
                          "planId":"2017101000000006", 
                         "planTime":15230403240,   //方案日期，时间戳
                         "lotteryCode":"ssq",      //彩票代码
                         "lotteryName":"双色球",    //彩票名称
                         "betMoney":2.00,           //方案投注金额
                         "betWinMoney":10.00,      //方案中奖金额
                         "openTime":1523212331,    //开奖时间，时间戳
                         "status":0,                //方案状态，0：未参与，1：等待参与，2：等待分钱，3：待领取，4：已领取
                         "bonus":0.01            //我的奖金
                            }
                ]
    },
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
