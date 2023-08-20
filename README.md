# Getting Started

### Reference Documentation

For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.7.14/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/2.7.14/maven-plugin/reference/html/#build-image)
* [Spring Web](https://docs.spring.io/spring-boot/docs/2.7.14/reference/htmlsingle/index.html#web)

### Guides

The following guides illustrate how to use some features concretely:

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/rest/)

# 支付系统探讨
    目前手机支付，网银支付等形式，许多品牌形式众多，用户可能不会在乎使用何种支付方式，或者说不同的用户在支付的时候有不同的支付软件使用偏好
    1.喜欢使用支付宝支付的
    2.喜欢微信支付的
    3.喜欢银联，银行卡App跳转支付的
    本系统目的是让用户无差异化的使用不同的平台，使用统一的入口来进行支付
### 聚合支付主要实现方式为：
    1.线上聚合收银台（通过开放API实现，淘宝等电商系统生成订单后会要求用户选择支付方式，平台集成的支付方式越多就能照顾到更多需求的用户）
    2.线下B2C扫码（线下超市内要求用户出示支付码，然后扫码扣钱，不关心出示的是微信付款码还是支付宝付款码）
    3.线下C2B扫码（商户提供一个统一的收款码，用户通过不同的支付app扫描统一的付款码，会分别跳转到相同的支付界面，进行结算）

### 主要功能及后期功能展望
    1.集成市面上占有率高的支付方式，并且支持后续其他支付方式的加入扩展，形成一个统一的支付入口，通过Saas平台向外提供服务
    2.提供给各商户订单管理，门店管理，财务数据统计等基础功能
    3.通过广告，营销，金融等服务，为平台提供更多的增值服务

# 功能模块
    
# 业务架构
# 技术架构
    本系统使用微服务架构，方便后期扩展，前后端分离实现，由用户层、负载层、服务层、数据管理层