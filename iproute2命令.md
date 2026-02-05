### 1.开启ipv4内核转发 值为0禁止转发,值为1开启转发

方式一：编辑/proc/sys/net/ipv4/ip_forward

方式二：sudo sysctl net.ipv4.ip_forward



### 2.iproute2的相关命令
`ip  [link | addr | route | neigh | tuntap]  [show | dev | list | del | add | set ]`<br />
具体教程可查看博客园`大数据老司机`的[笔记](https://www.cnblogs.com/liugp/p/16395089.html)

1. 创建虚拟网卡(tun是只认识ip的虚拟网卡,tap是只认识mac(如同在交换机)的网卡，二层网卡)
* ip tuntap add dev [网卡名称] mode [ tap | tun ]
>>- eg. ip tuntap add dev tap0 mode tap
>>- eg. ip tuntap add dev tun2 mode tun
* 

