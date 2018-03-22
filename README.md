# Java工程师成神之路

> 原文来自微信公众号的[Java工程师成神之路(2018修订版)](https://mp.weixin.qq.com/s/UKwZkwYmDSVTbj62ACuapg)。本仓库内容是针对该文章中提到的各个知识点的汇总。

## 一、基础篇

### 1.1 JVM

**1.1.1 JVM内存结构**

堆、栈、方法区、直接内存、堆和栈区别

**1.1.2 Java内存模型**

内存可见性、重排序、顺序一致性、volatile、锁、final

**1.1.3 垃圾回收**

内存分配策略、垃圾收集器（G1）、GC算法、GC参数、对象存活的判定 

**1.1.4 JVM参数及调优**

**1.1.5 Java对象模型**

oop-klass、对象头

**1.1.6 HotSpot**

即时编译器、编译优化

**1.1.7 类加载机制**

classLoader、类加载过程、双亲委派（破坏双亲委派）、模块化（jboss modules、osgi、jigsaw）

**1.1.8 虚拟机性能监控与故障处理工具**

jps, jstack, jmap、jstat, jconsole, jinfo, jhat, javap, btrace、TProfiler

###1.2 编译与反编译

javac 、javap 、jad 、CRF

###1.3 Java基础知识

**1.3.1 阅读源代码**

String、Integer、Long、Enum、BigDecimal、ThreadLocal、ClassLoader & URLClassLoader、ArrayList & LinkedList、 HashMap & LinkedHashMap & TreeMap & CouncurrentHashMap、HashSet & LinkedHashSet & TreeSet

**1.3.2 Java中各种变量类型**

**1.3.2.1 熟悉Java String的使用，熟悉String的各种函数**

1. JDK 6和JDK 7中substring的原理及区别、
2. replaceFirst、replaceAll、replace区别、
3. String对“+”的重载、
4. String.valueOf和Integer.toString的区别、
5. 字符串的不可变性

**1.3.2.2 自动拆装箱**

Integer的缓存机制

**1.3.2.3 熟悉Java中各种关键字**

transient、instanceof、volatile、synchronized、final、static、const 原理及用法。

**1.3.2.4 集合类**

常用集合类的使用

1. ArrayList和LinkedList和Vector的区别 
2. SynchronizedList和Vector的区别
3. HashMap、HashTable、ConcurrentHashMap区别
4. Java 8中stream相关用法
5. apache集合处理工具类的使用
6. 不同版本的JDK中HashMap的实现的区别以及原因

**1.3.2.5 枚举**

枚举的用法、枚举与单例、Enum类

**1.3.3 Java IO&Java NIO，并学会使用**

bio、nio和aio的区别、三种IO的用法与原理、netty

**1.3.4 Java反射与javassist**

反射与工厂模式、 java.lang.reflect.*

**1.3.5 Java序列化**

1. 什么是序列化与反序列化、为什么序列化
2. 序列化底层原理
3. 序列化与单例模式
4. protobuf
5. 为什么说序列化并不安全

**1.3.6 注解**

元注解、自定义注解、Java中常用注解使用、注解与反射的结合

**1.3.7 JMS**

什么是Java消息服务、JMS消息传送模型

**1.3.8 JMX**

java.lang.management.*、 javax.management.*

**1.3.9 泛型**

1. 泛型与继承
2. 类型擦除
3. 泛型中K T V E  
4. object等的含义、泛型各种用法

**1.3.10 单元测试**

junit、mock、mockito、内存数据库（h2）

**1.3.11 正则表达式**

java.lang.util.regex.*

**1.3.12 常用的Java工具库**

commons.lang, commons.*... guava-libraries netty

**1.3.13 什么是API&SPI**

**1.3.14 异常**

异常类型、正确处理异常、自定义异常

**1.3.15 时间处理**

时区、时令、Java中时间API

**1.3.16 编码方式**

解决乱码问题、常用编码方式

**1.3.17 语法糖**

Java中语法糖原理、解语法糖

###1.4 Java并发编程

**1.4.1 什么是线程，与进程的区别**

**1.4.2 阅读源代码，并学会使用**

Thread、Runnable、Callable、ReentrantLock、ReentrantReadWriteLock、Atomic*、Semaphore、CountDownLatch、、ConcurrentHashMap、Executors

**1.4.3 线程池**

自己设计线程池、submit() 和 execute()

**1.4.4 线程安全**

死锁、死锁如何排查、Java线程调度、线程安全和内存模型的关系

**1.4.5 锁**

CAS、乐观锁与悲观锁、数据库相关锁机制、分布式锁、偏向锁、轻量级锁、重量级锁、monitor、锁优化、锁消除、锁粗化、自旋锁、可重入锁、阻塞锁、死锁

**1.4.6 volatile**

happens-before、编译器指令重排和CPU指令重

**1.4.7 synchronized**

1. synchronized是如何实现的？
2. synchronized和lock之间关系
3. 不使用synchronized如何实现一个线程安全的单例

**1.4.8 sleep 和 wait**

**1.4.9 wait 和 notify**

**1.4.10 notify 和 notifyAll**

**1.4.11 ThreadLocal**

**1.4.12 写一个死锁的程序**

**1.4.13 写代码来解决生产者消费者问题**

**1.4.14 守护线程**

守护线程和非守护线程的区别以及用法

## 二、 进阶篇

### 2.1 Java底层知识

**2.1.1 字节码、class文件格式**

**2.1.2 CPU缓存，L1，L2，L3和伪共享**

**2.1.3 尾递归**

**2.1.4 位运算**

用位运算实现加、减、乘、除、取余

### 2.2 设计模式

**2.2.1 了解23种设计模式**

**2.2.2 会使用常用设计模式**

单例、策略、工厂、适配器、责任链。

**2.2.3 实现AOP**

**2.2.4 实现IOC**

**2.2.5 不用synchronized和lock，实现线程安全的单例模式**

**2.2.6 nio和reactor设计模式**

### 2.3 网络编程

**2.3.1 tcp、udp、http、https等常用协议**

三次握手与四次关闭、流量控制和拥塞控制、OSI七层模型、tcp粘包与拆包

**2.3.2 http/1.0 http/1.1 http/2之前的区别**

**2.3.3 Java RMI，Socket，HttpClient**

**2.3.4 cookie 与 session**

cookie被禁用，如何实现session

**2.3.5 用Java写一个简单的静态文件的HTTP服务器**

实现客户端缓存功能，支持返回304 实现可并发下载一个文件 使用线程池处理客户端请求 使用nio处理客户端请求 支持简单的rewrite规则 上述功能在实现的时候需要满足“开闭原则”

**2.3.6 了解nginx和apache服务器的特性并搭建一个对应的服务器**

**2.3.7 用Java实现FTP、SMTP协议**

**2.3.8 进程间通讯的方式**

**2.3.9 什么是CDN？如果实现？**

**2.3.10 什么是DNS？**

**2.3.11 反向代理**

### 2.4 框架知识

**2.4.1 Servlet线程安全问题**

**2.4.2 Servlet中的filter和listener**

**2.4.3 Hibernate的缓存机制**

**2.4.4 Hiberate的懒加载**

**2.4.5 Spring Bean的初始化**

**2.4.6 Spring的AOP原理**

**2.4.7 自己实现Spring的IOC**

**2.4.8 Spring MVC**

**2.4.9 Spring Boot2.0**

**2.4.10 Spring Boot的starter原理，自己实现一个starter**

**2.4.11 Spring Security**

### 2.5 应用服务器

1. JBoss
2. tomcat
3. jetty
4. Weblogic

### 2.6 工具

1. git & svn
2. maven & gradle
