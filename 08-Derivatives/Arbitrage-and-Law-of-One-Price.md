---
subject: Derivatives
topic: Arbitrage and Law of One Price
status: "待复习"
created: 2026-11-14
last-reviewed:
tags: [CFA-L1, Derivatives, Arbitrage, No-Arbitrage]
---

# 套利机会与一价定律（Arbitrage Opportunity & Law of One Price）

## 一句话理解

当两个在经济意义上完全相同、具有相同现金流和风险的资产，在同一时点出现不同价格时，可能产生套利机会（Arbitrage Opportunity）：买入低价资产、卖出高价资产，锁定价差。套利交易会推动价格收敛，因此真正无风险的套利机会通常短暂且不常见。

## 核心概念 / 定义

### 1. 套利（Arbitrage）

套利是利用相同或等价资产之间的错误定价，通过同时建立相反方向的交易，锁定无风险或近似无风险的利润。

典型思路：
- Buy Low：买入被低估的资产。
- Sell High：卖出被高估的相同或等价资产。
- Lock in the Spread：在交易成本、融资约束和执行风险等条件允许时锁定价差。

例子：
- 市场 A 中同一资产价格为 $100。
- 市场 B 中同一资产价格为 $105。
- 同时在 A 买入、在 B 卖出，理论价差为 $5（未扣除交易成本、融资成本及交易限制）。

### 2. 一价定律（Law of One Price）

如果两个资产具有相同的现金流、风险和其他经济特征，并且市场不存在显著交易障碍，那么它们在同一时点应当具有相同价格。

若价格不同，投资者可能通过套利交易促使价格差异缩小。

### 3. 套利机会为什么通常短暂？

- 套利者买入低价资产，推动其价格上涨。
- 套利者卖出高价资产，推动其价格下跌。
- 交易持续进行，价格偏差逐渐收敛，套利空间消失。

因此，真正的无风险套利机会（Risk-free Arbitrage Opportunity）通常是短暂的（Short-lived），并不常见。

## 套利与风险交易的区别

- **套利（Arbitrage）**：目标是在锁定交易结构后获得无风险或近似无风险收益。
- **投机（Speculation）**：主动承担市场风险，以期从价格变化中获利。
- **相对价值交易（Relative-Value Trading）**：利用相关资产之间的相对定价差异，但可能承担基差、模型、流动性和执行风险，不一定是真正无风险套利。

## 衍生品中的应用

衍生品定价常使用无套利原则（No-Arbitrage Principle）：
- 如果衍生品与复制组合（Replicating Portfolio）具有相同未来现金流，它们在无套利条件下应具有相同当前价值。
- 若价格不同，理论上可以通过买入便宜的一方、卖出昂贵的一方构造套利。
- 这一原则是远期、期货和期权定价的重要基础。

## 常见考试陷阱

1. **Identical assets at different prices**：相同资产在同一时点出现不同价格，是套利机会的典型描述。
2. **Long-term arbitrage opportunity**：真正无风险套利通常不会长期存在，因为套利交易会使价格偏差收敛。
3. **Common in markets**：严格意义上的无风险套利机会并不常见；市场中常见的套利策略不等于存在无风险利润。
4. 价差必须大于交易成本、融资成本和其他执行成本，才可能形成可实现的套利利润。
5. 不要把相对价值交易或统计套利自动视为无风险套利；它们可能包含模型风险、基差风险和执行风险。

## 典型题型 / 判断路径

题目：Which statement best portrays arbitrage opportunities?

- Two identical assets are sold at different prices → 正确，可能存在套利机会。
- They may exist for a long-term horizon → 错误，套利交易通常会促使价差收敛。
- They are common in the markets → 错误，严格意义上的无风险套利机会并不常见。

**正确答案：A。**

## 易混知识点 / Obsidian 链接

- [[Forward-vs-Futures-Contracts]]
- [[Derivative-Markets-vs-Spot-Markets]]

## 我的错因 / 验证记录

- [ ] 能解释一价定律（Law of One Price）
- [ ] 能描述买低卖高如何促使价格收敛
- [ ] 能区分无风险套利与承担风险的相对价值交易
