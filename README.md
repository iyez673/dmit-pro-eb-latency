# dmit速度到底快在哪：Pro 和 EB 差多少？香港 39ms、洛杉矶单核 1728 值不值这个价（附超量降速档位与全套餐对比）

DMIT 的速度口碑，能落到两个具体数字上：香港节点国内访问平均延迟约 39ms，网络稳定、基本不丢包；洛杉矶 Pro 套餐 Geekbench 6 单核跑分 1728，比不少双核 VPS 还高。支撑这两项的是 Pro 系列的三网 CN2 GIA 线路，以及严格控制用户数、不超售的做法，晚高峰才没有明显降速。

但“快”只是决策的一半。这篇文章还会讲清三件容易被含糊过去的事：流量跑完之后速度掉到多少、同样标 1TB 为什么有人半个月就见底、Pro 比 EB 贵出的那部分钱在什么场景下才值。DMIT 2017 年成立，产品线分 Premium（Pro）、Eyeball（EB）、Tier 1（T1）三档，速度这件事只在前两档上成立，第三档是另一套逻辑。

## 先给三档选购建议

> **国内访问速度优先、预算能上**：LAX.Pro 或 HKG.Pro，三网 CN2 GIA，晚高峰表现最稳。
> **联通、移动为主、想省钱**：LAX.EB，回程走 CMIN2 或 9929，同价位给的流量比 Pro 多。
> **面向海外用户或只做国际业务**：T1 系列，国内访问不做优化，但超量后仍保留 50–1000Mbps。

