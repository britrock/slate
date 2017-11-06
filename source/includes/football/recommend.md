##  足彩推荐投注：football-recommend

返回推荐投注信息

### 请求URI

`POST http://{domain}/api/football/recommend`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 


```json
{
    "code": 200,
    "data": {
            "leagueName": "意甲",       //联赛名称
            "winOdds": 5.72,            //主队胜的赔率
            "winOddsId": 272,           //主队胜的id
            "matchId": 42,              //比赛id
            "lostOddsId": 42,           //主队负的id
            "guestName": "桑普",        //客队名称
            "hostImgUrl": "https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=1340925344,145113786&fm=27&gp=0.jpg",
                                        //主队图标url
            "guestImgUrl": "https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=1340925344,145113786&fm=27&gp=0.jpg",
                                        //客队图标url
            "hostName": "拉齐奥",        //主队名称
            "lostOdds": 4.33,           //主队负的赔率
            "tieOdds": 8.117,           //平的赔率
            "tieOddsId": 107,           //平的id
            "matchTime": 1506392332094  //比赛时间
        }
}
```
