
# MJPayApi

使用之前，请先完成微信支付及支付宝支付所需的项目配置

####支付调用

- 微信
```
[[MJPayApi sharedApi]wxPayWithPayParam:data success:^(PayCode code)
{
[self payStatus:code Co_nbr:co_nbr];
} failure:^(PayCode code) {
[self payStatus:code Co_nbr:co_nbr];
}];
```
- 支付宝

```
[[MJPayApi sharedApi]aliPayWithPayParam:data success:^(PayCode code)
{
[self payStatus:code Co_nbr:co_nbr];
} failure:^(PayCode code) {
[self payStatus:code Co_nbr:co_nbr];
}];
```

是不是很简单那~~~

[关于项目的讲解连接](http://www.jianshu.com/p/6105550fe070)

[欢迎关注我的简书博客](http://www.jianshu.com/u/2a2051ad6a5d)
