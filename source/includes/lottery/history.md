##  彩票历史开奖：lottery-history

返回历史开奖号码

### 请求URI

`POST http://{domain}/api/lottery/history/{lotteryCode}-{issueNumber}`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
lotteryCode| - | String | 是 | 彩票代码
 issueNumber| - | int | 是 | 查询期数（30,50,100）
 
```json
{
    "code": 200,                                 //状态码
    "data": [
        {
            "issueNumber": 17000,               //期号
            "openCode": [[7,10,6,1,2,5],[1]],   //开奖号码
                                                //1、双色球、大乐透：[[红球数字],[蓝球数字]] ；
                                                //2、七星彩、重庆时时彩、福彩3d[[各个位数的中奖号码]]
                                                //3、七乐彩：[[7个30内的数字]];
            "openTime": 1506312030148         //开奖时间，时间戳
        },
        {
            "issueNumber": 17001,
            "openCode": [[7,10,6,1,2,5],[1]],
            "openTime": 1506312030148
        }
    ]
}
```
