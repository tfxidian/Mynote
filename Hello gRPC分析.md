# Hello gRPC 分析

一开始我是希望有一个简单的示例来让我快速上手，然后我按照官方的教程搭建了环境，并且成功运行了一个helloworld程序[grpc hello world](https://github.com/tfxidian/go-tutorial/tree/main/grpc_class),然而对其中的实现依然是很模糊。还是要参考更多的文章和源码来理解，下面就来记录这个过程。

## gRPC介绍

RPC（远程过程调用）是一个计算机通信协议。该协议允许运行于一台计算机的程序调用另一个地址空间（通常为一个开放网络的一台计算机）的子程序，而程序员就像调用本地程序一样，无需额外地为这个交互作用编程（无需关注细节）。
参考链接

gRPC是一个现代开源的远程过程调用框架，它可以在任何地方运行。
它使客户机和服务器应用程序能够透明地通信，并使构建连接的系统变得更容易。

## 为什么使用gRPC
- 低延迟、高可扩展性、分布式系统。
- 开发与云服务器通信的移动客户端
- 设计一个新的协议，需要准确、高效和独立于语言
- 分层设计，以支持扩展、身份验证、负载均衡、日志记录和监控等

## 示例学习
这个例子很接地气，能够很方便的了解gRPC的用法，建议学习。
[最简单的 gRPC 教程— 1 初识 gRPC](https://zhuanlan.zhihu.com/p/359968500)

[Linux grpc环境部署](https://github.com/tfxidian/go-tutorial/tree/main/grpc_class)
[gRPC快速入门](https://www.liwenzhou.com/posts/Go/gRPC/)
[最简单的 gRPC 教程— 1 初识 gRPC](https://zhuanlan.zhihu.com/p/359968500)