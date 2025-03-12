# DMIT 美国洛杉矶 CN2 GIA VPS 测评

本次测评针对 DMIT 的美国洛杉矶 Premium Secure 套餐（sPro.CREATOR），其主要特色是整合了 Cloudflare Magic Transit（CFMT），配备全球 5T 高防御流量。无论是对速度还是安全需求较高的用户来说，都是一项令人瞩目的选择。

👉 [【推荐收藏】2025年 DMIT 最新优惠活动整理汇总 - 每日更新可用优惠套餐](https://bit.ly/dmit_coupon)

> **关于 DMIT**  
> DMIT 成立于 2018 年，由美籍华人创办，拥有 ASN 网络号 AS906/AS54574。主营香港、中国大陆、美国洛杉矶、日本东京的独立服务器及 KVM VPS 服务，也是搬瓦工（Bandwagonhost）部分机房的上游服务商。技术实力可靠，承诺不超售，支持支付宝、微信、PayPal 的多样化付款方式，提供中文客服服务。

## TCP 路由测试

DMIT 的 Premium 套餐采用了以下网络优化配置：

- **Premium 套餐**：去程 China Telecom 和 China Unicom 使用 CN2 GIA，China Mobile 使用 CMI，回程全网 CN2 GIA。
- **Premium Secure 套餐**：去程通过 Cloudflare Magic Transit，回程采用三网 CN2 GIA。尽管服务器物理位置在美国，打开站点的速度依然表现出色。

示例路由测试（部分）：

### 厦门电信

traceroute to 117.28.254.129 (117.28.254.129), 30 hops max, 32 byte packets
 1  193.41.248.72  0.34 ms  AS54574  美国, 洛杉矶
 2  199.245.24.252  1.72 ms  AS2914  美国, 洛杉矶
...
15  117.28.254.129  178.47 ms  AS4809  中国, 福建, 厦门, 电信


### 成都联通

traceroute to 119.6.6.6 (119.6.6.6), 30 hops max, 32 byte packets
 1  193.41.248.72  2.02 ms  AS54574  美国, 洛杉矶
...
11  119.6.6.6  183.99 ms  AS4837  中国, 四川, 成都, 联通


### 上海移动

traceroute to 120.204.197.126 (120.204.197.126), 30 hops max, 32 byte packets
 1  193.41.248.72  18.27 ms  AS54574  美国, 洛杉矶
...
13  120.204.197.126  166.87 ms  AS9808  中国, 上海, 移动


## Superbench 性能测试

DMIT 的服务器性能也颇具优势，以下使用 Superbench 测试的结果：


CPU Model            : AMD EPYC 7402P 24-Core Processor
CPU Cores            : 2 Cores @ 2794.748 MHz
Total RAM            : 732 MB / 1994 MB
Disk I/O Speed       : 平均 739.7 MB/s
Kernel Version       : 4.19.0-16-amd64
Uptime               : 115 天 13 小时


高性能的 AMD EPYC CPU 强化了卓越的 I/O 性能，在响应速度和整体稳定性上表现出色。

## 国际测速（单线程）

测试服务器为 sPro.CREATOR 套餐（带宽 100 Mbps），部分测速结果如下：


Linode, Tokyo, JP             : 10.39 MiB/s | 83.08 Mbps
SoftLayer, Singapore, SG      :  9.08 MiB/s | 72.63 Mbps
Linode, London, UK            :  9.93 MiB/s | 79.44 Mbps
DO, Toronto, CA               : 10.45 MiB/s | 83.59 Mbps


无论是亚洲、北美还是欧洲地区，网络表现均十分稳定，带宽利用率优秀。

## 流媒体解锁能力

作为落地服务器，DMIT 的流媒体解锁能力优势明显，大部分主流平台均支持：

- **Netflix**：支持完整解锁（地区：美国）。
- **Disney+**：部分地区支持。
- **HBO Max**、**Amazon Prime Video** 等：均表现良好。
- **中国地区平台**：支持如 TVBAnywhere+ 等。

> 注意：IPv6 解锁部分平台功能尚存在限制。

## DMIT 套餐推荐

DMIT 提供多种套餐，以下是部分推荐选项：

- **PVM.LAX.Pro.TINY**  
  - 配置：1 核 AMD EPYC, 1G 内存, 10G SSD 存储
  - 流量：650GB/月, 带宽：500Mbps
  - 价格：$28.88/季 | $88.88/年

- **PVM.LAX.Pro.MINI**  
  - 配置：2 核 AMD EPYC, 2G 内存, 20G SSD 存储
  - 流量：4TB/月, 带宽：2Gbps
  - 价格：$58.88/月

- **PVM.LAX.sPro.CREATOR**（带高防）  
  - 配置：2 核 AMD EPYC, 2G 内存, 20G SSD 存储
  - 流量：1000GB/月, 带宽：100Mbps
  - **全球 5T 高防**  
  - 价格：$71.99/季 | $259.99/年

## 测评总结

- **Premium 套餐**（PVM.LAX.Pro）：双向 CN2 GIA 路由，延迟较低，非常适合流量密集型业务或网站建设。
- **Premium Secure 套餐**（PVM.LAX.sPro）：集成 CFMT 和高防御能力，更适用于对安全性要求较高的网站或业务部署。

无论是优化的网络路由，还是灵活的套餐选择，DMIT 的洛杉矶 VPS 都是追求高性能和稳定网络的优质选择。