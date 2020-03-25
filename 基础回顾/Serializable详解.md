### 为什么有些Java对象需要实现Serializable空接口？有什么作用？原理是什么？

序列化：用于将Java对象转换为有序字节流，便于存储或传输；序列化后的字节流保存了Java对象的状态以及相关的描述信息

反序列化：获取到序列化后的对象字节流后，根据字节流中所保存的对象状态及描述信息，通过反序列化重建对象。

序列化思想：“冻结”对象状态，然后写到磁盘或者在网络中传输

反序列化思想：“解冻”对象状态，重新获得可用的 Java 对象。

注意：

1. 如果序列化对象没有实现Serializable接口，会抛出NotSerializableException异常
2. static和transient修饰的字段是不会被序列化的
3. serialVersionUID序列化ID，它是决定 Java 对象能否反序列化成功的重要因子。在反序列化时，Java 虚拟机会把字节流中的 serialVersionUID 与被序列化类中的 serialVersionUID 进行比较，如果相同则可以进行反序列化，否则就会抛出序列化版本不一致的异常。

