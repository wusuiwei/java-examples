Java 学习路线图
----

### 常用工具

- 项目构建工具
    - [Apache Maven](docs/notes/Maven学习笔记.md)
    - Ant
    - Gradle

----

- Java核心
    - Java核心语法
    - Java面向对象核心
    - 集合框架
    - 异常机制
    - Java常用API
    - Java泛型、枚举、注解
    - 反射机制
    - 线程、线程通信
    - 网络编程
    - Java 8 新特性
    - Java9~13新特性
    - 数据结构与算法
    - 设计模式
    - 集成开发环境的使用
- Java与数据库交互（15）
    - SQL与PL/SQL的使用
    - MySQL数据库
    - 数据库事务
    - 存储过程
    - 函数
    - 存储引擎
    - JDBC
    - C3P0、Druid数据库连接池
- Java Web前后端交互（5）
    - Html基础与CSS
    - JavaScript与Jquery
    - XML与XML解析
    - Tomcat服务器安装与配置
    - Http协议
    - 服务器组件Servlet
    - JSP
    - EL表达式
    - 会话控制Cookie与Session
    - 服务器组件Filter
    - 服务器组件Listener
    - 异步数据传输框架Ajax
    - 文件的上传下载
    - 前端框架Bootstrap
- Java EE框架（40）
    - 系统整体分层解耦框架Spring
    - Spring IOC容器
    - Spring AOP容器
    - Spring高级应用
    - 轻量级Web框架SpringMVC
    - 轻量级持久化层框架Mybatis
    - Mybatis自定义插件开发
    - 反向代码生成器MybatisGenerator
    - Mybatis增强器Mybatis_Plus
    - 快速集成构建框架SpringBoot
    - 微服务构建框架SpringCloud
    - 服务网关SpringCloudGateway
    - 分布式配置SpringCloudConfig
    - 消息总线SpringCloudBus
    - 客户端负载均衡SpringCloudRibbon
    - 服务熔断与服务降级SpringCloud Hystrix
    - 服务注册与发现SpringCloud Eureka
    - 申明式服务调用SpringCloud Feign
    - Web安全框架SpringSecurity
    - 分布式Session管理SpringSession
    - 缓存机制
- 常用工具和环境
    - 项目构建、jar包管理工具Maven
    - 日志输出Log4j
    - 分布式版本管理工具Git和Github
    - 分布式系统与内存数据库Redis
    - MySQL集群
    - 服务器操作系统Linux常用操作、进程、线程
    - Java虚拟机JVM原理、优化
    - 高并发编程工具JUC
    - 命令解析器Shell
    - Intellij IDEA的使用
- Java EE高级
    - 服务器操作系统Linux常用操作
    - 远程调用技术WebService
    - 企业级现代数据访问技术SpringData
    - MySQL索引优化与锁
    - MyCat实现MySQL的分布式、分库分表、读写分离
    - 支付接口调用开发
    - Nginx反向代理、负载均衡、动静分离
    - 全文索引数据库Solr
    - 分布式构建框架Dubbo
    - Tomcat性能优化
    - JVM内存模式、参数调优
    - Java并发包JUC
- 互联网架构新技术（5）
    - 分布式架构中的注册中心Zookeeper
    - 全文检索引擎ElasticSearch
    - 日志收集、转发工具Logstash
    - 用于分析ElasticSearch中数据的可视化平台 Kibana
    - 分布式发布-订阅消息系统Kafka
    - 虚拟化应用容器Docker
    - 大数据分析存储框架Hadoop
    - 数仓仓库工具Hive
    - MapReduce编程模型
    - 前端技术栈Node.js+Vue.js
    - 消息队列ActiveMQ
    - 消息队列RabbitMQ
    - 消息队列RocketMQ
    - 数据库增量订阅Canal
    - 实时接口文档Swagger2
    - 社交登录SpringSocial
    - 分布式配置、服务发现与注册Nacas
    - 服务熔断Sentinel
    - 分布式事务Seata
- 大数据技术
    - 大数据技术概论
    - Hadoop概述与安装
    - HDFS伪分布式文件
    - Hadoop-HA高可用
    - HDFS完全分布式
    - Hive入门

-------

**Java 学习路线图**（2020-02-13--2020-05-10）

java基础阶段：（10）

相关工具：linux、IDEA

1.

java基础：[Java核心技术](https://www.bilibili.com/video/av48144058/?spm_id_from=333.788.b_636f6d6d656e74.5)、[java数据结构与算法](www.bilibili.com/video/av54029771/)、[java设计模式]( https://www.bilibili.com/video/av57936239/?spm_id_from=333.788.b_636f6d6d656e74.20 )

2. JUC：可延后学习
3. 面试题总结

学习指南：

1. 学习IO时，同时学习NIO，对比学习；
2. 学习集合时，学习java数据结构与算法，加深印象；
3. 学习linux及idea的使用教程；（1）

数据库技术阶段：（15）

1. 数据库基础：[MySQL基础]( www.bilibili.com/video/av21400736/ )
   、[MySQL高级](https://www.bilibili.com/video/av21334868/?spm_id_from=333.788.b_636f6d6d656e74.37 )）--(5)
2. 数据架构相关：[Mycat]( https://www.bilibili.com/video/av80469766/?spm_id_from=333.788.b_636f6d6d656e74.54 )可延后学习
3. 框架：[Mybatis](mybatis-examples/README.md)、Mybatisplus、通用Mapper、hibernate、jpa、springdata--(10)

Web基础：（10）

1. 基础：javascript、css、html、XML（2）
2. Java Web基础：servlet/jsp、mvc、cookie、session、EL表达式、简单标签、JSTL表达式、Fileter/Listener、文件上传下载、国际化（3）
3. 项目实战（5）

Java EE：（30）

Spring-->SpringMVC-->SpringBoot-->SpringCloud

MySQL基础-->MySQL高级-->MyCAT

Mybatis-->Mybatisplus-->通用mapper

hibernate-->Jpa-->[SpringData Jpa](./spring-data-jpa-examples/)

Redis

常用工具：Docker、Nginx、Jenkins、git、maven

SSM项目实战：（30）

面试阶段：（10）

数据库技术：

- MySQL-->JDBC-->Mybatis（MP等）-->hibernate-->SpringData
- redis

Web开发框架：Spring-->SpringMVC-->SpringBoot-->SpringCloud(或Dubbo)

框架整合：SSM、SSP等。

常用工具：

- [maven](docs/notes/Maven学习笔记.md)
- docker
- linux
- tomcat
- jenkins
- nginx
- git&github

思维训练：

- 设计模式
- 数据结构与算法

前端技术：html-->css-->javascript-->jQuery-->Ajax-->Vue