# CAP理论
CAP理论是分布式系统设计中最基础，也是最为关键的理论。常用于分布式存储，它指出，分布式数据存储不可能同时满足以下三个条件。

- 一致性（Consistency）：每次读取要么获得最近写入的数据，要么获得一个错误。 
- 可用性（Availability）：每次请求都能获得一个（非错误）响应，但不保证返回的是最新写入的数据。 
- 分区容忍（Partition tolerance）：尽管任意数量的消息被节点间的网络丢失（或延迟），系统仍继续运行。

也就是说，CAP 定理表明，在存在网络分区的情况下，一致性和可用性必须二选一。而在没有发生网络故障时，即分布式系统正常运行时，一致性和可用性是可以同时被满足的。这里需要注意的是，CAP 定理中的一致性与ACID数据库事务中的一致性截然不同。