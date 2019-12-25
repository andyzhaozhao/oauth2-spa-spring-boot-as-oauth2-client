### 概述
前后端分离架构下的统一认证示例——vue前后端共享后端cookie跨域访问的方式
* authorizationserver: 作为OAuth2 Server。
* spring-boot-spa-oauth2-client: 作为OAuth2 Client，被vue前端跨域访问。
* vue-front-end: 普通vue前端工程。调用接口时候需要设置http header的withCredentials为true，
从而跨域访问时候可以传递cookie给后端。

### 运行
1. 启动vue-front-end(启动方式参考：[vue-front-end的readme](vue-front-end/README.md)）
1. 启动spring-boot-spa-oauth2-client
1. 启动authorizationserver
1. 浏览器访问：http://localhost:9527/

