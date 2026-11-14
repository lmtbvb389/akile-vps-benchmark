# Akile 评测：¥7.3/月的大带宽 VPS 实际能跑多快？流媒体解锁稳不稳？哪几档套餐值得买（附全套餐价格与优惠码）

Akile（AkileCloud）眼下查得到的最低入门价是 ¥7.3/月，日本 JPHyper-One 番茄特供那一档；香港 HKLite-One 报 ¥8.8/月，香港 HKSM-One、日本 JPIIJ-Lite、新加坡 SGLite-One 都落在 ¥9.99/月附近。这笔钱买到的是每个节点自带的 DNS 流媒体解锁，加上标称 2500M 到 10000M 的带宽数字。要接受的代价同样明确：官方写明不保证大陆直连，标称带宽是共享上限，实际跑多少要看同一台物理机上的邻居。

下面按系列把能查到的在售套餐拆开，给出几份可以对照的实测数据，再说清楚哪一档值得掏钱、哪一档多数人用不上。

> **快速对号入座**
> 只要港区、日区流媒体落地：香港 HKLite-One（¥8.8/月）或日本 JPHyper-One（¥7.3/月），配置够用，别指望直连。
> 要大陆方向低延迟：香港 HKPro，或洛杉矶 LAXPro / LAX Premium 的三网优化档，从几十元到几百元一个月。
> 要原生 IP、家宽属性：洛杉矶 LAX4837 双 ISP 系列，¥54.99/月起。
>
> 👉 [查看 Akile 当前在售套餐与价格](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811)

## 全套餐对比：先看清价格口径

Akile 的套餐名和档位调整比较频繁，同一款产品在不同时间能查到不同配置。下表整理的是第三方推广文与测评站公开记录的口径，价格会随促销变动，下单前请以官网结算页为准。所有套餐均为 KVM 虚拟化（部分节点 Hyper-V），自研控制面板，支持支付宝和微信付款。

### 香港 / 日本 / 新加坡入门档

