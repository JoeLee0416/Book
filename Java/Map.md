# Map

### HashMap
1. 无序，允许值为null，最多允许一个key为null
2. 底层基于哈希表实现，Java的哈希表由数组加链表实现，在JDK1.8中的HashMap还加入了红黑树
3. 初始容量与装载因子对HashMap影响比较大，初始容量默认为16
4. 线程不同步，即同一时刻可以有多个线程同时写HashMap，可能会导致数据不一致问题。如果需要满足线程同步，可以用Collections的synchronizedMap方法实现，或者使用ConcurrentHashMap。

### HashMap和HashTable的区别
相同：存储结构基本相同
不同：HashMap是非同步的，HashTable是同步的，需要同步使用ConcurrentHashMap；HashMap允许为null，HashTable不允许为null

