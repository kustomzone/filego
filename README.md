# FilEgo - A decentralized storage platform

* ``Version: 1.0``
* ``Author: Eximua Labs``
* ``Email: xieyang@dodora.cn``
* ``Date: July 22, 2018``

## 摘要

FilEgo是一个去中心化存储平台，我们通过IPFS技术连接世界范围内的空闲存储设备，同时利用区块链为设备提供方（以下简称矿工）、用户和开发者提供经济价值。

使用FilEgo能使存储市场在没有中介的情况下运营。与传统云存储厂商相比，我们通过智能合约保障存储交易，提供了稳定、安全且便宜的硬盘空间租赁方案，保证每一个人都能买得起。并且，没有任何一方能审查FilEgo上的内容，FilEgo将真正做到**自己的数据归自己**。

无论是个人还是企业，都可以以矿工或用户的身份融入FilEgo的生态圈，生态圈内的所有交易都使用EgoCoin。

FilEgo是由``File``和``Ego``两个单词组成的合成词，``Ego``的中文翻译是``自我意识``，我们的目标是让存储在FilEgo之上的文件拥有充分的``自我意识``，从而确保文件的自主权。

长期目标是希望能够成为下一代互联网存储方案的基础设施。

## 详细介绍

传统云存储厂商（七牛云、百度云盘等）都是大型第三方机构，这种系统易受各种安全威胁，如中间人攻击、应用程序漏洞等。此外，由于托管在第三方服务器上，一旦受到攻击，容易暴露消费者隐私和企业私密数据。而且，大多存储服务依赖于相同的基础设施，一旦发生故障，往往波及范围广。另外一个潜在的威胁是监管，第三方服务往往会在上传时审查你的内容并过滤掉一些他们认为的“非法内容”，从而对用户、企业和社会的权益造成侵犯。

与之相比，去中心化存储平台则具有很大优势。首先，数据安全使用客户端加密来保证，数据完整性使用可检索证明来维护。同时，P2P（Peer-to-Peer）的冗余存储特性，可以大大降低基础设施故障带来的文件丢失问题。每个人都可以参与的自由存储市场，也将降低普通用户的存储成本。使用IPFS的版本控制系统（Version Control），可以记录文件的每一个版本，从而抵制审查、篡改和侵权等问题。

本文详述了包含去中心化存储和加密货币一套系统的实现方案。

## 基本架构

FilEgo包含三方面的基础架构：

1. 服务端及其生态（矿工、开发者）
2. 客户端及其生态（普通用户、开发者）
3. 加密货币（EgoCoin）

### 服务端及其生态

服务端主要给矿工和开发者使用，目标是零成本启动成为FilEgo网络中的一个节点，并为用户提供租赁服务。

此外，为开发者提供服务的相关软件开发包（SDK, Software Development Kit）也包含在这其中。

EgoCoin的部分组件也会在服务端中有所体现，如``文件可检索证明``、``网络稳定性证明``等。

### 客户端及其生态

客户端主要给普通用户和开发者使用，主要目标是使用户能方便的管理自己的文件，包括但不限于存储、上传、下载和分享。次要目标是使开发者能利用应用程序编程接口（API, Application Programming Interface）方便的集成自己的服务。

EgoCoin的部分组件也会在客户端中有所体现，如``区块浏览器``等。

### EgoCoin加密货币

EgoCoin加密货币将作为FilEgo网络内的交易货币。矿工提供设备并被系统证明可用后将会获得相应的EgoCoin作为奖励；用户可支付法币或EgoCoin进行租赁，若支付法币则兑换成当前EgoCoin的价格，然后系统再使用EgoCoin进行支付，支付完成后该EgoCoin将按比例（系统将根据存储容量、下行容量、上行容量、稳定性等参数对矿工进行评分）分发给所有矿工。

### 为什么FilEgo需要加密货币

为什么需要加密货币则需要从“加密货币”的本质说起。ICO（首次币发行）这种创新的方式，让每一家中小企业或个人都拥有了在市场上募集资本的权利，这种权利不再归属于已经成熟并且拥有稳定现金流的公司。通过加密货币这种成本稍低的方式，可以很快的帮助一个初创项目获得起始资本从而快速推动产品发展，这种方式比现今流行的种子轮、天使轮、A轮更加激进有效。但是，我们应该避免市面上的空气币。如果你是因为加密货币背后的产品、技术、团队和愿景而投资，那么你就不是被割的韭菜或投机者，而是真正的**价值投资者**。

小米上市时，圈内人盛传“小米的股票值得长期持有”。那么FilEgo也希望某一天圈内的人也能说“EgoCoin值得长期持有”，此时，对FilEgo、矿工和用户是一个三方共赢的局面。

这就是FilEgo需要加密货币的原因。

## 设计方案

### 身份认证

### 网络

### 数据安全

### 服务端

### 客户端

### EgoCoin介绍

### 应用场景

## 未来展望
