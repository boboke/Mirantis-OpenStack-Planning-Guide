# Mirantis Openstack 和 Fuel 简介


OpenStack是一个可扩展的，通用的，灵活的云管理平台。这是一个组合的云基础设施服务–计算，存储，网络和其他核心资源，它们之间是通过公开的REST API。它能更大范围的控制这些服务，可以从这两个角度开看，一个是由应用控制的技术架构即服务（IaaS），一个是能够自动化操作的基础架构的一套工具。

Mirantis OpenStack 是一个产品化开放源代码技术，它包含 Fuel 一个帮助你快速部署你的云环境的云图形化 web 工具。Fuel 包含的脚本能大大促进和加速云部署过程，你不需要完全熟悉需要安装OpenStack环境组成的复杂的过程。

本指南提供详细让你开始在一套物理服务器（裸金属安装）上安装Mirantis OpenStack 和 Fuel ，看详细的[用户手册](User Guide)关于怎么下载和在 Fuel 安装主 Fuel 节点和怎么使用 Fule 界面去部署你的 OpenStack 环境。 

进一步阅读以下文件是：

- [术语参考]()是按字母顺序列出的技术和概念，作为一个术语表和主索引中的 Mirantis 文档和开放源代码文件中。
- [操作指南]()提供一些信息在部署 OpenStack 环境之后进一步任务要求维护，大多数任务都是通过文本编辑器和命令行工具来操作完成。
- [参考体系结构]()提供了有关如何执行Mirantis OpenStack及其支持HA架构背景信息。

You have ways to use Mirantis OpenStack and Fuel other than the bare-metal installation:
你有多种方式使用 Mirantis OpenStack and Fuel 对比裸金属安装：

- 你可以安装 Fuel 和使用它去部署 Mirantis OpenStack 环境在 Oracle VirtualBox上。VirtualBox 用于演示并且是一个很好的方式开始你的工具和技术研究，看0 to OpenStack in 60 Minutes or less 入门，其它额外信息在运行Fule 在VirtualBox 注意在VirtualBox上部署不用满足大部分生产环境的性能和健壮性要求
- 你能安装Fuel 主节点在vSphere 和部署 Mirantis OpenStack 环境在vSphere上。 
- Mirantis OpenStack 提供随需而变的，预配置和准备使用托管私有云产品， Mirantis OpenStack Express。

社区成员或合作伙伴将 Fuel 更进一步, 看[开发文档]()获得Fuel内部架构信息，构建项目说明，REST API 之间的相互作用内容和其他感兴趣的主题向更高级的开发者，你也能访问 [Fuel 项目]()更详细的信息并成为贡献者。