# MSL

^aaa635

MSL是Maximum Segment Lifetime，报文最大生存时间，它是任何报文在网络上存在的最长时间，超过这个时间报文将被丢弃。

# TTL
IP头中有一个TTL字段，是IP数据报可以经过的最大路由数，每经过一个处理他的路由器此值就减 1，当此值为0则数据报将被丢弃，同时发送ICMP报文通知源主机。