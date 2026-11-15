# OneirosCoin（ONRC）
## 项目白皮书 · 中文版 · 1.0 版

**发布日期：**2026 年 11 月 16 日  
**网络：**Solana 主网  
**官方网站：**https://yohakusama.github.io/oneiroscoin/  
**代币 Mint 地址：**`D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55`  
**项目联系邮箱：**waylanus@gmail.com

> **文档范围与依据。** 本白皮书介绍 OneirosCoin 的定位、2026 年 11 月 15 日链上核验时确认的参数，以及尚未解决的问题。本文件属于项目信息披露。它不构成独立安全审计、招股说明书或投资建议。链上状态会变化，交易前应重新查询实时数据。

## 1. 项目摘要

OneirosCoin，简称 **ONRC**，是部署在 Solana 上的迷因代币。项目名称受到古希腊神话中梦之精灵 *Oneiroi* 的启发，品牌形象是一只梦境中的大鹅。项目的核心定位是文化表达与社区交流。ONRC 没有开发新的公链、共识算法、去中心化交易协议或支付网络。代币依托 Solana 的 SPL Token 标准和 Meteora Dynamic Bonding Curve（DBC）运行。

已核验的发行总量为 **10 亿枚 ONRC**，精度为 **6 位小数**。代币的增发权限与冻结权限均已撤销。初始 ONRC/USDC DBC 资金池配置了 **0.30% 基础交易手续费**，关闭了 DBC 动态手续费，并将毕业门槛设为 **750 USDC 的报价资产储备**。当毕业条件满足且迁移成功执行后，目标资金池为 **Meteora DAMM v2**，其中**创建者 LP 分配比例设为 100% 永久锁定**。这是未来迁移的链上配置，并不代表锁仓已经发生。

根据 **2026 年 11 月 15 日 21:32（UTC）** 的链上核验记录，资金池当时的 USDC 储备为 **0**，毕业进度为 **0%**，**尚未完成迁移**。该记录有时间限制，不代表实时行情。

## 2. 项目定位与用途边界

### 2.1 品牌背景

Oneiroi 是古希腊神话中与梦有关的精灵群体。“大鹅”“金币纹理”和“Born from a dream. Destined for nothing. Honk your dreams.” 均属于项目的品牌创作。项目不宣称大鹅本身是古希腊神话中的原始角色。

### 2.2 当前已经实现的功能

ONRC 是部署在 Solana 主网的可转移 SPL 代币。项目已创建以 USDC 为报价资产的 Meteora DBC 资金池。用户能够通过 Solana 区块浏览器或 RPC 查询代币、资金池、配置账户与交易记录。是否能顺利买卖、获得什么成交价格，以及是否被聚合交易平台收录，取决于查询时的链上状态和第三方服务。

### 2.3 当前没有提供的权利

**现有公开资料没有证明 ONRC 附带公司股权、分红、项目收入分配权、金库资产索取权、固定价格赎回权、链上治理投票权、质押收益或特定付费服务权益。** 本白皮书也不作出这些承诺。

## 3. 代币技术参数

| 参数 | 已核验信息 |
|---|---|
| 名称 / 代号 | OneirosCoin / ONRC |
| 网络 | Solana 主网 |
| 代币标准 | SPL Token（传统 Token Program） |
| Mint 地址 | `D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55` |
| 精度 | 6 位小数 |
| 已核验总供应量 | 1,000,000,000 ONRC（10 亿枚） |
| 最小单位供应量 | 1,000,000,000,000,000 |
| 增发权限 | 已撤销，链上值为 null |
| 冻结权限 | 已撤销，链上值为 null |
| 元数据 | 名称和代号已上链；元数据不可修改 |
| 报价代币 | Solana USDC：`EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v` |
| DBC 配置账户 | `DARJaFYLWWepZnmN4ezrTziU2ymRbZae1NhZYuetNc1E` |
| DBC 资金池 | `2zbY23A7UWMmdY14zgeneJw5jcdRwqYQu6K6XbsgDpgU` |
| 链上元数据链接 | `https://gateway.irys.xyz/3S2vDEHeS4HQFsU3ePvzmpvB4Z3yxuWJznT8fLyAfpzK` |

