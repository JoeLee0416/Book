# Java集合
Java集合类位于Java.Util包中，主要有三种：Set、List和Map。
1. Collection：是List、Map和Queue的基本接口。
2. Iterator：迭代器，可以通过迭代器遍历集合内元素
3. Map：映射表的基础接口

### ArrayList
1. 底层基于动态数组实现
2. 根据索引查询元素，速度快；增删需要copy操作以及移位，因此增删比较慢（非绝对）
3. 默认容量为10，每次扩容为原来的1.5倍
4. 有序集合

### Vector
1. 底层基于数组实现
2. 线程安全
3. 默认容量为10，每次扩容为原来的2倍
4. 有序集合

### LinkedList
1. 底层基于双向链表实现，方便向前遍历
2. 查询某个元素需要遍历，查询慢；增删不需要copy操作以及移位，速度快

*注意：当一直对尾部执行添加或删除操作的情境下，ArrayList比LinkedList效率更高*

### ArrayList和Vector的区别
相同:都是有序集合，底层为数组，允许元素重复以及为null
不同：ArrayList不同步，Vector同步；ArrayList扩容为原来的1.5倍，Vector扩容为原来的2倍