价格和库存变动频繁，实时报价以结账页为准：👉 [查看 DMIT 全部套餐与当前价格](https://www.dmit.io/aff.php?aff=9081)

## 全套餐对比

下表按官网月付基准整理，同一机型偶尔会有限量年付款（MALIBU、WEE 这类命名）不定期补货，是否在售看官网库存；所有价格下单前请以结账页显示为准。

**洛杉矶 LAX.Pro（三网 CN2 GIA）**

| 套餐 | CPU·内存·硬盘 | 流量 @ 带宽 | 月付 | 购买 |
| --- | --- | --- | --- | --- |
| TINY | 1C / 2G / 20GB | 1000GB @ 1Gbps | $9.99 | [ 查看 TINY](https://www.dmit.io/aff.php?aff=9081) |
| Pocket | 2C / 2G / 40GB | 1500GB @ 4Gbps | $14.90 | [ 查看 Pocket](https://www.dmit.io/aff.php?aff=9081) |
| STARTER | 2C / 2G / 80GB | 3000GB @ 10Gbps | $29.90 | [ 查看 STARTER](https://www.dmit.io/aff.php?aff=9081) |
| MINI | 4C / 4G / 80GB | 5000GB @ 10Gbps | $58.88 | [ 查看 MINI](https://www.dmit.io/aff.php?aff=9081) |
| MICRO | 4C / 4G / 160GB | 7000GB @ 10Gbps | $74.99 | [ 查看 MICRO](https://www.dmit.io/aff.php?aff=9081) |
| MEDIUM | 6C / 8G / 160GB | 14000GB @ 10Gbps | $168.88 | [ 查看 MEDIUM](https://www.dmit.io/aff.php?aff=9081) |
| LARGE | 8C / 16G / 320GB | 25000GB @ 10Gbps | $338.88 | [ 查看 LARGE](https://www.dmit.io/aff.php?aff=9081) |
| GIANT | 12C / 24G / 640GB | 50000GB @ 10Gbps | $619.99 | [ 查看 GIANT](https://www.dmit.io/aff.php?aff=9081) |

**洛杉矶 LAX.EB（回程 CMIN2 / 9929）**

| 套餐 | CPU·内存·硬盘 | 流量 @ 带宽 | 月付 | 购买 |
| --- | --- | --- | --- | --- |
| TINY | 1C / 2G / 20GB | 1500GB @ 2Gbps | $9.99 | [ 查看 EB TINY](https://www.dmit.io/aff.php?aff=9081) |
| Pocket | 2C / 2G / 40GB | 3000GB @ 4Gbps | $14.90 | [ 查看 EB Pocket](https://www.dmit.io/aff.php?aff=9081) |
| STARTER | 2C / 2G / 80GB | 5000GB @ 10Gbps | $29.90 | [ 查看 EB STARTER](https://www.dmit.io/aff.php?aff=9081) |
| MINI | 4C / 4G / 80GB | 10000GB @ 10Gbps | $58.88 | [ 查看 EB MINI](https://www.dmit.io/aff.php?aff=9081) |
| MICRO | 4C / 4G / 160GB | 14000GB @ 10Gbps | $74.99 | [ 查看 EB MICRO](https://www.dmit.io/aff.php?aff=9081) |
| MEDIUM | 6C / 8G / 160GB | 30000GB @ 10Gbps | $168.88 | [ 查看 EB MEDIUM](https://www.dmit.io/aff.php?aff=9081) |
| LARGE | 8C / 16G / 320GB | 50000GB @ 10Gbps | $338.88 | [ 查看 EB LARGE](https://www.dmit.io/aff.php?aff=9081) |
| GIANT | 12C / 24G / 640GB | 100000GB @ 10Gbps | $619.99 | [ 查看 EB GIANT](https://www.dmit.io/aff.php?aff=9081) |

同价位对比很直观：TINY 档 Pro 和 EB 都是 $9.99，EB 给 1500GB@2Gbps，Pro 给 1000GB@1Gbps。Pro 贵在线路，不贵在配置。

**香港 HKG.Pro（电信双向 CN2 GIA，移动联通直连）**

| 套餐 | CPU·内存·硬盘 | 流量 @ 带宽 | 月付 | 购买 |
| --- | --- | --- | --- | --- |
| TINY | 1C / 1G / 20GB | 400GB @ 1Gbps | $39.90 | [ 查看 HKG TINY](https://www.dmit.io/aff.php?aff=9081) |
| STARTER | 1C / 2G / 30GB | 800GB @ 2Gbps | $74.99 | [ 查看 HKG STARTER](https://www.dmit.io/aff.php?aff=9081) |
| MINI | 2C / 2G / 40GB | 1000GB @ 2Gbps | $99.00 | [ 查看 HKG MINI](https://www.dmit.io/aff.php?aff=9081) |

**T1 系列（国际线路，三地配置档位多，完整参数以官网为准）**

| 机房 | 套餐 | 超量后限速 | 参考价格 | 购买 |
| --- | --- | --- | --- | --- |
| 香港 | HKG.T1.WEE | 50Mbps | 约 $9.9/月（年付） | [ 查看 HKG T1](https://www.dmit.io/aff.php?aff=9081) |
| 东京 | TYO.T1.WEE | 50Mbps | 约 $9.9/月（年付） | [ 查看 TYO T1](https://www.dmit.io/aff.php?aff=9081) |
| 洛杉矶 | LAX.T1.WEE | 100Mbps | 年付 $36.9 | [ 查看 LAX T1](https://www.dmit.io/aff.php?aff=9081) |
| 三地 | TINY 及以上 | 100–1000Mbps | 按机房与配置浮动 | [ 查看全部 T1 套餐](https://www.dmit.io/aff.php?aff=9081) |

## 速度从哪来：三条线路三种命

Pro 系列三网 CN2 GIA，这是 DMIT 速度口碑的全部来源。香港机房电信双向 CN2 GIA，移动联通直连；洛杉矶机房电信联通去程 CN2 GIA、移动去程 CMI、三网回程 CN2 GIA；东京机房做三网高速优化。三条路径里，回程走 CN2 GIA 对国内访问体感影响最大，晚上八九点跨境链路最拥堵的时段，差距就出在这里。

EB 系列回程换成三网 CMIN2 或 9929，价格低一档，速度在联通、移动网络下体感接近 Pro，电信用户能感觉到区别。需要留意的是，非 Pro 产品可能因网络攻击或成本原因切换路由，如果高端线路是刚需，直接买 Pro，别指望 EB 长期稳定在同一套路由上。

T1 走国际线路，不做国内优化。国内访问它不会给你 39ms 这种数字，它的价值在另一头：超量之后还剩很高的带宽，以及面向海外用户的连通性。

物理距离决定了延迟的下限。香港离大陆最近，39ms 是地理优势加线路优化的结果；洛杉矶跨太平洋，光信号往返就要一百多毫秒，再优化也追不上香港；东京在两者之间，面向亚太用户更合适。

## 三个机房怎么选

**香港**延迟最低，代价是流量小、单价高。HKG.Pro.TINY 月付 $39.90 只给 400GB 流量，Pro 系列又是双向计费，跑代理类应用实际可用约 200GB。适合远程办公、轻量 API、对响应时间极敏感但流量需求不大的场景。拿它跑大流量业务，账单会很难看。

**洛杉矶**档位最全，8 档配置从 1C2G 铺到 12C24G，流量从 1TB 到 50TB，绝大多数人在这里能选到合适的型号，也是 Pro 与 EB 差价最值得算一算的机房。

**东京**面向亚太用户。国内访问比洛杉矶好、比香港差，适合访客主要在日本、韩国、东南亚的业务。

想确认哪个机房当前有货：👉 [查看三地机房实时库存](https://www.dmit.io/aff.php?aff=9081)

## 流量跑完之后，速度还剩多少

这是 Pro 和 T1 差距最大的地方，也是买之前最该算清楚的一项。2025 年 2 月 18 日起，超量降速不停机正式覆盖洛杉矶 LAX Pro 与 EB 系列，T1 后续跟进，限速上限经过多次提升。

| 系列 | 套餐档位 | 超量后限速 |
| --- | --- | --- |
| LAX.Pro / LAX.EB | WEE、MALIBU、INTRO、CORONA | 2Mbps |
| LAX.Pro / LAX.EB | TINY、Pocket、STARTER、PalmSpring、Irvine、FONTANA | 4Mbps |
| LAX.Pro / LAX.EB | MINI、MICRO | 8Mbps |
| LAX.Pro / LAX.EB | MEDIUM、LARGE、GIANT | 10Mbps |
| T1 | HKG / TYO 的 WEE | 50Mbps |
| T1 | HKG / TYO 的 TINY、STARTER、MINI；LAX 的 WEE | 100Mbps |
| T1 | HKG / TYO 的 MICRO、MEDIUM；LAX 的 TINY、STARTER、MINI | 200Mbps |
| T1 | HKG / TYO 的 LARGE；LAX 的 MICRO、MEDIUM、LARGE | 500Mbps |
| T1 | 三地 GIANT | 1Gbps |

Pro 和 EB 的入门款超量后掉到 2–4Mbps，这个速度够 SSH 登录、改配置、传几个小文件，撑不起正常业务。8–10Mbps 能带一个轻量站点，访问会慢但不会打不开。T1 的入门款超量后还有 50–100Mbps，跑轻站、同步数据基本无感，这个“降速”比很多商家的正常速度还快。

流量超了之后有四条路：等下个账单周期自动重置；提工单升级套餐，按差价折算；在控制面板里先切到“超量停机”再切回“超量降速”，用来触发新的限速档位；或者干脆切回超量停机模式。

## 流量怎么算才不踩坑

Pro 和 EB 双向计流量，入站出站都算；T1 单向取最大值，也就是 MAX（入站，出站）。同样标 1TB，Pro 实际能跑的量只有 T1 的一半左右。

跑代理类应用时这个差别被放大：上行下行同时计费，标称 1TB 的套餐实际可用约 500GB，月中就见底并不奇怪。买 EB 大流量款之前先按这个口径折算一遍，别按标称数字做容量规划。

流量按账单周期重置，从购买日起算，不是自然月 1 号。重置后自动恢复满速，不需要手动操作。月初买和月末买，重置日期不一样，转移大流量之前先看一眼自己的周期。

## 硬件平台和滚动升级

DMIT 把硬件平台分成 Next、Stable、LTS 三级。2024 年 10 月洛杉矶产品做过一次全面升级，宿主机从第二代、第三代 AMD EPYC 换到第四代 EPYC 9654，存储和套餐流量同步加大，存量用户免费同步升级。洛杉矶目前已经部署 AMD EPYC 9005，香港与东京计划在 2026 年第二季度升级，这一条是计划口径，落地情况以官网为准。

滚动升级的机制是：Next 平台换新之后，原来的硬件下放到 Stable 平台。所以买到的不是最新配置，也不代表会一直用旧硬件，这套机制下存在免费升上来的可能。洛杉矶 Pro 单核 1728 这个跑分就是这么来的，CPU 不是这套方案的瓶颈，速度差异基本都由线路决定。

## 下单前必须知道的六件事

1. 只有 Linux，没有 Windows VPS。
2. 强制 SSH 密钥登录，不支持 root 密码，首次购买后要在后台下载密钥文件。
3. IP 被墙可以免费更换，规则是每 15 天一次；其他情况 $5 一次。
4. 非 Pro 产品可能因攻击或成本原因切换路由。
5. 硬件升级维护时可能不提前发邮件通知，跑高稳定性业务要考虑这一点。
6. 提供原生 IP，YouTube Premium 等多数能解锁，Netflix 和 Disney+ 不保证 100%，主要看流媒体的话，下单前先问客服确认当前 IP 段。

## 退款、付款与试错成本

3 天内无理由全额退款，条件是使用流量少于 30GB；30 天内按剩余价值退款。可以退到账户余额，也可以原路退回，原路退会扣支付渠道的手续费。付款支持支付宝、微信、PayPal 和信用卡，客服能中文沟通，工单一般 6 小时内回复。

退款窗口只有 3 天，拿到机器当天就该测延迟和路由，别等到第五天才想起来。想先小额试一台：👉 [开通月付套餐，3 天内可全额退](https://www.dmit.io/aff.php?aff=9081)

## 常见问题

**流量超了会自动停机吗？**
LAX Pro、LAX EB 和全系 T1 都是降速不停机，服务保持在线。控制面板里可以手动切回停机模式。

**下个账单周期会自动恢复速度吗？**
会。流量按账单周期重置，重置后自动恢复满速，不用提交工单。

**为什么流量掉得比想象中快？**
Pro 和 EB 双向计费，跑代理类应用上下行都计入，标称 1TB 实际可用约 500GB。T1 单向取最大值，同样标称数字下更耐用。

**Pro 和 EB 差在哪，多花的钱值不值？**
差在线路。Pro 三网 CN2 GIA，EB 回程 CMIN2 或 9929。联通、移动用户日常体感差距不算大；电信用户、以及对晚高峰敏感的业务，Pro 的溢价才花得值。只做海外访问的话，两者都不必买，直接看 T1。

**网上那些优惠码还能用吗？**
流传的码前缀大多是 2025，距现在超过一年，是否仍有效只能在结账页填一次看结果。本文不承诺任何折扣力度，也不保证叠加规则。

## 按你的情况对号入座

只需要国内访问快、预算能上：LAX.Pro 或 HKG.Pro，机房按访客位置定，南方和华南偏多选香港，全国铺开选洛杉矶。

联通移动为主、想省钱：LAX.EB。同价位配置和流量都比 Pro 高一档，代价是路由稳定性略差。

面向海外用户、流量波动大：T1。超量后还有 50Mbps 起步，比 Pro 入门款的 2Mbps 更能兜底。

下单前确认两件事：目标套餐当前有没有库存，热门款经常缺货；当前优惠在结账页是否仍然生效，别按旧文章里的折扣做预算。

👉 [去 DMIT 看今天哪些套餐有货](https://www.dmit.io/aff.php?aff=9081)
