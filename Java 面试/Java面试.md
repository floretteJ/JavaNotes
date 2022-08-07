# 1、JVM 调优

![image-20220607092809525](D:/Typora/imgs/image-20220607092809525.png)

![image-20220607095027352](D:/Typora/imgs/image-20220607095027352.png)

# 2、JDK、JRE、JVM 三者关系

![image-20220607095640317](D:/Typora/imgs/image-20220607095640317.png)

# 3、 == 和 equals 比较

![image-20220607100131027](D:/Typora/imgs/image-20220607100131027.png)

![image-20220607100330060](D:/Typora/imgs/image-20220607100330060.png)

# 4、final 及局部内部类和匿名内部类只能访问局部 final 变量

![image-20220607100408254](D:/Typora/imgs/image-20220607100408254.png)

![image-20220607100557862](D:/Typora/imgs/image-20220607100557862.png)

![image-20220607100701921](D:/Typora/imgs/image-20220607100701921.png)

![image-20220607100802192](D:/Typora/imgs/image-20220607100802192.png)

![image-20220607100958155](D:/Typora/imgs/image-20220607100958155.png)

# 5、String、StringBuilder、StringBuffer 区别

![image-20220607101104085](D:/Typora/imgs/image-20220607101104085.png)

# 6、重载、重写的区别

![image-20220607101338671](D:/Typora/imgs/image-20220607101338671.png)

# 7、接口、抽象类的区别

![image-20220607101522195](D:/Typora/imgs/image-20220607101522195.png)

# 8、List 和 Set 的区别

![image-20220607102000434](D:/Typora/imgs/image-20220607102000434.png)

# 9、hashCode 与 equals 的区别

![image-20220607102131559](D:/Typora/imgs/image-20220607102131559.png)

# 10、ArrayList 和 LinkedList 的区别

![image-20220607102923921](D:/Typora/imgs/image-20220607102923921.png)

# 11、HashMap 和 HashTable 的区别及底层实现

![image-20220607103718219](D:/Typora/imgs/image-20220607103718219.png)

# 12、ConcurrentHashMap 原理（jdk7 及 jdk8）

![image-20220607104327094](D:/Typora/imgs/image-20220607104327094.png)

# 13、字节码

![image-20220607112133894](D:/Typora/imgs/image-20220607112133894.png)

# 14、Java 类加载器

![image-20220607133532246](D:/Typora/imgs/image-20220607133532246.png)

# 15、双亲委派机制

![image-20220607133741483](D:/Typora/imgs/image-20220607133741483.png)

![image-20220607134031462](D:/Typora/imgs/image-20220607134031462.png)

# 16、Java 中的异常体系

![image-20220607134245773](D:/Typora/imgs/image-20220607134245773.png)

# 17、GC 如何判断对象可以被回收

![image-20220607134715420](D:/Typora/imgs/image-20220607134715420.png)

![image-20220607134735517](D:/Typora/imgs/image-20220607134735517.png)

# 18、线程的生命周期

![image-20220607135253024](D:/Typora/imgs/image-20220607135253024.png)

![image-20220607135316670](D:/Typora/imgs/image-20220607135316670.png)

# 19、sleep()、wait()、join()、yield() 的区别

![image-20220607135446391](D:/Typora/imgs/image-20220607135446391.png)

![image-20220607135728380](D:/Typora/imgs/image-20220607135728380.png)

![image-20220607135928775](D:/Typora/imgs/image-20220607135928775.png)

# 20、线程安全的理解

![image-20220607141010637](D:/Typora/imgs/image-20220607141010637.png)

# 21、Thread 和 Runnable 的区别

![image-20220608090254504](D:/Typora/imgs/image-20220608090254504.png)

![image-20220608090405350](D:/Typora/imgs/image-20220608090405350.png)

# 22、守护线程的理解

![image-20220608090544045](D:/Typora/imgs/image-20220608090544045.png)

![image-20220608090611448](D:/Typora/imgs/image-20220608090611448.png)

# 23、ThreadLocal 的原理及使用场景

![image-20220608090711438](D:/Typora/imgs/image-20220608090711438.png)

![image-20220608091103454](D:/Typora/imgs/image-20220608091103454.png)

# 24、ThreadLocal 内存泄漏原因及解决

![image-20220608091404128](D:/Typora/imgs/image-20220608091404128.png)

![image-20220608090859530](D:/Typora/imgs/image-20220608090859530.png)

![image-20220608091913278](D:/Typora/imgs/image-20220608091913278.png)

![image-20220608092030649](D:/Typora/imgs/image-20220608092030649.png)

# 25、并发、并行、串行的区别

![image-20220608092411888](D:/Typora/imgs/image-20220608092411888.png)

# 26、并发的三大特性

![image-20220608092557062](D:/Typora/imgs/image-20220608092557062.png)

![image-20220608093428692](D:/Typora/imgs/image-20220608093428692.png)

保证原子性（第一、二、三步是一起的）

![image-20220608094405451](D:/Typora/imgs/image-20220608094405451.png)

