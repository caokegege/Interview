# JavaList面试题汇总

1、List集合：ArrayList、LinkedList、Vector等。

2、Vector是List接口下线程安全的集合。

3、List是有序的。

4、ArrayList和LinkedList数据结构不一样，前者用在查询较多的场合，后者适用于插入较多的场合。

5、ArrayList使用的是数组结构，LinkedList使用的是链表结构。

6、Jdk1.7之前ArrayList默认大小是10，JDK1.7之后是0，JDK差异，每次约按1.5倍扩容。

7、List中的Vector才是线程安全的，其他要实现线程安全使用工具类Collections.synchronizedList(new ArrayList())方法。

8、使用List自身的sort方法，或者使用Collections.sort(list)方法;

9、Arrays.asList使用的是final数组，并且不支持add方法，不支持扩容。

10、List>Array使用toArray方法，Array>List使用Arrays.asList(array)方法，由于它是固定的，不固定的可以使用new ArrayList(Arrays.asList(array))。

11、 ArrayList和LinkedList的区别：

1）ArrayList是实现了基于动态数组的数据结构，LinkedList基于链表的数据结构。 （LinkedList是双向链表，有next也有previous）

2）对于随机访问get和set，ArrayList觉得优于LinkedList，因为LinkedList要移动指针。

3）对于新增和删除操作add和remove，LinedList比较占优势，因为ArrayList要移动数据。

# Java Map面试题汇总

1、常用的Map集合：HashMap、HashTable、LinkedHashMap、ConcurrentHashMap。

2、Collection是List、Set父接口不是Map父接口。

3、HashMap不是线程安全的。线程安全的有HashTable、ConcurrentHashMap、SynchronizedMap，性能最好的是ConcurrentHashMap。

4、使用HashMap要注意避免集合的扩容，它会很耗性能，根据元素的数量给它一个初始大小的值。

5、HashMap是数组和链表组成的，默认大小为16，当hashmap中的元素个数超过数组大小*loadFactor（默认值为0.75）时就会把数组的大小扩展为原来的两倍大小，然后重新计算每个元素在数组中的位置。

6、按添加顺序使用LinkedHashMap,按自然顺序使用TreeMap,自定义排序TreeMap(Comparetor c)。

7、HashMap的链表结构设计是用来解决key的hash冲突问题的。

8、HashMap的键值都可以为NULL，HashTable不行。

9、key的hash冲突，如果key equals一致将会覆盖值，不一致就会将值存储在key对应的链表中。

10、先根据key的hashcode值找到对应的链表，再循环链表，根据key的hash是否相同且key的==或者equals比较操作找到对应的值。

11、HashMap不是线程安全的，效率高，允许有null的键和值。线程安全，效率低，不允许有null的键和值。

12、HashSet和HashTree的区别：HashSet哈希表实现，数据是无序的，可以放入一个null值。TreeSet二差树实现，数据是自动排好序的，不允许放入null值。

# String经典面试题

1、String不是基本数据类型。

2、String是final类型的，不可变。

3、比较字符串的值是否相同用equals,比较字符串对象是否同一个用==。

4、jdk7+中的switch可以使用String类型。

5、创建了两个，”abc”本身创建在常量池，通过new又创建在堆中。

6、String、StringBuffer、StringBuilder最大的不同是String不可变，后者可变。StringBuffer是线程安全的，StringBuilder线程不安全速度较快。

7、trim去掉字符串首尾的空白字符。

8、既然String是final的，所以不能被继承。

9、可以自定义java.lang.String类并编译成功，但不能被加载使用，具体请学习类加载机制。

10、String > byte[] 通过String类的getBytes方法；byte[] > String通过new String(byte[])构造器。
