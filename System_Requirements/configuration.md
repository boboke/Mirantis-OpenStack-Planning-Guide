# Target 节点硬件配置


环境特征：
- 12台服务器（一个Fuel 主节点，3台控制节点，3台存储节点，5台计算节点）
- 高可用HA 配置
- Neutron 网络，使用另外的VLAN 或者 GRE 技术
- Ceph 作为Cinder，Glance，和Nova后端存储
- 三额外的服务器作为MongoDB节点将被需要，为 Ceilometer / MongoDB 环境准备。

## 控制节点（3) ##

除了OpenStack组件（Nova,Neutron,Cinder和Glance），控制节点要求有足够的资源运行Ceph监控以及Mysql程序。

每个控制节点应该有：

- 2个CPU，至少每个CPU 6个物理核心
- 64GB 内存推荐（1000+ VM）；24GB 最小（注意：为了测试，一个控制节点能运行在只要2GB的内存下，但是生产系统需要很大的内存容量）
- 硬RAID 1 控制 至少1TB的格式化容量作为主操作系统磁盘，更大的磁盘可能需要根据预期的数据库和日志存储要求。请注意，这是频繁在运行控制器节点上扩展磁盘存储。
- 2个网络接口，另外1Gbit/s或者10Gbit/s


## 存储节点（3） ##
我们建议分离 Ceph 节点获得可伸缩性和健壮性。这个硬件的估算要求是每个Ceph-OSD CPU 为5 个内核和每TB Ceph-OSD 空间配置1GB内存。所有Ceph存储和硬盘可以被配置在JBOD模式（只是一堆磁盘）在RAID控制器上，或者可以插入端口免费MB。

生产设施，Ceph的复制因子应设置为3或更多；

- 至少有4个物理核心CPU没插槽
- 24GB内存
- RAID1 控制器至少500GB容量主机操作系统磁盘
- 2个网卡，一个1Gbit/s或者10 Gbit/s
- 18 TB Ceph存储（6×3TB）
- 1-2SSD硬盘，64GB或者更多，为Ceph Journal

计算节点（5）：
虚拟机的主机是计算节点，默认情况下，Fuel配置扩展，如果你不知道你的将来的vm的工作负载的话，设置为1：1的CPU

每个控制节点应该有：

- Dual-socket CPU with at least 4 physical cores per socket
- 64GB RAM
- RAID1 Controller with at least 500GB capacity for the Host operating system disk
- 2 NICs, either 1 Gbit/s or 10 Gbit/s

