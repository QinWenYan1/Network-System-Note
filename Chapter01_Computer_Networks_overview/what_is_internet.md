# 📘 1.1 什么是 Internet (What is the Internet)

> 来源说明：计算机网络（自顶向下方法）第1章 | 本节涵盖：Internet的具体构成、服务角度定义、协议概念

---

## 🧠 核心概念总览（严格按原文顺序）

- [*知识点1: 具体构成角度定义internet*](#id1)
- [*知识点2: 具体构成角度定义internet: 数以亿计的互联计算设备*](#id2)
- [*知识点3: 协议(Protocol)的定义*](#id3)
- [*知识点4: 服务角度定义internet*](#id4)
- [*知识点5: 网络结构总览*](#id5)

---

<a id="id1"></a>
## ✅ 知识点1: 具体构成角度定义internet

**理论**

Internet从具体构成角度来看，包含以下核心组件：

- **节点(Node)**
  - **主机(Host)**及其上运行的**应用程序(Application)**
  - **路由器(Router)**、<b>交换机(Switch)</b>等网络交换设备

- **边(Edge)**：通信链路(Communication Link)
  - **接入网链路(Access network links)**：主机连接到互联网的链路
  - **主干链路(Backbone links)**：路由器间的链路

- **协议(Protocol)**
  - 对等层实体(Peer entities)在通信过程中应当遵守的规则集合

💡 **理解技巧**：把Internet想象成一个巨大的图(Graph)，主机和路由器是节点，通信链路是连接节点的边。

📋 **术语提醒**：
- 主机(Host) = 端系统(End System)
- 路由器(Router) 工作在网络层，交换机(Switch)工作在数据链路层

---

<a id="id2"></a>
## ✅ 知识点2: 具体构成角度定义internet: 数以亿计的互联计算设备

**理论**

- **数以亿计的、互联的计算设备**
  - 主机(Host) = **端系统(End System)**
  - 运行网络应用程序（如Web、email等）

- **通信链路(Communication links)**
  - 类型：**光纤(Fiber optic)**、**同轴电缆(Coaxial cable)**、**无线电(Radio)**、**卫星(Satellite)**
  - **传输速率(Transmission rate)** = **带宽(Bandwidth)**，单位是 **bps(bits per second)**

- **分组交换设备(Packet switching devices)**
  - 功能：转发**分组(Packets)**
  - 设备：**路由器(Router)** 和 **交换机(Switch)**

- **Internet："网络的网络"(Network of networks)**
  - 松散的层次结构，互连的ISP
  - **公共Internet(Public Internet)** vs **专用Intranet**

- **Internet标准(Internet Standards)**
  - **RFC(Request for Comments)**：请求评论，技术规范文档
  - **IETF(Internet Engineering Task Force)**：互联网工程任务组

⚠️ **注意**：Internet不是单一的网络，而是由无数个网络互联而成的"网络的网络"。

---

<a id="id3"></a>
## ✅ 知识点3: 协议(Protocol)的定义

**理论**

- **人类协议(Human protocols)** 类比
  - "几点了？" "我有个问题" "你好"
  - 类似人类协议，但机器之间的协议而非人与人

- **网络协议(Network protocols)**
  - 控制发送、接收消息
  - 如 **TCP**、**IP**、**HTTP**、**FTP**、**PPP**

- **协议定义**
  > 协议定义了两个或多个通信实体之间交换的**报文格式(Message format)**和**次序(Order)**，以及在报文传输和/或接收或其他事件方面所采取的**动作(Actions)**。

- **协议三要素**
  1. **语法(Syntax)**：报文的结构和格式
  2. **语义(Semantics)**：需要发出的控制信息及完成的动作
  3. **时序(Timing)**：事件实现的顺序和速度匹配

⚠️ **警告注意**：Internet中所有的通信行为都受协议制约！没有协议就没有Internet。

💡 **理解技巧**：协议就像交通规则，规定了数据如何在网络中"行驶"，确保不会"撞车"。

---

<a id="id4"></a>
## ✅ 知识点4: 服务角度定义internet

**理论**

从服务角度来看，Internet提供：

- **分布式应用(Distributed applications)**
  - 使用通信设施进行通信的分布式应用
  - **网络存在的理由**！
  - 包括：**Web**、**VoIP**、**email**、**分布式游戏(Distributed games)**、**电子商务(E-commerce)**、**社交网络(Social networks)**

- **通信基础设施(Communication infrastructure)**
  - 为应用程序提供**编程接口(Programming Interface)**（通信服务）
  - 将发送和接收数据的apps与互联网连接起来

- **服务类型**
  - **无连接不可靠服务(Connectionless, unreliable service)**：如UDP
  - **面向连接的可靠服务(Connection-oriented, reliable service)**：如TCP

💡 **理解技巧**：把Internet想象成邮政系统，应用程序是寄件人和收件人，Internet提供寄送服务（可靠或不可靠）。

📋 **术语提醒**：
- **VoIP(Voice over IP)**：IP电话/网络语音通话
- **API(Application Programming Interface)**：应用程序编程接口

---

<a id="id5"></a>
## ✅ 知识点5: 网络结构总览

**理论**

网络结构分为三个主要部分：

| 部分 | 组成 | 说明 |
|------|------|------|
| **网络边缘(Network Edge)** | 主机(Hosts)、应用程序（客户端和服务器） | 端系统所在的位置 |
| **网络核心(Network Core)** | 互连的路由器、网络的网络 | 数据传输的骨干 |
| **接入网和物理媒体(Access networks, Physical media)** | 有线或无线通信链路 | 连接边缘和核心 |

🔄 **知识关联**：
- 第1.2节将详细讲解网络边缘
- 第1.3节将详细讲解网络核心
- 第1.4节将详细讲解接入网和物理媒体

---

## 🔑 核心要点总结

1. **Internet的双重定义**：从构成角度（节点+链路+协议）和服务角度（分布式应用的基础设施）

2. **协议三要素**：语法、语义、时序，是通信的"交通规则"

3. **Internet的本质**："网络的网络"，由无数ISP互联而成

4. **Internet标准**：RFC文档由IETF发布，是技术实现的权威依据

5. **两种服务模式**：面向连接的可靠服务 vs 无连接不可靠服务

---

## 📌 考试速记版

### 关键术语对照
| 中文 | 英文 | 含义 |
|------|------|------|
| 主机 | Host / End System | 运行应用的端系统 |
| 路由器 | Router | 网络层分组转发设备 |
| 交换机 | Switch | 链路层分组转发设备 |
| 协议 | Protocol | 通信规则集合 |
| 带宽 | Bandwidth | 链路传输速率(bps) |
| 分组 | Packet | 数据传输单元 |
| RFC | Request for Comments | 互联网标准文档 |
| IETF | Internet Engineering Task Force | 互联网工程任务组 |

### 易混淆概念
- **主机 vs 路由器**：主机运行应用，路由器转发分组
- **公共Internet vs Intranet**：前者公开可访问，后者私有专用

**记忆口诀**：
> "节点链路加协议，网络构成三要素；服务角度看应用，基础设施连万物。"
