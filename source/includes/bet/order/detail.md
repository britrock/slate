##  我的订单详细：bet-order-detail

返回订单详细内容

### 请求URI

`POST http://{domain}/api/bet/order/detail`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token| - | String | 是 | 令牌
orderId| - | String | 是 | 订单id

```json
{
    "code": 200,                                 //状态码
    "data": [
            {
                "betNumber":[[1,3,5,7,2,13,14],[12,11]],     //投注号码
                "playType":0,                        //玩法类型，0：直选；1：组三；2：组六
                "isSingle":1,                           //是否是复式投注，0：复式，1：单式
                "status":0,                                //是否中奖，0：未中奖，1：已中奖，2：等待开奖，3：失效
                "winMoney":0.00,                           //中奖金额，默认为0
                "level":1                                  //中奖级别，1：一等奖；2：二等奖；以此类推
            },
            {
                "betNumber":[[1,3,5,7,2,13],[12]],    
                 "playType":0,  
                "isSingle":0,                        
                "status":1,                                
                "winMoney":4.00,       
                "level":2                    
            }
        ]
      
}
```
