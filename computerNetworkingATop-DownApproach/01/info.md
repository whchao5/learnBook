
#### 1.2接入网
家庭电话线同时承载数据和传统的电话信号，编码为不同的频率:
* 高速下行信道，位于50kHz 到 1MHz 频段
* 中数上行信道，4KHz 到 50KHz频段;
* 普通的双向电话信道，位于0到4KHz 频段


#### 1.4 分组交换网中的延迟、对包和吞吐量

Linux `Traceroute` 软件查看 网络信息 [Traceroute](http://traceroute.org) ;  windows `Tracert` 软件,直接运行命, 格式 tracert www.csdn.net

#### 1.5 协议层次及其服务模型
1 协议分层
 * 应用层 ：协议有 http, https(请求和传输), SMTP(电子邮件) -> 信息分组称为 ``报文``
 * 运输层 :  两个运输协议，即 TCP 和 UDP, 利用其中任何一个都能运输应用层的报文, `TCP` 向应用层提供了面向链接的服务，能确保 传递和流量控制，`UDP` 是提供无连接服务 运输分组称为 ``报文段``
 * 网络层 ： ``数据报`` ，包括 IP 协议
 * 链路层 ：链路层分组 称为 ``帧``
 * 物理层 ：将 ``帧`` 中的 一个一个 ``比特`` 从一个节点移到下一个节点

 2 OSI 模型 </br>
 7 层协议 ： 应用层, 表示层，会话层，运输层，网络层，链路层，物理层。 因特网缺少 表示层，会话 层


| 因特网 五层协议 | | OSI 模型 |
|:-------:| ---| :----:|
|    应用层 | | 应用层|
| 运输层 | |  **表示层**|
| 网络层 | | **会话层**|
| 链路层 | | 运输层|
| 物理层 | | 网络层|
| |  | 链路层|
| | | 物理层|