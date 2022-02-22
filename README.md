## redis-demo

### 介绍

redis学习案例

### 结构

* springboot-redis-1 项目

  为redis的简单使用、包括布隆过滤器的相关案例

* springboot-redis-2 项目

  为自定义客户端的项目；各个客户端的使用
  同时包含redisson的相关使用；

  包含其中的lua脚本及时间轮的使用；

* lottery

  redis实战——转盘抽奖
  
* redis-network-model

  网络模型相关

  BIO\NIO等实例

## 补充

### 原来的URL

https://gitee.com/cl1429745331/redis-demo.git

### 我的修改

``` 
    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>2.5.2</version><version>2.6.0</version>
        <relativePath/> <!-- lookup parent from repository -->
	</parent>
    <modules>
        <module>lottery</module>
        <module>redis-network-model</module>
        <module>springboot-redis-1</module>
    </modules>

```

### 其他问题

我是在Windows压缩上传到服务器再解压的，然后src路径下使用命令mvn spring-boot:run运行。这是我这样命令成功运行的第一个项目，也是最近以来的最后一个项目。我对多模块方面了解还不够多。

项目中用到的MySQL和redis我都是用docker容器运行的，感觉比较方便，而且还可以迁移容器。

项目使用的maven，我了解到它很早就被**技术雷达**标记为不暂缓了。以后我也会多尝试gradle。
