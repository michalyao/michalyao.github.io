---
layout: post
title: "推荐几个 Github 上好玩的 Java Repo"
description: "Github 上流行的 Java 库，框架，语言，数据库应有尽有。"
date: 2017-04-12
tags: [Java, Github, Share]
comments: true
---

正文之前打波小广告，[Evermonkey](http://monkey.yoryor.me) 是我前几天刚刚完成的一个小项目，类似马克飞象的一款 VS Code 扩展，能够在 VS Code 中使用 Markdown 新建，编辑，打开和更新印象笔记。

## 基础

### guava 

[google/guava](https://github.com/google/guava) -- Google Core Libraries for Java.

虽然 JDK1.8 已经补充了很多 Guava 之前提供的特性，但是 Guava 提供的集合，缓存等等工具依然是你效率开发的必备神器。很优秀的源码，建议新手多读读。

### java-design-patterns

[iluwatar/java-design-patterns](https://github.com/iluwatar/java-design-patterns) -- Design patterns implemented in Java.

学习设计模式的不二选择，不止四人帮，还为你提供了很多现代软件开发的解决方案，架构，模型等等。不管是新手还是老鸟都适合花时间读一读。

## 框架

### spring

[spring-project](https://github.com/spring-projects) -- Spring CNY Grazing Bucket.

不多说了，不管你喜不喜欢 Spring，它为你赚得钱你总归不会拒绝。当然不是黑 Spring，相比以前已经进步不少了，但是前提是你的公司要在用 Spring-boot...

### vertx

[eclipse/vert.x](https://github.com/eclipse/vert.x) -- Vert.x is a tool-kit for building reactive applications on the JVM.

厌倦了SSM？ 厌倦了分布式Dubbo? 想做个新世纪的 Java 程序员？想感受一下异步应用的性能？那我推荐你好好看看这个库。微服务，响应式应用， DevOps...除却这些火爆的新概念，Vertx 最重要的是能让你重新感受到编程的乐趣。

``` java
public class HttpServer extends AbstractVerticle {
    @Override
    public void start() throws Exception {
        vertx.createHttpServer().requestHandler(req -> {
            req.response().end("Hello Vert.x!");
        }).listen(80, "localhost");
        super.start();
    }
}
```

### dropwizard

[dropwizard/dropwizard](https://github.com/dropwizard/dropwizard) -- A damn simple library for building production-ready RESTful web services.

描述的很清楚了，为 RESTful 而生，到底有多便捷，那要你学习使用之后才知晓。

## 语言

### Scala

[scala/scala](https://github.com/scala/scala) -- The Scala programming language.

基于 JVM 的编程语言太多太多了，Scala 这门语言如果你学习一下，我相信你会爱上它的。面向对象，函数式编程，能够满足你当初对编程的所有幻想。尤其在大数据，机器学习如火如荼的时代，对你的qian途很有帮助。平时没有太多机会接触 Scala，但是 Akka，Play 这些词你总该听过。当初用过 [gatling](https://github.com/gatling/gatling) 给公司做过集群应用的负载测试。

### kotlin

[JetBrains/kotlin](https://github.com/JetBrains/kotlin) -- The Kotlin Programming Language

说实话，没太接触过 kotlin, 不过 JetBrains 这家公司你可能不会陌生。为了我最爱的 IDE，友情推荐一发，毕竟这么有逼格的公司开发的语言也不会太差。

## 数据库

### elasticsearch

[elastic/elasticsearch](https://github.com/elastic/elasticsearch) -- Open Source, Distributed, RESTful Search Engine.

许多年前，一个叫Shay Banon的待业工程师跟随他的新婚妻子来到伦敦，他的妻子想在伦敦学习做一名厨师。而他在伦敦寻找工作的期间，接触到了Lucene的早期版本，他想为自己的妻子开发一个方便搜索菜谱的应。爱情的结晶，文本搜索必备神器。

### opentsdb

[OpenTSDB/opentsdb](https://github.com/OpenTSDB/opentsdb) -- A scalable, distributed Time Series Database. 

时序型数据库鼻祖，官方文档很详细，如果有运维监控方面的业务需求可以学习学习。有一个基于 opentsdb 重写的库 [kairosbd](https://github.com/kairosdb/kairosdb)，代码设计的很好，不过文档不是很详细，不推荐不熟悉时序型数据库的同学作为入门库。

## 其他

### Netty

[netty/netty](https://github.com/netty/netty) -- Netty project - an event-driven asynchronous network application framework

高性能、异步事件驱动的NIO框架，它提供了对TCP、UDP和文件传输的支持，作为一个异步NIO框架，Netty的所有IO操作都是异步非阻塞的。 前面提到的 Vert.x 底层就是用 Netty 实现的。也许你觉得这东西太底层，但是时间久了你就会明白，精华都在底层。

### RxJava

[ReactiveX/RxJava](https://github.com/ReactiveX/RxJava) -- Reactive Extensions for the JVM.

同样是异步事件驱动模型，相信做 Android 的同学一定不会陌生。。。


喜欢的朋友们就到 github 上面给个 star 吧。