# 使用IP时间戳远程识别虚拟机
## 概要
In this paper, we present a remote detection technique for VM that uses IP timestamp option in full virtualization that could be used to detect VM environment and contributing to VM vulnerability。

IP timestamp option allows a requester to request
timestamps value from any machine which handles
packets by specifying its IP address
这是本文作者的一个联系性工作，本文聚焦于使用网络时间戳测试远程虚拟机（全虚拟化）检测方法
之前的工作是研究半虚拟化和非虚拟机的时间戳不同。

## 背景
虚拟化分类
安全问题：
## 相关工作


在以往的研究中，其中一种方法检测 VM 内的执行，通常有专注于实现的特定工件，例如硬件命名、**guest-to-host通信系统**或内存地址

可参考
Functional and transparency detection method was discussed in (Ferrie, P., 2007; Garfinkel, T., et al., 2007) by highlighting detection strategies that look upon the characteristic of logical discrepancies, resource discrepancies and timing discrepancies between VM and non-VM environment
逻辑差异、资源差异和时序差异的特征
Detection method that focuses on differences in performance between VM and physical hardware were also discussed.  as machines that are being used to host the VM are continuously improved, the
difference according to performance might be different and more tests need to be done constantly to verify current situation   用性能差异检测并不靠谱

A light weight detection method of Virtual Machine Monitor using CPU instruction execution performance stability had been studied in (K. Miyamoto, et al., 2011) CPU指令性能检测方法轻量化，

聚焦在网络实现和虚拟机表现的方法可以考虑作为远程虚拟机检测的方法，该方法不会compromise目标

Method that using network timestamps was first exploited by (Kohno, T., et al.,2005) using TCP timestamps as a convert channel to reveal a target host’s physical clock skew, which uniquely identifies a physical machine

使用时间戳的方法由2005年提出检测主机物理时钟偏差

通过诸如网络时间协议 (NTP) 之类的机制，计算机可以保持准确的当前时间，并校准到秒的几分之一。网络时间戳存在于各种网络协议中，例如 Internet 协议 (IP) 和 Internet 控制消息协议 (ICMP)

IP设计用于分组交换计算机通信网络的互连系统。 它提供了将称为数据图的数据块从源传输到目的地的信息，其中源和目的地由固定长度地址标识  
IP时间戳(Mills, 1992)是对IP报头的可选扩展。它允许发送方通过指定时间戳值，向任何处理数据包的机器请求时间戳值
IP地址

使用ESXi和 VirtualBox