**固定供应量的含义。** 撤销增发权限后，该 Mint 无法通过普通增发流程增加供应量。但这不能证明代币分配公平、持仓分散、市场流动性充足或价格稳定。元数据不可修改，也不代表项目网站或社交账号永远不会变化。

## 4. 发行机制与毕业流程

### 4.1 动态绑定曲线

ONRC 使用 Meteora 已有的 Dynamic Bonding Curve（DBC）程序。毕业前，代币在虚拟资金池中按照链上价格曲线交易。成交价格与滑点取决于曲线参数、当前储备和交易规模。项目没有承诺稳定价格或最低卖出价格。

### 4.2 USDC 报价与毕业门槛

资金池使用 Solana USDC 报价。已核验配置将报价资产储备达到 **750 USDC** 设为毕业门槛。这是资金池生命周期中的迁移条件，**不代表项目已经持有 750 USDC，也不代表团队承诺投入 750 USDC**。它同样不构成投资者保护准备金。Meteora 文档将使用 750 USDC 门槛的合格主网 DBC 池列为自动迁移服务的适用情形，但迁移仍取决于合约条件与相关服务能否执行 [5]。

### 4.3 毕业之后

配置的迁移目标为 **Meteora DAMM v2**。核验结果显示，**创建者永久锁定 LP 占比 100%**，创建者可提取 LP 为 **0%**，合作方可提取 LP 为 **0%**，合作方永久锁定 LP 为 **0%**。这些比例针对迁移后的流动性头寸分配，**不等于锁定 100% 的 ONRC 代币总供应量**。只有毕业迁移完成并生成 DAMM v2 流动性头寸后，才能核实真实锁定状态。

永久锁仓限制从头寸中提走被锁定的底层流动性资产。但根据 Meteora 的设计，永久锁定的头寸仍可能产生可领取的交易手续费 [6]。所以，“100% 永久锁仓”不能理解为“创建者永久放弃全部经济收益”。

## 5. 手续费与创建者收益

| 项目 | 当前核验配置 |
|---|---|
| DBC 基础交易手续费 | 30 个基点，即 0.30% |
| DBC 动态交易手续费 | 已关闭 |
| 创建者对非协议手续费份额的分配 | 创建者/合作方份额中的 100% |
| DBC 资金池创建费配置 | 0 |
| 毕业后的目标协议 | DAMM v2 |
| DAMM v2 选择的基础费率档位 | 0.30% |
| 迁移后 LP 锁定分配 | 创建者永久锁定 100%，可提取 0% |

**0.30% 基础费率**指每 1 单位交易名义金额所对应的基础交易费率为 0.003。它不包含用户可能承担的网络手续费、路由成本、价格冲击和滑点。Meteora DBC 会将交易费划分为协议份额与非协议份额。“创建者分配比例 100%”**仅针对创建者与合作方之间可分配的份额，不能理解为创建者获得全部交易手续费** [4]。

核验时的创建者、费用领取者和剩余资产接收地址为：`9p9dNQSVoq3hD6iGG9k9WF2ozcMsfMQGY6ZSN2xq2GbY`。已有公开证据不能证明这部分收入必须用于开发、营销、回购、销毁、奖励或补充流动性。本白皮书不作出相关资金用途承诺。协议级手续费及迁移时的费用依照 Meteora 当时适用的程序规则执行 [4]。

## 6. 供应量、分配与持仓披露

**供应量已经核验，完整分配方案尚未核实。** 链上观察结果证明总发行量为 10 亿枚，但现有核验资料未提供覆盖全部钱包的初始分配表、最终受益人信息、团队与投资者分配比例、归属期协议或交易所持仓说明。因此项目不宣称“团队零持仓”“100% 公平发行”“没有内部人”或“所有权完全去中心化”。

