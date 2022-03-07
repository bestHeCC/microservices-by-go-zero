# 微服务实践 ![Version](https://img.shields.io/badge/version-1.3.0-green.svg)
```
              _                                            _                             __   
   ____ ___  (_)_____________        ________  ______   __(_)_______     _________  ____/ /__ 
  / __ `__ \/ / ___/ ___/ __ \______/ ___/ _ \/ ___/ | / / / ___/ _ \   / ___/ __ \/ __  / _ \
 / / / / / / / /__/ /  / /_/ /_____(__  )  __/ /   | |/ / / /__/  __/  / /__/ /_/ / /_/ /  __/
/_/ /_/ /_/_/\___/_/   \____/     /____/\___/_/    |___/_/\___/\___/   \___/\____/\__,_/\___/ 
                                                                                              
```

### 写在开头  
感谢go-zero作者万老师提供的 `go-zero` 入门学习教程的示例代码  
详细教程:[go-zero实战：让微服务Go起来](https://juejin.cn/post/7036011047391592485)。  

## 项目说明
go-zero配合docker环境快速搭建微服务架构的商城系统，以下各服务均需要在goland容器中启动  
此仓库为具体实现代码  
docker环境部署文件可以[参考此处](https://gitee.com/bestHeCC/microservices.docker)。

## Release Notes

~~~
v1.0.0 (2022-02-16)
* 第一次提交，实现用户服务
* 启动 user rpc 服务
cd mall/service/user/rpc && go run user.go -f etc/user.yaml
* 启动 user api 服务
cd mall/service/user/api && go run user.go -f etc/user.yaml
~~~

~~~
v1.1.0 (2022-02-25)
* 实现商品服务
* 启动 product rpc 服务
cd mall/service/product/rpc && go run product.go -f etc/product.yaml
* 启动 product api 服务
cd mall/service/product/api && go run product.go -f etc/product.yaml
~~~

~~~
v1.2.0 (2022-02-28)
* 实现订单服务
* 启动 order rpc 服务
cd mall/service/order/rpc && go run order.go -f etc/order.yaml
* 启动 order api 服务
cd mall/service/order/api && go run order.go -f etc/order.yaml
~~~

~~~
v1.3.0 (2022-03-07)
* 实现支付服务
* 启动 pay rpc 服务
cd mall/service/pay/rpc && go run pay.go -f etc/pay.yaml
* 启动 pay api 服务
cd mall/service/pay/api && go run pay.go -f etc/pay.yaml
~~~