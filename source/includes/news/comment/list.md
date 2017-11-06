##  资讯评论列表：news-comment-list

返回资讯评论列表信息

### 请求URI

`POST http://{domain}/api/news/comment/list/{newsId}-{page}-{size}`

### 请求参数
参数 | 默认值 | 类型 | 是否必填 | 描述 
--------- | ------- | --------- | ------- | ----------- 
 newsId| - |  int | 是 | 资讯id
 page| - |  int  | 是 | 页码
 size| - |  int  | 是 | 每页数量

```json
{
    "code": 200,
    "data": [
            {
                "photoUrl": "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2261085032,115920914&fm=27&gp=0.jpg",
                                               //头像地址
                "userName": "路人乙",          //用户名称
                "commentId": 1,               //评论id
                "likeCount": 0,               //点赞数
                "content": "Xie Ofhe Xkqzrzx",//评论内容
                "userId": 1,                  //用户id
                "publishTime": 1506389544600  //发表时间
            },
            {
                "photoUrl": "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2261085032,115920914&fm=27&gp=0.jpg",
                "userName": "\u8def\u4eba\u4e59",
                "commentId": 2,
                "likeCount": 1,
                "content": "Ykeipltmm Dqumblxxv Rakd Fshiwp",
                "userId": 2,
                "publishTime": 1506389544600
            }
        ]
}
```