链上余额和转账记录公开可查。未来若发布正式分配说明，应列出各类份额、持仓钱包、由谁控制以及核对日期。在完成这类披露之前，**持仓集中度仍属于未确认事项**。

创建者或费用领取钱包的存在，也不能证明该地址受社区共同管理，或其资产属于独立法律主体持有的公共金库。项目尚未提供可核验的金库治理机制。

## 7. 治理与运营安排

### 7.1 当前治理状态

现有资料没有证明 ONRC 建立了链上代币投票系统、社区 DAO 金库或由持有人控制的协议升级机制。网站和社交媒体内容由链下运营者管理。项目公开联系邮箱为 `waylanus@gmail.com`。现有资料没有披露完整的法律运营主体及其注册司法辖区。

### 7.2 后续计划的范围

项目计划持续公开中英文说明、链上核验入口以及必要的更正记录。任何未来的社区活动、艺术创作或产品功能，都需要另行公布并提供相应证据，才属于正式项目承诺。**本文件不承诺上线交易所、特定营销预算、社区激励、开发进度或未来收益。**

### 7.3 链上数据优先

本白皮书用于解释项目，不改变智能合约的实际执行。涉及发行量、权限、资金池参数与迁移状态时，应优先依据最新链上数据，不能只凭网页描述、平台缓存或截图作判断。

## 8. 安全与技术依赖

ONRC 使用 Solana SPL Token Program 及第三方 Meteora DBC 和 DAMM v2 程序。使用成熟基础设施不意味着没有风险。程序漏洞、权限配置、系统更新、节点服务故障、第三方服务中断及钱包密钥泄露，都会影响用户。

此前项目使用只读脚本检查了部分链上字段和交易最终确认状态。**这种检查不构成独立的代码安全审计，也不等于安全认证。** 增发与冻结权限已撤销、元数据不可修改，是可以核实的安全约束。但这些约束不能保证行情安全、流动性充足、代币分配公平或所有交易对手可信。

## 9. 主要风险

**投机和本金损失。** ONRC 没有承诺赎回价格、利息或分红。市场价格波动很大，代币价值可能归零。

**流动性与成交风险。** 资金池规模较小时，卖出交易可能面临高滑点、极端价格冲击、MEV 夹子交易、失败交易或暂时无法成交。

**代币持仓和费用领取。** 持仓集中度、内部持有情况尚未完整披露。费用领取权确实存在。永久锁定流动性不等于放弃全部手续费收益。

**毕业与迁移风险。** 750 USDC 门槛和 DAMM v2 迁移属于链上配置。达到门槛的时间、自动迁移执行及锁仓完成均未得到保证。第三方程序或服务出现故障会影响过程。

**技术和托管风险。** Solana、Meteora、钱包、节点服务、Irys 元数据存储、项目网页与社交账号均存在独立风险。私钥泄露或遗失可能导致不可逆的资产损失。

**法律与税务风险。** 不同地区的数字资产规则不同，也会继续变化。交易者需要自行核对当地法律要求及税务责任。

**信息更新风险。** 浏览器、聚合器与项目网页显示的数据可能存在延迟。本文引用的核验记录不能证明此刻的代币价格、持有人数、交易量、市值或未来表现。

## 10. 链上核验记录及其限制

| 核验项目 | 2026 年 11 月 15 日记录 |
|---|---|
| DBC 配置账户和资金池 | 已建立，SDK 解码成功 |
| ONRC Mint | 已建立，10 亿枚，6 位小数 |
| 增发 / 冻结权限 | 均已撤销 |
| 代币元数据 | 已上链且不可修改，名称与 URI 匹配 |
| DBC 费率 | 基础 0.30%，动态费已关闭 |
| 毕业门槛 | 750 USDC 报价储备 |
| 迁移与锁仓设置 | DAMM v2，创建者 LP 100% 永久锁定 |
| 当时池内储备 / 毕业进度 | 0 USDC / 0% |
| 当时的迁移和最终锁仓 | **尚未完成** |
| 独立代码安全审计 | **现有资料未提供** |
| 最终受益人维度的代币分配 | **现有资料未提供** |

