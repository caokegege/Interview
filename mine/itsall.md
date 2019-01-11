#前言
每次准备面试题的时候都是拿起一大坨资料来看，没有系统性的总结，做成一个知识点的目录。
所以想利用这次被辞退的机会，整理出一篇文档出来，在自己复习的同时可以加深自己的记忆。

##Java
1. JVM的内存划分，各部分作用
2. GC垃圾回收机制，有哪些垃圾回收器，分代收集
3. Java有哪些基本类型，分别占用多少空间，Object，包装类型空间 
4. Java集合框架类图，ArrayList、LinkedList、HashSet等源码
5. Map框架类图，HashMap源码（1.7,1.8），HashTable，ConcurrentHashMap
6. JUC并发包，ConHashMap,CopyOnWrite,Atomic,lock,CompletableFuture,Synchronized,Volatile
7. 线程池工具类Executors,各参数含义，线程队列，拒绝策略

## DB
1. MySQL存储引擎，MyISAM,Innodb作用与区别
2. SQL优化，慢查询，索引的构建，最左前缀
3. 索引的数据结构，B+tree
4. 索引分类，主键，唯一，聚集
5. 事务隔离级别，ACID，MVCC，next-key，间隙锁，排它锁
6. MySQL分库分表，垂直/水平，主从复制，延迟

## cache
1. redis数据类型，各应用场景
2. redis与memcache区别，redis vm机制
3. redis数据淘汰策略，如何实现
4. redis持久化策略，rdb，aof
5. redis分布式锁
6. redis与MySQL缓存一致性
7. redis高可用，redis cluster

## MQ
1. MQ的使用场景，运用实现，AMQ、RMQ、Kafka有什么区别
2. MQ发送保证，重复发送，重复消费，失败，幂等
3. MQ延迟队列，死信队列，持久化

## RPC
1. 什么是RPC，熟悉的RPC框架，dubbo，springcloud
2. 服务注册发现，失败重试等如何实现
3. 微服务，SOA，服务治理，降级，熔断

## Linux
1. Linux的常用命令
2. Awk
3. shell

## Spring
1. IOC/AOP
2. 动态代理如何实现
3. 设计模式，工厂，单例
4. dispatchServlet处理过程
5. 事务的传播机制，如何实现，不能被代理的情况

## 算法
1. 各种排序算法
2. 数组旋转，合并，去重
3. 斐波那契数列
