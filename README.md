<div align="center">
<br/>
  <h1 align="center">
    Waiter-Security
  </h1>
  <h4 align="center">
    一款基础权限系统
  </h4> 




<p align="center">
    <a href="#">
        <img src="https://img.shields.io/badge/java-1.8-green.svg" alt="java Version">
    </a>
    <a href="#">
        <img src="https://img.shields.io/badge/SpringBoot-2.4.0-red.svg" alt="SpringBoot Version">
    </a>
    <a href="#">
        <img src="https://img.shields.io/badge/Mybatis Plus-3.4.1-blue.svg" alt="Swagger Version">
    </a> 
    <a href="#">
        <img src="https://img.shields.io/badge/hutool-5.3.3-orange.svg" alt="Swagger Version">
    </a> 
     <a href="#">
        <img src="https://img.shields.io/badge/kaptcha-0.0.9-blueviolet.svg" alt="Swagger Version">
    </a> 
</p>




#### 项目简介

一个基于 Spring Boot 2.4.0 、 Mybatis-plus、 JWT、Spring Security、Redis、Vue的前后端分离的基础权限系统[项目截图](#jump)



#### 项目源码

|        | 后端源码                                                    | 前端源码                                                |
| ------ | ----------------------------------------------------------- | ------------------------------------------------------- |
| github | https://github.com/waiterxiaoyy/waiter-sercurity-java-admin | https://github.com/waiterxiaoyy/waiter-security-vue-web |
| 码云   | https://gitee.com/waiterxiaoyy/waiter-security-vue-admin    | https://gitee.com/waiterxiaoyy/waiter-security-vue-web  |

#### 主要特性

- 使用最新技术栈，社区资源丰富
- 支持接口级别的功能权限与数据权限，可自定义操作
- 前后端统一异常拦截处理，统一输出异常，避免繁琐的判断
- 完善的登录逻辑、授权逻辑、用户管理、菜单管理、角色管理，可作为后台管理系统的基础模块

####  系统功能

- 用户管理：获取用户表单，为用户分配角色，新增用户后，默认密码为888888
- 角色管理：对权限与菜单进行分配
- 菜单管理：已实现菜单动态路由
- 登录鉴权：使用

#### 项目结构

```
|-- 后端项目
    |-- java
    |   |-- com
    |       |-- waiterxiaoyy
    |           |-- common // 公共组件
    |           |   |-- dto
    |           |   |-- exception // 统一异常处理
    |           |   |-- lang // 定义统一数据格式
    |           |-- config // 配置类
    |           |-- controller // 控制器
    |           |-- entity // 实体类
    |           |-- mapper
    |           |-- security // 安全处理，包括jwt鉴定，权限处理，拦截器
    |           |-- service // 业务处理层
    |           |-- utils // 工具类
    |-- resources
        |-- application.yml // 全局配置
        |-- mapper
```

```
|-- 前端项目
    |-- package-lock.json
    |-- package.json
    |-- vue.config.js
    |-- src
        |-- App.vue
        |-- axios.js // 统一request设置
        |-- globalFun.js // 全局方法
        |-- main.js
        |-- mock.js // 前端假数据
        |-- settings.js
        |-- assets
        |   |-- logo.png
        |   |-- css
        |   |-- icons
        |   |-- img
        |-- components
        |   |-- common // header、bar等处理，已实现标签页
        |   |-- page
        |   |-- SvgIcon
        |   |-- user
        |-- router // 已实现动态路由
        |-- store
        |-- utils
        |-- views // 页面存放
```



#### 项目启动

| 前端项目                                | 后端项目                                                     |
| --------------------------------------- | ------------------------------------------------------------ |
| git clone项目到本地                     | git clone项目到本地                                          |
| 使用idea或者vscode打开项目              | 使用idea打开项目                                             |
| 打开终端，执行：npm install             | 执行maven引入，在数据库管理平台引入数据库vueadmin，启动redis |
| install完成后，执行：npm run dev        | 在application.yml中修改数据库账号和密码                      |
| 启动成功后，访问：http://localhost:8080 | 启动项目，接口前缀：http://localhost:8081                    |

> **注意：后台项目需要引入redis、Lombok插件**
>
> 
>
> 这里提供一些基础教程供刚入门的同学
>
> 1、JDK：1.8+ 
> 安装教程：https://www.runoob.com/java/java-environment-setup.html
> 2、Redis 3.0+
> 安装教程：https://www.runoob.com/redis/redis-install.html
> 3、Maven 3.0+
> 安装教程：https://www.runoob.com/maven/maven-setup.html
> 4、MYSQL 5.7
> 安装教程：https://www.runoob.com/mysql/mysql-install.html
> 5、Node v10+ (最好使用 12，高版本可能会有问题)
> 安装教程：https://www.runoob.com/nodejs/nodejs-install-setup.html



#### 项目截图

<span id="jump">部分截图</span>

| ![](https://blog20211013.oss-cn-shenzhen.aliyuncs.com/blog/picture-waiter-admin/login.jpg?versionId=CAEQMxiBgMCllqPx8xciIDNkODM2NjcwMjgzNzRjZTQ5MGRhMGZkOTczYzQ4YTkz) | ![](https://blog20211013.oss-cn-shenzhen.aliyuncs.com/blog/picture-waiter-admin/dashborad.jpg?versionId=CAEQMxiBgIDElaPx8xciIDZkMDk5MTQ3Mzk3YzQwNzViOWFjOTg4MzgwMDhlMTQ1) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](https://blog20211013.oss-cn-shenzhen.aliyuncs.com/blog/picture-waiter-admin/user1.jpg?versionId=CAEQMxiBgMCdlKPx8xciIDVmYzcyNWMxZWNjMjQzMTlhMGM3MDczZTU3MjYxODRk) | ![](https://blog20211013.oss-cn-shenzhen.aliyuncs.com/blog/picture-waiter-admin/user2.jpg?versionId=CAEQMxiBgMCsk6Px8xciIDE5NzU4Y2E4ZGVlYzRhZGM4ZTM3ODc3NWI5MmFhZjJk) |
| ![](https://blog20211013.oss-cn-shenzhen.aliyuncs.com/blog/picture-waiter-admin/role.jpg?versionId=CAEQMxiBgMDClKPx8xciIDdmNjA2NDQyMjMzMDQ0MTBiNThlNzlhNWNkNzc5MzUw) | ![](https://blog20211013.oss-cn-shenzhen.aliyuncs.com/blog/picture-waiter-admin/role1.jpg?versionId=CAEQMxiBgIDVk6Px8xciIGM3MjMwMjE3ZGJkNDQ5MGE5NmExMzMxYWZjZGRkMDg5) |
| ![](https://blog20211013.oss-cn-shenzhen.aliyuncs.com/blog/picture-waiter-admin/menu.jpg?versionId=CAEQMxiBgMC4laPx8xciIDk0MzM2MmMzYzA2NTRiNzZhOGQxZmJmYWQxMjQxNWVh) | ![](https://blog20211013.oss-cn-shenzhen.aliyuncs.com/blog/picture-waiter-admin/menu2.jpg?versionId=CAEQMxiBgMD8lKPx8xciIDlhNDA2MzU1YWQ3NDQzYWE4NmM3NzY2MTU4NTFiZmE2) |



#### 项目捐赠

|                             微信                             |                            支付宝                            |
| :----------------------------------------------------------: | :----------------------------------------------------------: |
| ![](https://blog20211013.oss-cn-shenzhen.aliyuncs.com/blog/wechatpay.png?versionId=CAEQMxiBgMDgnq_x8xciIGYwYmZhMmM0N2U0ZTRjYzBiMmJhNzhjMzJlYThiMDQ3) | ![](https://blog20211013.oss-cn-shenzhen.aliyuncs.com/blog/alipay.jpg?versionId=CAEQMxiBgIC5nq_x8xciIGZjY2ExOWE4N2E0NDRmYmZhMTI5ZmVhZDQ2ZGNiMDgx) |

