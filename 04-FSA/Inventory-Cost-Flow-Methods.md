---
subject: Financial Statement Analysis
topic: Inventory Cost Flow Methods
status: "🟡 解析能懂，待独立验证"
created: 2026-11-03
last-reviewed:
tags: [CFA-L1, FSA, Inventory, FIFO, LIFO]
---

# 存货成本流转方法（Inventory Cost Flow Methods）

## 一句话理解
FIFO、LIFO 和 Weighted Average Cost 决定哪批采购成本计入当期销售成本（COGS），哪批成本留在期末存货（Ending Inventory），不一定等于实物实际出售的顺序。

## 三种方法
- **FIFO — First In, First Out（先进先出法）**：较早购入成本先计入 COGS，较新购入成本留在存货。
- **LIFO — Last In, First Out（后进先出法）**：较新购入成本先计入 COGS，较早购入成本留在存货。
- **Weighted Average Cost (WAC，加权平均成本法）**：使用平均单位成本计算销售成本和期末存货。

$$
Average\ Unit\ Cost=\frac{Total\ Cost\ of\ Goods\ Available\ for\ Sale}{Total\ Units\ Available\ for\ Sale}
$$

## 价格上涨与下降时的影响

在采购价格持续单向变化、销售数量等其他条件一致，且没有特殊存货层清算等影响时：

| 观察项目 | Rising Prices 价格上涨 | Falling Prices 价格下降 |
|---|---|---|
| FIFO 的 COGS | 较低 | 较高 |
| LIFO 的 COGS | 较高 | 较低 |
| FIFO 的报告利润 | 较高 | 较低 |
| LIFO 的报告利润 | 较低 | 较高 |
| FIFO 的期末存货 | 较高 | 较低 |
| LIFO 的期末存货 | 较低 | 较高 |

WAC 的结果在常见连续单向价格变动情境下通常位于 FIFO 和 LIFO 之间。

## 价格下降：为什么 LIFO 的利润更高？

假设先购入100件、单位成本 $10；后购入100件、单位成本 $6；本期售出100件、单位售价 $15。忽略其他费用。

| 方法 | COGS | 毛利润 |
|---|---:|---:|
| FIFO | 100×10 = $1,000 | $1,500−$1,000 = $500 |
| WAC | 100×8 = $800 | $700 |
| LIFO | 100×6 = $600 | $900 |

结论：

$$
COGS_{LIFO}<COGS_{WAC}<COGS_{FIFO}
$$

$$
Gross\ Profit_{LIFO}>Gross\ Profit_{WAC}>Gross\ Profit_{FIFO}
$$

**易错点：早期采购成本更高，不代表卖出商品一定亏损，只意味着采用 FIFO 时确认的销售成本较高、其他条件相同时报告利润较低。**

## IFRS 与 US GAAP
| 方法 | US GAAP | IFRS |
|---|---|---|
| FIFO | 允许 | 允许 |
| LIFO | 允许 | **不允许** |
| Weighted Average Cost | 允许 | 允许 |

## 考试判断路径
1. 判断采购价格是上涨还是下降。
2. FIFO：先把旧成本放进 COGS；LIFO：先把新成本放进 COGS。
3. 用 Revenue − COGS 计算毛利润，判断高低。
4. 期末存货与 COGS 的成本批次通常相反。
5. 留意 IFRS 禁止 LIFO；还应关注 LIFO Liquidation（后进先出存货层清算）等特殊情境。

## 自测
- [ ] 价格上涨时能正确判断 FIFO 和 LIFO 的 COGS、利润、期末存货
- [ ] 价格下降时能正确判断 FIFO 和 LIFO 的 COGS、利润、期末存货
- [ ] 能解释成本流转假设不必等于实物流转
- [ ] 能解释 IFRS 与 US GAAP 对 LIFO 的不同规定

## 存货跌价减记（Inventory Write-down）与资产周转率

**存货减记不是商品销售。** Inventory（存货）是资产负债表上的存量；Revenue（营业收入）是利润表中已经履行相应义务而确认的期间收入。存货账面价值下调，不会直接改变已确认的营业收入。

存货减记的典型直接影响：
- **Inventory / Total Assets（存货 / 总资产）下降**；
- **Write-down Expense or Loss（跌价费用或损失）增加**；
- **Net Income（净利润）通常下降**（税后下降幅度受税务影响）；
- **Revenue（营业收入）不因这项减记本身改变**。

### 总资产周转率（Total Asset Turnover）

$$
\boxed{Total\ Asset\ Turnover=\frac{Revenue}{Average\ Total\ Assets}}
$$

其中：

$$
Average\ Total\ Assets=\frac{Beginning\ Total\ Assets+Ending\ Total\ Assets}{2}
$$

在收入及其他条件不变时，如果存货减记使期末总资产减少，平均总资产随之下降，则：

$$
Revenue\ unchanged,\quad Average\ Total\ Assets\downarrow
\quad\Rightarrow\quad Total\ Asset\ Turnover\uparrow
$$

**示例**：收入100；期初资产100；减记前期末资产100；减记后期末资产90。

- 减记前：100 / 100 = 1.00 倍。
- 减记后：100 / [(100+90)/2] = 1.0526 倍。

这只是资产账面金额下降导致的**比率机械上升**，不能自动视为经营效率改善。

### 易混概念
- **Inventory Write-down（存货跌价减记）**：存货账面金额下降，确认相应损失，不直接确认或减少 Revenue。
- **Sale of Inventory（销售存货）**：满足收入确认条件时确认 Revenue，并结转相应 COGS。
- **Current Ratio（流动比率）**：存货减记通常使分子减少。
- **Quick Ratio（速动比率）**：分子通常不含存货，因此存货减记不会直接减少速动资产；仍须留意其他调整。

关联：[[Common-Size-Statements-and-Financial-Ratios|财务比率分析]]。


## 销售成本（Cost of Goods Sold，COGS）基础概念

**一句话理解：COGS 是本期已销售商品所对应的存货成本，而不是本期全部采购成本，也不是商品售价。**

### Revenue、COGS 和 Inventory 的区别

| 项目 | 英文 | 所属报表 | 含义 |
|---|---|---|---|
| 营业收入 | Revenue | 利润表 | 已满足收入确认条件的商品或服务销售收入 |
| 销售成本 | Cost of Goods Sold (COGS) | 利润表 | 本期已经售出商品对应的成本 |
| 存货 | Inventory | 资产负债表 | 截至报告日尚未售出商品等的成本 |
| 毛利润 | Gross Profit | 利润表 | Revenue 减 COGS |

### 公式一：毛利润

$$
\boxed{Gross\ Profit=Revenue-COGS}
$$

其他条件不变时，COGS 上升会使毛利润下降；COGS 下降会使毛利润上升。

### 公式二：零售企业简化的存货流转公式（BASE）

$$
Beginning\ Inventory+Purchases-COGS=Ending\ Inventory
$$

因此：

$$
\boxed{COGS=Beginning\ Inventory+Purchases-Ending\ Inventory}
$$

例如：期初存货20,000，本期采购100,000，期末存货40,000，则 COGS = 80,000。

该简化公式假设没有存货跌价、损耗、退货、转移等其他调整。生产企业还需要考虑制造成本、在产品和完工产品等。

### 实例：采购不等于销售成本

手机店采购100台手机，每台进货成本1,000元，其中卖出60台、每台售价1,500元：
- Purchases（采购成本）：100,000元；
- Revenue（营业收入）：60×1,500 = 90,000元；
- COGS（销售成本）：60×1,000 = 60,000元；
- Ending Inventory（期末存货）：40×1,000 = 40,000元；
- Gross Profit（毛利润）：90,000−60,000 = 30,000元。

**易错点：**买了100台不等于卖了100台；只有卖出去的60台对应的成本计入本期 COGS，未售的40台仍留在 Inventory。

### 与 FIFO、LIFO 的联系

FIFO、LIFO、WAC 是 **Cost Flow Assumptions（成本流转假设）**，决定哪些采购批次的成本进入 COGS，哪些留在 Ending Inventory，并不一定代表商品的实际物理出库顺序。

### 自测
- [ ] 能区分 Revenue、Purchases、COGS、Inventory
- [ ] 能用 BASE 推出 COGS
- [ ] 能解释为什么未售出的商品成本不计入 COGS
