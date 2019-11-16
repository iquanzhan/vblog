# vblog：分布式个人博客管理系统

## 一、目的
​		本项目旨在总结前后端分离常用技术点，形成集前端+后端+小程序+移动端一整套的个人技术博客解决方案。技术采用主流前后端分离微服务架构，并涵盖持续集成及自动化部署的相关解决方案。既然是以学习为目的，可能并不是以做成一个博客系统为最终目标，可能会基于此基础之上进行技术的扩充。

​		技术方面，后端采用Java技术栈，前端使用工程化的SPA单体应用实现。项目计划分为两个版本分别为vue+Spring Cloud、react+Dubbo。除了还该常用的增删改查业务之外，也会涉及高并发、限流、支付、爬虫等主流流行技术点。

​		业务方面分为后台+前台场景，后台管理系统负责对整个网站进行管理，前台为展示个人博客内容。除了实现博客的常用功能外，也希望加入秒杀、分布式搜索、区块链等功能。

​		本人才疏学浅，可能有些观点不是很成熟，考虑的没有很全面，望大家积极指正。也希望可以结识更多热爱技术的朋友，一起加油，一起进步。

![image-20191116142651832](assets/image-20191116142651832.png)

## 二、主要技术：
所用到的主要技术点：

![image-20191116152652573](assets/image-20191116152652573.png)

### 2.1 后端

数据库：MySql

数据访问层：Mybatis、Spring Data Jpa

NoSql：Redis、MongoDB

持续集成：docker、k8s

分布式搜索：ElasticSearch

消息队列：RabbitMQ、ActiveMQ

版本控制：git

依赖管理：maven

分布式：Spring Boot、Spring Cloud、Dubbo、Spring Cloud Alibaba

其他：Quartz、FFmpeg、Spring、maven、SSO、WebMagic、Netty等

### 2.2 前端
前端框架：Vue、React、Ant Design、Element UI

网络请求：axios、Fetch

表格图表：ECharts

数据状态管理：redux、vuex

路由管理：react-router、vue-router

小程序：mpvue

代码检查工具：ESLint

代码打包工具：webpack

## 三、主要功能
1.登录注册：实现对用户名、手机号及扫码的登录实现，实现单点登陆功能。

2.文章模块:对文章进行管理

3.分类目录：对分类目录进行管理

4.文章标签模块

5.作品管理：可添加自己的作品

6.友情链接管理

7.页面管理

8.评论管理

9.菜单管理

10.用户管理

11.网站seo设置

12.媒体资源管理：fastdfs

13.网站爬虫设计：可以抓取指定的数据到个人博客中

14.课程管理：可以发布自己的视频等课程资源，实现收费及免费功能。包括支付

15.统计模块：统计网站访问量、评论量、等信息记录网站的历程

16.搜索：分布式搜索实现对文章的搜索功能。

17.活动与招聘信息

18.吐槽与问答

19.网站数据备份与导入导出

20.数据字典管理

...

## 四、项目汇总

目前主流的技术架构采用前后端分离技术实现，在项目工程上来讲，也应是分离的项目。每个项目进行单独开发。下面是本项目中所有的工程目录。

### 4.1 版本一：

Java采用Spring Boot + Spring Cloud + Spring Data JPA  技术栈

后端项目地址：https://github.com/iquanzhan/vblog-spring-cloud

前端采用react技术栈

前端项目地址：https://github.com/iquanzhan/vblog-web-react

### 4.2 版本二：

Java采用Spring Boot + Dubbo + MyBatis 技术栈

后端项目地址：https://github.com/iquanzhan/vblog-dubbo

前端采用vue技术栈

前端项目地址：https://github.com/iquanzhan/vblog-web-vue



使用nginx+docker+k8s进行持续集成与发布管理。









