---
title: 114彩票-API文档

language_tabs: # must be one of https://git.io/vQNgJ
  - javascript

toc_footers:
  - <a href='http://test.114.com'>114彩票</a>

includes:
    #公共配置参数
    - common        
    #------------ 彩票 ------------#
    #彩票类型列表
    - lottery/type
    #彩票开奖列表
    - lottery/award
    #彩票走势图
    - lottery/trend
    #售彩页面
    - lottery/sale
    #历史开奖号码
    - lottery/history
    #用户定制信息
    - lottery/custom/detail
    #更新定制信息
    - lottery/custom/update
    #------------ 资讯 ------------#
    #首页轮播图
    - news/banner
    #资讯列表
    - news/list
    #资讯详细
    - news/detail
    #首页通知信息
    - news/notice
    #评论列表
    - news/comment/list
    #发表评论
    - news/comment/send
    #------------ 足彩 ------------#
    #推荐足彩投注
    - football/recommend
    #------------ 订单投注 ------------#
    #新增订单
    - bet/order/save
    #获取订单编号
    - bet/order/number
    #我的订单列表
    - bet/order/list
    #订单详细
    - bet/order/detail
    #支付凭据
    - bet/pay/charge
    #支付验证
    - bet/pay/verify
    #------------ 会员 ------------#
    # 会员登录
    - member/login
    # 会员注销
    - member/logout
    # 会员注册
    - member/register
    # 修改密码
    - member/update-password
    # 忘记密码
    - member/update-password-forget
    # 会员基本资料
    - member/detail
    # 会员是否已登录
    - member/has-login
    # 手机绑定
    - member/bind-mobile
    #------------ 我的 ------------#
    # 帐户明细
    - member/bill
    # 我的优惠券列表
    - coupon/list-member
    #------------ 短信 ------------#
    # 发送验证码
    - sms/sendcode
    # 验证验证码
    - sms/verifycode
    #------------ 天天分钱 ------------#
    # 方案列表
    - share/list
    # 方案详情
    - share/detail
    # 参与方案
    - share/join
    # 领取奖金
    - share/receive
    #------------ 优惠券 ------------#
    # 优惠券列表
    - coupon/list
    # 优惠券领取
    - coupon/get
    #------------反馈------------#
    # 反馈提交
    - more/feedback/save    

    #- errors
    

search: true
---

# 简介：Intro
114彩票API文档

<aside class="notice">
    domain=test.114.com
    配置hosts，C:\Windows\System32\drivers\etc\hosts
</aside>

192.168.2.114       test.114.com