保证可见性 volatile+CAS（第三、四步是一起的）：总线锁定、缓存一致性协议（MESI）

![image-20220608094814186](D:/Typora/imgs/image-20220608094814186.png)

![image-20220608095228163](D:/Typora/imgs/image-20220608095228163.png)

volatile：保证了可见性和有序性，不保证原子性

synchronized：保证了三大特性

# 27、线程池使用原因及流程

![image-20220608095537957](D:/Typora/imgs/image-20220608095537957.png)

![image-20220608100628419](D:/Typora/imgs/image-20220608100628419.png)

# 28、线程池中阻塞队列的作用及线程复用原理

![image-20220608100738752](D:/Typora/imgs/image-20220608100738752.png)

![image-20220608101405586](D:/Typora/imgs/image-20220608101405586.png)



# 29、Spring 是什么

![image-20220608101751360](D:/Typora/imgs/image-20220608101751360.png) 

# 30、对 IOC 的理解

![image-20220608102839452](D:/Typora/imgs/image-20220608102839452.png)

![image-20220608103224925](D:/Typora/imgs/image-20220608103224925.png)

# 31、对 AOP 的理解

![image-20220608102213304](D:/Typora/imgs/image-20220608102213304.png)

# 32、如何实现一个 IOC 容器

![image-20220607105003870](D:/Typora/imgs/image-20220607105003870.png)

# 33、BeanFactory 和 ApplicationContext 的区别

![image-20220608103536535](D:/Typora/imgs/image-20220608103536535.png)

![image-20220608103834380](D:/Typora/imgs/image-20220608103834380.png)

# 34、Spring Bean 的生命周期及作用域

![image-20220608104104605](D:/Typora/imgs/image-20220608104104605.png)

![image-20220608104345628](D:/Typora/imgs/image-20220608104345628.png)

# 35、Spring 中的单例 Bean 是线程安全的吗？

![image-20220608104742547](D:/Typora/imgs/image-20220608104742547.png)

# 36、Spring 框架中的设计模式

![image-20220608105334988](D:/Typora/imgs/image-20220608105334988.png)

![image-20220608110104148](D:/Typora/imgs/image-20220608110104148.png)

![image-20220608110129557](D:/Typora/imgs/image-20220608110129557.png)

# 37、Spring 事务的实现方式、原理及隔离级别

![image-20220608110230098](D:/Typora/imgs/image-20220608110230098.png)

![image-20220608110509358](D:/Typora/imgs/image-20220608110509358.png)

# 38、Spring 事务传播机制

![image-20220608110828543](D:/Typora/imgs/image-20220608110828543.png)

![image-20220608111754114](D:/Typora/imgs/image-20220608111754114.png)

# 39、Spring 事务什么时候会失效？

![image-20220608111831056](D:/Typora/imgs/image-20220608111831056.png)

# 40、Bean 自动装配的方式

![image-20220608112316207](D:/Typora/imgs/image-20220608112316207.png)

![image-20220608112634255](D:/Typora/imgs/image-20220608112634255.png)

# 41、Spring、Spring MVC、Spring Boot 的区别

![image-20220608112738035](D:/Typora/imgs/image-20220608112738035.png)

# 42、Spring MVC 的工作流程

![image-20220609102558732](D:/Typora/imgs/image-20220609102558732.png)

# 43、Spring MVC 的主要组件

![image-20220609102705330](D:/Typora/imgs/image-20220609102705330.png)

![image-20220609103137672](D:/Typora/imgs/image-20220609103137672.png)

![image-20220609103157197](D:/Typora/imgs/image-20220609103157197.png)

# 44、Spring Boot 自动配置原理![image-20220609103239689](D:/Typora/imgs/image-20220609103239689.png)

# 45、理解 Spring Boot 中的 Starter

![image-20220609103406105](D:/Typora/imgs/image-20220609103406105.png)

# 46、什么是嵌入式服务器?

![image-20220609103533645](D:/Typora/imgs/image-20220609103533645.png)

# 47、Mybatis 的优缺点

![image-20220609103619324](D:/Typora/imgs/image-20220609103619324.png)

# 48、Mybatis 和 Hibernate 的区别

![image-20220609103733938](D:/Typora/imgs/image-20220609103733938.png)

![image-20220609103906211](D:/Typora/imgs/image-20220609103906211.png)

![image-20220609103922965](D:/Typora/imgs/image-20220609103922965.png)

![image-20220609103942660](D:/Typora/imgs/image-20220609103942660.png)

# 49、#{} 和 ${} 的区别

![image-20220609104005093](D:/Typora/imgs/image-20220609104005093.png)

# 50、Mybatis 的插件运行原理

![image-20220609104125571](D:/Typora/imgs/image-20220609104125571.png)

![image-20220609104205704](D:/Typora/imgs/image-20220609104205704.png)



# 51、索引的基本原理

![image-20220609104244341](D:/Typora/imgs/image-20220609104244341.png)

# 52、MySQL 聚簇（InnoDB）与非聚簇索引（MyISAM）的区别

![image-20220609104834062](D:/Typora/imgs/image-20220609104834062.png)

