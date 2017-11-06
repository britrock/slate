##  我的订单新增订单：bet-order-save

返回新增订单结果

### 请求URI

`POST http://{domain}/api/bet/order/save`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token| - | String | 是 | 令牌
orderId| - | String | 是 | 订单id
lotteryType| - | int | 是 | 投注彩票类型，1：彩票；2：足球；3：篮球
lotteryCode| - | String | 是 | 彩票代码
issueNumber| - | String | 是 | 投注期号
betNums| - | int | 是 | 投注注数
betMultiple| - | int | 是 | 投注倍数                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             
betMoney| - | decimal | 是 | 投注总金额
payTime| - | String | 是 | 付款时间
pursueIssue| - | int | 是 | 追投期数
betNumList| - | List | 是 | 投注号码列表

```json
{
    "betNumList":[
         {
            "betNumber":"1,2,3,4,5,6,7+3",  //投注号码
            "playType":0,               //玩法类型，0：直选；1：组三；2：组六
            "isSingle":1,                   //是否是单式投注，0：复式；1：单式
            "betMoney": 24.00               //金额
         },
         {
          "betNumber":"1,2,3,4,5,6+3",  
           "playType":0,  
          "isSingle":0,   
          "betMoney": 24.00       
         }
    ] 
 }
```


```json
{
    "code": 200,                                 //状态码
    "msg":"成功"//更新结果，成功、失败
}
```
