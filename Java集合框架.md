集合框架 

Collection(继承Iterator):工具类 Collections

List（存储可重复，有序（插入顺序）的对象）:ArrayList LinkedList Vector Stack 

特点:List和数组类似，可以动态增长，根据实际存储的数据的长度自动增长List的长度。查找元素效率高，插入删除效率低，因为会引起其他元素位置改变



 Set（存储不可重复，无序的对象）:SortedSet(有序) HashSet（允许包含值为null的元素，但最多只能一个）TreeSet LinkedHashSet（有序，原因:实现了LinkedHashMap对象）

特点:Set检索效率低下，删除和插入效率高，插入和删除不会引起元素位置改变



Queue:队列 LikedList实现了Queue接口，可以把LinkedList当成Queue来用。



Map(存储键值对):HashMap（根据键的HashCode值存储数据，具有很快的访问速度，最多允许一条记录的键为null，不支持线程同步。）SortedMap(使 Key 保持在升序排列) TreeMap LinkedHashMap WeakHashMap Hashtable

常用的有:ArrayList、LinkedList、HashSet、LinkedHashSet、HashMap、LinkedHashMap 等等