![image-20220609105844608](D:/Typora/imgs/image-20220609105844608.png)

# 53、MySQL 索引的数据结构

![image-20220609110312942](D:/Typora/imgs/image-20220609110312942.png)

![image-20220609110506776](D:/Typora/imgs/image-20220609110506776.png)

![image-20220609110629004](D:/Typora/imgs/image-20220609110629004.png)

![image-20220609110743295](D:/Typora/imgs/image-20220609110743295.png)

# 54、索引的设计原则

![image-20220609111130617](D:/Typora/imgs/image-20220609111130617.png)

# 55、MySQL 锁的分类

![image-20220609111444052](D:/Typora/imgs/image-20220609111444052.png)

![image-20220609112244357](D:/Typora/imgs/image-20220609112244357.png)

![image-20220609112530576](D:/Typora/imgs/image-20220609112530576.png)

![image-20220609112900898](D:/Typora/imgs/image-20220609112900898.png)

# 56、MySQL 执行计划

![image-20220610110329143](D:/Typora/imgs/image-20220610110329143.png)

![image-20220610110804853](D:/Typora/imgs/image-20220610110804853.png)

![image-20220610110831745](D:/Typora/imgs/image-20220610110831745.png)

![image-20220610110842494](D:/Typora/imgs/image-20220610110842494.png)

# 57、MySQL 事务的基本特性及隔离级别

![image-20220610112115193](D:/Typora/imgs/image-20220610112115193.png)

![image-20220610112642663](D:/Typora/imgs/image-20220610112642663.png)

![image-20220610113317845](D:/Typora/imgs/image-20220610113317845.png)

# 58、SQL 耗时、优化慢查询？

![image-20220610113504070](D:/Typora/imgs/image-20220610113504070.png)

# 59、ACID 靠什么保证的？

![image-20220610113949980](D:/Typora/imgs/image-20220610113949980.png)

# 60、什么是 MVCC（隔离性）

![image-20220610114402518](D:/Typora/imgs/image-20220610114402518.png)

![image-20220610114608734](D:/Typora/imgs/image-20220610114608734.png)

![image-20220610114707910](D:/Typora/imgs/image-20220610114707910.png)

![image-20220610114747946](D:/Typora/imgs/image-20220610114747946.png)

![image-20220610114758149](D:/Typora/imgs/image-20220610114758149.png)

# 61、MySQL 主从同步原理

![image-20220610115317959](D:/Typora/imgs/image-20220610115317959.png)

![image-20220610165749900](D:/Typora/imgs/image-20220610165749900.png)

# 62、MyISAM 和 InnoDB 的区别

![image-20220610170042051](D:/Typora/imgs/image-20220610170042051.png)

![image-20220610170217620](D:/Typora/imgs/image-20220610170217620.png)

# 63、MySQL 中索引类型对数据库性能的影响

![image-20220610170443635](D:/Typora/imgs/image-20220610170443635.png)



# 64、Redis 中的 RDB 和 AOF 机制

![image-20220610171544291](D:/Typora/imgs/image-20220610171544291.png)

![image-20220610172038327](D:/Typora/imgs/image-20220610172038327.png)

![image-20220610172308958](D:/Typora/imgs/image-20220610172308958.png)

# 65、Redis 过期键的删除策略

![image-20220610172455531](D:/Typora/imgs/image-20220610172455531.png)

# 66、Redis 单线程模型

![image-20220610172906501](D:/Typora/imgs/image-20220610172906501.png)

# 67、缓存雪崩、缓存穿透、缓存击穿

![image-20220610174154624](D:/Typora/imgs/image-20220610174154624.png)

![image-20220610174433237](D:/Typora/imgs/image-20220610174433237.png)

![image-20220610174448483](D:/Typora/imgs/image-20220610174448483.png)

# 68、Redis 事务实现

![image-20220610175105901](D:/Typora/imgs/image-20220610175105901.png)

![image-20220610175542493](D:/Typora/imgs/image-20220610175542493.png)

![image-20220610175615327](D:/Typora/imgs/image-20220610175615327.png)

# 69、Redis 集群方案

![image-20220610180039587](D:/Typora/imgs/image-20220610180039587.png)

![image-20220610180447227](D:/Typora/imgs/image-20220610180447227.png)

![image-20220610180738280](D:/Typora/imgs/image-20220610180738280.png)

![image-20220610181009262](D:/Typora/imgs/image-20220610181009262.png)

# 70、Redis 主从复制原理

![image-20220610181206853](D:/Typora/imgs/image-20220610181206853.png)

![image-20220610181419683](D:/Typora/imgs/image-20220610181419683.png)

![image-20220610181146120](D:/Typora/imgs/image-20220610181146120.png)





# 71、CAP、BASE 理论

![image-20220610182335208](D:/Typora/imgs/image-20220610182335208.png)

![image-20220610182809488](D:/Typora/imgs/image-20220610182809488.png)

# 72、负载均衡算法、类型

![image-20220610183006704](D:/Typora/imgs/image-20220610183006704.png)