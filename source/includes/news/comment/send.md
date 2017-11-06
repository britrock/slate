##  资讯发表评论：news/comment/send

返回发表评论结果信息

### 请求URI

`POST http://{domain}/api/news/comment/send`

### 请求参数
 
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
token| - |  String  | 是 | 会话id
content| - |  String  | 是 |  评论内容
newsId| - |  int | 是 |  资讯id
publishTime| - |  String  | 是 |  发表时间
 

```json
{
    "code": 200,    //状态码
    "msg":"成功"  //发表评论结果：成功、失败
}
```
