---
title: 114彩票 API

language_tabs: # must be one of https://git.io/vQNgJ
  - javascript

toc_footers:
  - <a href='http://test.114.com'>114-lottery</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# 简介
配置host：

```
192.168.2.114   test.114.com
```
# 彩票接口

## 彩票开奖

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let kittens = api.kittens.get();
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

返回当天及昨天所有开奖结果

### 请求URI

`GET/POST http://{domain}/api/lottery/award`

###  请求参数

参数 | 默认值 | 描述
--------- | ------- | -----------
 无|  | 

```javascript
{
  "code": 200,
  "data": [
    {
      "code": "dlt", //彩票代码
      "issueNumber": "2017104",//彩票期号
      "name": "超级大乐透",//彩票名称
      "openCode": "09,11,22,27,30+09,11",//开奖号码
      "openTime": 1504701200000//时间截
    },
    {
      "code": "fc3d",
      "issueNumber": "2017242",
      "name": "福彩3d",
      "openCode": "2,3,7",
      "openTime": 1504704000000
    },
    ...
  ],
  "msg": null
}
```
##  走势图
```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let max = api.kittens.get(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

### 请求URI

`GET/POST http://{domain}/api/lottery/trend/{code}`

### 请求参数
参数 | 默认值 | 描述
--------- | ------- | -----------
 code| '' |  彩票代码

```javascript
{
  "code": 200,
  "data": [
    {
      "code": "ssq",//彩票代码
      "issueNumber": "2017104",//开奖期号
      "name": "",//彩票名称
      "openCode": "01,14,15,20,23,30+14",//开奖号码
      "openTime": 1504617500000//开奖时间
    },
    {
      "code": "ssq",
      "issueNumber": "2017103",
      "name": "",
      "openCode": "01,21,23,25,31,33+01",
      "openTime": 1504444700000
    },
    ...
}
    
```