| 套餐 | 配置 | 带宽 / 月流量 | 参考价格 | 入口 |
| --- | --- | --- | --- | --- |
| HKSM-One | 1 核 / 1GB / 5GB NVMe | 1000M / 1TB | ¥9.99/月 | [ 查看该档价格](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| HKLite-One（番茄特供） | 1 核 / 1GB / 5GB SSD | 5000M / 2TB | ¥8.8/月 | [ 查看该档价格](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| JPHyper-One（番茄特供） | 1 核 / 1GB / 5GB | 2500M / 1TB | ¥7.3/月 | [ 查看该档价格](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| JPIIJ-Lite | 1 核 / 512MB / 5GB | 1000M / 500GB | ¥9.99/月起 | [ 查看该档价格](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| SGLite-One | 1 核 EPYC / 1GB / 5GB NVMe | 500M / 1TB | ¥9.99/月 或 ¥99.99/年 | [ 查看该档价格](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| SGLite-翻倍盲盒 | 1 核 / 256~1024MB / 5~20GB | 600~2400M / 800~3200GB | ¥9.99/月 | [ 查看该档价格](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |

香港 HKLite-One 必须单独说明：2024 年 12 月一份测试记录里的同款套餐，标的是 1 核 / 1024M / 10GB 硬盘 / 10000M 带宽 / 2000G 月流量，售价 **¥150.00/3 年**，并且明确写着 IPv6 为 0 个。这和上表 ¥8.8/月、5GB 硬盘、5000M 的版本是两套配置。买之前在下单页核对硬盘和计费周期，不要拿一个版本的价格去套另一个。

另有一份更新到 2026 年 10 月的第三方整理给出了不同的入门序列：LAXLite-One ¥8.88/月起、SGLite-One ¥10.42/月起、JPHyper-Lite ¥14.99/月、HKLite-Mini ¥24.99/月。档位名称和价格都对不上，说明这段时间产品线做过调整。哪个版本在你下单当天有效，只有结算页能回答。

### 洛杉矶 LAX4837 双 ISP 住宅方案

三网回程走 AS4837，原生 IP，双 ISP 家宽属性，1Gbps 端口。

| 方案 | 配置 | 月流量 | 月付 | 入口 |
| --- | --- | --- | --- | --- |
| ISPMini | 1 核 / 2GB / 10GB | 1TB | ¥54.99 | [ 查看 ISPMini](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| ISPStarter | 2 核 / 2GB / 10GB | 2TB | ¥74.99 | [ 查看 ISPStarter](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| ISPStandard | 4 核 / 4GB / 10GB | 4TB | ¥94.99 | [ 查看 ISPStandard](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| ISPPro | 4 核 / 8GB / 20GB | 8TB | ¥184.99 | [ 查看 ISPPro](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |

### 洛杉矶 LAX Premium 三网双向优化

联通 9929、移动 CMIN2、电信 CN2 GIA，原生 IP。

| 方案 | 配置 | 带宽 / 月流量 | 月付 | 入口 |
| --- | --- | --- | --- | --- |
| Premium-Mini | 1 核 / 1GB / 20GB | 200Mbps / 500GB | ¥79.99 | [ 查看 Premium-Mini](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| Premium-Starter | 2 核 / 2GB / 20GB | 200Mbps / 1TB | ¥149.99 | [ 查看 Premium-Starter](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| Premium-Standard | 4 核 / 4GB / 30GB | 300Mbps / 2TB | ¥289.99 | [ 查看 Premium-Standard](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| Premium-Pro | 4 核 / 8GB / 40GB | 500Mbps / 4TB | ¥569.99 | [ 查看 Premium-Pro](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |

Premium 的端口带宽只有 200Mbps，流量也比同价位产品少，卖点是线路本身。跑流媒体和代理够用，做大流量下载就不划算。

### 洛杉矶 LAXPro 三网优化

同样是 CN2 GIA + 9929 + CMIN2，原生 IP，DNS 流媒体解锁，含 20Gbps 单 IP DDoS 防护。

| 方案 | 配置 | 带宽 / 月流量 | 月付 | 入口 |
| --- | --- | --- | --- | --- |
| LAXPro-Light | 1 核 / 1GB / 20GB | 500Mbps / 300GB | ¥43.74 | [ 查看 LAXPro-Light](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| LAXPro-Standard | 1 核 / 1GB / 20GB | 500Mbps / 1TB | ¥74.99 | [ 查看 LAXPro-Standard](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| LAXPro-Pro | 1 核 / 1GB / 30GB | 500Mbps / 2TB | ¥112.49 | [ 查看 LAXPro-Pro](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| LAXPro-Max | 2 核 / 2GB / 40GB | 500Mbps / 3TB | ¥187.49 | [ 查看 LAXPro-Max](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |

LAXPro-Light 的 ¥43.74 是否为折后价，公开资料没有说明，不要按 8 折或 7 折自行倒推原价。

洛杉矶还有更便宜的入门线。有推广文写“LAX Base ¥9.99/月起（用码 8 折）”，另一份 2026 年的整理写 LAXLite-One ¥8.88/月起。这两档不带三网优化，属于国际线路落地机，和上面三个系列不是一回事。

### 英国与其他地区

英国节点可查到的记录：1 核 / 1GB / 10GB / 1TB 流量 / 500Mbps，约 ¥19.99/月，英国原生 IP，超额限速 10Mbps，重置流量 ¥14。另有一款 UKbgp，1 核 / 512MB / 5GB SSD / 496Mbps，三网回程 9929，年付 ¥127.99，被第三方测评站评为 3.8 星。这两条来自测评摘要，未经官方页面复核，仅作参考。台湾、韩国、德国节点也有在售，配置档位同样以结算页为准。

## 实测数据能说明什么

**香港 HKLite-One，2024 年 12 月融合怪测试。** CPU 是 AMD EPYC 7D12，单核主频 1100MHz，sysbench 单核 **1465 分**。磁盘 fio 4K 随机读写都在 102MB/s 左右（约 25.6k IOPS），1M 块读写 106MB/s，这个 IO 在低价位机型里不算差。流媒体方面 Netflix 港区完整解锁（支持非自制剧）、Disney+ 解锁 HK 区、Amazon Prime Video HK、TVBAnywhere+ 可用、ChatGPT 显示 Yes，Google Gemini 和 Reddit 是 No，YouTube Premium 识别成英国区但 CDN 落在香港。

三网回程的差距比参数表更值得看。广州移动经 PCCW 转 CMI 新加坡回香港再到广州，延迟 **45ms** 左右；广州电信绕美国圣何塞、山景城再回广州，**380~389ms**；广州联通经 NTT、Lumen 转洛杉矶再回广州，**434~491ms**。测试者自己的结论是“性价比不错，2T 流量，落地很不错。国内直连不行”。这句话基本概括了 Akile 全线 Lite 档的性格。

**台湾 NAT，2024 年 8 月。** 套餐 TWNAT2-128M，1 核 256M / 3GB / 1024G 月流量，¥61.99/年。使用者拿它解锁 GPT 和 Netflix，路由和延迟都满意，但看视频始终上不了 4K。早中晚随机测速稳定在 **40Mbps** 左右，而机器标注的带宽是 600Mbps（套餐页另一处写 248M）。找商家沟通得到的答复是共享带宽。这条记录的价值在于给出了“标称带宽”和“实际带宽”之间可以差多少的量级。

**IX 打流，2025 年 9 月。** 用 RouterOS Bandwidth Test 双向各跑 200M，CPU 占用约 70%。同场对比的另一家只能跑上下行合计 200M、CPU 占用 80%，判断是单核瓶颈。这条只说明 Akile 在纯转发场景下的 CPU 余量还行，不代表大陆方向速度。

## 系列之间的差别到底在哪

Lite 和 Hyper 系列（HKLite、JPHyper、SGLite、LAXLite）没有大陆方向优化，定位是落地机：解锁流媒体、做海外业务的出口、跑不需要低延迟的脚本。它们的标称带宽数字最大，价格最低，也最容易受共享带宽影响。

Pro 和 Premium 系列（HKPro、JPPro、LAXPro、LAX Premium）卖的是线路。电信 CN2 GIA、联通 9929、移动 CMIN2 三条都覆盖，双向优化。价格贵一个量级，端口带宽反而小，因为成本花在线路上了。要大陆访问稳定，只能从这一档里选。

BGP 和 ISP 系列（KR BGP、KR Pro、LAX4837 双 ISP、UKbgp）的特点是原生 IP、家宽属性、带防护。KR Pro 比 KR BGP 多防护，其他一致，第三方测评站给了 4.0 星，亚洲双向 GIA。LAX4837 那四档则是给需要美国住宅 IP 属性的场景准备的。

翻倍盲盒是纯概率产品。月付随机翻倍一项配置，年付翻倍两次，¥9.99/月能开出 256MB 还是 1024MB 内存看运气。想稳就别买。

## 优惠码与真实年成本

目前能交叉确认的优惠码有四个：

| 优惠码 | 力度 | 适用范围 |
| --- | --- | --- |
| `AkileCloud/LAXBASE/CUT-20` | 8 折 | 洛杉矶 LAX Base 新购 |
| `AkileCloud/LAXPRO-MONTH/CUT-20` | 8 折 | 洛杉矶 LAX Pro 月付 |
| `AkileCloud/LAXPRO-YEAR/CUT-30` | 7 折 | 洛杉矶 LAX Pro 年付 |
| `AkileCloud/HOT/CUT-15` | 85 折 | 全场非独享套餐 |

用法是在产品详情页右上角的兑换码输入框填入并确认，系统自动折扣。部分码兑换后 **30 分钟内必须使用**，过期作废，所以先想好买哪档再去领。多数码是循环的，续费时还能用。

另有一份整理列出过 `AkileCloudLsStart`（全场轻量云永久 8 折）和 `AK47`（LAX4837 75 折），但更新更近的那份清单里没有这两个码，无法确认当前是否仍有效。想试的话在结算页填一下就知道，不要为了一个不确定的码改变购买计划。

年付 7 折比月付 8 折再低约 12.5%。以 LAXPro-Standard 的 ¥74.99/月为基准，按月付价折算 12 个月，8 折是 ¥719.88 一年，7 折约 ¥629.92 一年，差 **90 元左右**。这是纯算术，实际年付标价和计费月数以下单页为准。如果你确定要用满一年，年付码值得多花两分钟。

👉 [用年付 7 折开通 LAXPro](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811)

## 哪些人不该买，哪些坑要提前知道

需要稳定直连大陆跑业务、跑数据库、要企业级 SLA 的，Akile 不是合适的选择，官方自己就写明不保证大陆直连。这类需求应该找专线回国产品或者国内云。

剩下的坑都属于“买之前知道就没事”的类型：

**入门盘只有 5GB。** 缓存内容、跑日志、装大一点的依赖都会卡住。真要跑服务，选 20GB 起的档位，或者自己挂块盘。

**标称带宽是共享上限。** 5000M、10000M 这些数字不是独占。台湾 NAT 那台标 600Mbps 实测 40Mbps 的例子摆在那里，买之前把预期调到“够用”而不是“跑满”。

**宣传线路可能变。** 有第三方测评记录，JPPro-One 双 11 版官方宣传三网优化（电信联通 IIJ、移动 CMI），实测当时三网都走 CMI，测评者的原话是“不知道能持续多久”。线路调优是动态的，别把某一篇测评的路由图当成永久承诺。

**部分机型 IP 不能原生解锁。** LaxHyper（¥77.77/年）被测评站给了 2.8 星，评价是没有大陆方向优化、没有强计算性能，唯一亮点是 DNS 流媒体解锁，改 DNS 之后才看到原生解锁情况，IP 本身无法原生解锁。买之前分清你要的是 DNS 解锁还是 IP 原生解锁。

**IPv6 不一定有。** 官方说每台配 IPv4 和 IPv6，但 2024 年 12 月那份 HKLite 实测里 IPv6 是 0 个。依赖 IPv6 的业务先问清楚。

**面板要适应。** 自研面板不是 cPanel 体系，第一次上手会愣一下，用过几次就顺了。

**英文支持一般。** 客服和文档以中文为主，英文工单响应慢。

## 退款和下单前的动作

第三方整理给出的退款规则是新购 3 天内退 80%、7 天内退 50%、10 天内退 20%，超过不退。三档比例都按购买价算。这条只有一个来源，下单前请在官网条款页自己确认一遍。

买完的第一件事不是装环境，是跑测试：用 Looking Glass 看回程路由，用流媒体检测脚本确认解锁区域，用 speedtest 打到你的宽带看实际速度。有问题在前三天内提工单，退款比例最高。

## 常见问题

**Akile 靠谱吗？**

2023 年成立，AKILE LTD 注册在英国伦敦，机房覆盖香港、台湾、日本东京、韩国首尔、新加坡、美国洛杉矶、英国伦敦、德国法兰克福等约 10 个国家和地区。这两条信息在两个独立来源里一致。它是预算型服务商，不是企业级供应商，用它跑非关键业务问题不大。

**能不能直连大陆？**

官方明确不保证。实测数据是移动走 CMI 约 45ms，电信绕美 380ms 以上，联通绕美 430ms 以上。要低延迟只能选 HKPro、LAXPro、LAX Premium 这些三网优化档。

**哪个套餐最便宜？**

目前查得到的最低价是日本 JPHyper-One 番茄特供 ¥7.3/月，1 核 1GB，2500M 带宽 1TB 流量，限量供应经常缺货。香港 HKLite-One ¥8.8/月排第二。

**流量超了会怎样？**

限速到共享 10Mbps，不会停机。想恢复可以付费重置流量，费用按套餐不同，公开记录里有 ¥7、¥10、¥14 三种口径。

**Akile 和 Acck 是什么关系？**

第三方测评站把 Acck 称为 Akile 的“孪生兄弟”，产品、线路、技术师出同源，价格更低。Acck 的 TWlite 和 JPlite 各 3.0 星，被评价为“纯粹落地鸡”；JP IIJ 3.3 星。两家定位接近，选哪家看具体档位的价格和库存。

## 最后怎么选

预算压在 ¥10/月以内、主要用来解锁流媒体或做海外出口：JPHyper-One 或 HKLite-One，缺货就退到 HKSM-One 或 SGLite-One。这一档不要期待大陆速度。

需要大陆方向稳定、能接受几十到一百多一个月：LAXPro-Light（¥43.74/月，300GB 流量）或 LAXPro-Standard（¥74.99/月，1TB 流量），配合年付 7 折码。流量用得少就选 Light，别为用不完的额度付钱。

需要美国原生 IP 和家宽属性：LAX4837 的 ISPMini，¥54.99/月，1TB 流量 1Gbps。往上加钱只是加核心和流量，线路不变。

下单前确认两件事：结算页上的实际配置和你看到的是不是同一版（尤其是硬盘和计费周期），以及优惠码填入后价格有没有真的变。

👉 [前往 Akile 核对当前套餐与优惠](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811)
