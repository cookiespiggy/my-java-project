# java
1、hashMap hashTable区别？ 强一致和弱一致问题？

答：[1、Java中重要集合类的对比.md]()

2、hashMap哈希算法是怎样的，如何做到均匀hash的，做了哪些优化？hashMap中hash算法怎样的，什么情况下效率最低、最快？

答：[2、HashMap实现详解.md]()

3、jdk中常用的设计模式，及应用

答：[JDK中常用设计模式的应用.md]()

4、concurrentHashMap的锁分段技术？读时为什么不加锁？为什么是弱一致？

答：[2、HashSet、HashMap、HashTable、TreeSet和TreeMap区别.md]()

5、treeMap的红黑树

-- 有关红黑树的面试题是怎样的？？？

6、string的hashcode算法

答：[String 类中 hashCode() 方法详解.md]()

7、Collections.sort()如何排序的

答：[5、Collections.sort方法的算法实现.md]()



# 线程
1、thread 多次start 会怎样？

答：第二次调start()方法时，就会抛IllegalThreadStateException运行时异常。但第一次start的线程还会执行完。



# web
1、长连接和短连接区别，如何保证长连接？

答：[1、短连接、长连接、http和websocket的区别.md]()

2、session的实现原理，与cookie的关系？

答：[2、session的实现原理，与cookie的关系.md]()

3、分布式session的四种实现方式？

答：[2、session的实现原理，与cookie的关系.md]()



# mysql
1、死锁的条件？如何避免死锁？

答：[3、死锁及解决办法.md]()

2、mysql针对大数据量时的性能优化？

答：[2、数据库性能优化.md]()

3、事务 隔离级别

答：[4、事务和隔离级别介绍.md]()

4、倒排索引？索引的优点 缺点



# spring
1、spring mvc启动过程？

答：[1、spring mvc启动过程.md]()

2、spring mvc如何管理url和controller的映射

答：[2、spring mvc如何管理url和controller的映射.md]()

3、spring mvc实现原理，用什么数据结构管理bean依赖的？

答：[3、spring mvc如何管理bean依赖.md]()

4、ioc和aop如何实现的？



# 分布式
1、zk的分布式锁, 和redis的分布式锁的区别？？

答：zk实现的分布式锁，可以持久化，可靠性更好，但频繁的创建、删除节点，性能开销较大，适合并发量不大、对可靠性要求较高的核心业务场景。
redis的效率更高，但对于客户端宕机等情况不能优雅释放锁，也不够可靠。
[1、zk和redis的分布式锁的对比.md]()

2、kafka负载均衡的实现，选举leader的实现

3、分布式事务如何实现的。

答：解决分布式事务的最好办法就是不考虑分布式事务。
拆分大的业务流程，转化成几个小的业务流程，然后考虑最终一致性。
复杂的业务交互过程中，不建议使用强一致性的分布式事务。就像刚说的问题一样，把分布式的事务过程拆解成多个中间状态，中间状态的东西不允许用户直接操作，等状态都一致成功，或者检测到不一致的时候全部失败掉。就解耦了这个强一致性的过程。

4、如何解决缓存被“击穿”问题？

答：[2、解决缓存被击穿的问题.md]()



# jvm
1、jvm运行时问题

2、性能调优

3、堆 栈 何时发生OutOfMemory异常？

4、happens-before机制是什么鬼？
















# 算法
1、快排 冒泡 归并 各自的高级实现，时间复杂度

2、二叉树反转 b树 b+树区别？数据库为什么用btree不用其他树？

3、二分查找

4、lru代码实现

5、快速幂 取模算法

6、如何最少时间复杂度求一个大数组中的第k大的数



