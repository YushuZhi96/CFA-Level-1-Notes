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