上述数据来自 2026 年 11 月 15 日 21:32（UTC）的 Solana 主网只读检查。检查通过，但有一项信息提示：SDK 未返回部分 tokenSupply 字段，脚本改为直接核对 Mint 总供应量。创建配置交易与创建资金池交易在当时均显示最终确认，且没有执行错误。**这不能证明资金池现在的储备或迁移状态。**

## 11. 公开地址与联系方式

- **ONRC Mint 地址：**`D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55`
- **DBC 资金池：**`2zbY23A7UWMmdY14zgeneJw5jcdRwqYQu6K6XbsgDpgU`
- **DBC 配置账户：**`DARJaFYLWWepZnmN4ezrTziU2ymRbZae1NhZYuetNc1E`
- **创建者 / 费用领取者：**`9p9dNQSVoq3hD6iGG9k9WF2ozcMsfMQGY6ZSN2xq2GbY`
- **元数据：**https://gateway.irys.xyz/3S2vDEHeS4HQFsU3ePvzmpvB4Z3yxuWJznT8fLyAfpzK
- **Solscan：**https://solscan.io/token/D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55
- **官网：**https://yohakusama.github.io/oneiroscoin/
- **X：**https://x.com/oneiroscoin
- **Telegram：**https://t.me/OneirosCoin
- **联系邮箱：**waylanus@gmail.com

## 12. 参考资料与编写方法

本白皮书借鉴成熟项目对“目标、设计、机制、验证和风险”的说明方法。以下资料仅用于结构和技术核对，**不表示相关项目参与、支持 ONRC，也不表示 ONRC 拥有相同技术创新**。

1. Satoshi Nakamoto，《Bitcoin: A Peer-to-Peer Electronic Cash System》（2008）。https://bitcoin.org/bitcoin.pdf
2. Ethereum，《A Next-Generation Smart Contract and Decentralized Application Platform》（2014）。https://ethereum.org/whitepaper/
3. Solana，《A New Architecture for a High Performance Blockchain》。https://solana.com/solana-whitepaper.pdf
4. Meteora，《DBC Formulas》《Launch Configurations》。https://github.com/MeteoraAg/docs/blob/main/core-products/dbc/formulas.mdx 和 https://github.com/MeteoraAg/docs/blob/main/core-products/dbc/launch-configurations.mdx
5. Meteora，《DBC Developer Guide and Migration Keeper Thresholds》。https://github.com/MeteoraAg/docs/blob/main/developer-guides/dbc/index.mdx
6. Meteora，《DAMM v2 Overview and LP Locks》。https://github.com/MeteoraAg/docs/blob/main/core-products/damm-v2/what-is-damm-v2.mdx 和 https://github.com/MeteoraAg/docs/blob/main/user-guides/how-to-use-damm-v2/damm-v2-pool-detail.mdx
7. Uniswap，《Uniswap v3 Core Whitepaper》（2021）。https://app.uniswap.org/whitepaper-v3.pdf
8. OneirosCoin，2026 年 11 月 15 日 21:32（UTC）链上只读核验记录。主要公开账户见第 3 节与第 11 节。该检查由项目执行，不属于独立协议安全审计。

## 版本与免责声明

**1.0 版，2026 年 11 月 16 日。** 本文以已验证的资料为基础，并明确列出未知事项。今后修订应注明日期、修改内容和新的链上核验依据。英文版与中文版应保持相同的实质信息。本文件仅供了解项目，不构成证券销售邀约，不承诺收益、流动性、毕业、奖励或安全性。