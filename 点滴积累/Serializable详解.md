### 为什么有些Java对象需要实现Serializable空接口？有什么作用？

Serializable（Java序列化）：用于将Java对象转换为字节数组，便于存储或传输。序列化后依然可以将字节数组转换会Java对象原有的状态（反序列化）。

序列化思想：“冻结”对象状态，然后写到磁盘或者在网络中传输

反序列化思想：“解冻”对象状态，重新获得可用的 Java 对象。

注意：

1. 如果序列化对象没有实现Serializable接口，会抛出NotSerializableException异常
2. static和transient修饰的字段是不会被序列化的
3. serialVersionUID序列化ID，它是决定 Java 对象能否反序列化成功的重要因子。在反序列化时，Java 虚拟机会把字节流中的 serialVersionUID 与被序列化类中的 serialVersionUID 进行比较，如果相同则可以进行反序列化，否则就会抛出序列化版本不一致的异常。

