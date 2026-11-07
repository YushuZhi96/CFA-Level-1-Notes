---
subject: CFA Level I
topic: Equity Investments Fundamentals
status: 持续更新
tags: [CFA-L1, Equity, Fundamentals]
---

# Equity Investments Basics｜权益投资基础概念

本文件集中整理 CFA 一级权益投资（Equity Investments）章节中的基础概念、重要英文术语及做题判断方法。复杂模型与专项考点另建独立笔记。遇到涉及其他科目的知识点时，标明交叉关系，不按每道题重复建文件。

## 1. Market Participants and Trading Objectives｜市场参与者与交易目的

### Hedger｜套期保值者

- **定义**：已经面临某种价格、利率或汇率等风险的个人或机构，利用金融合约抵消或降低原有风险敞口（Risk Exposure）。
- **目的**：Risk Reduction（降低风险），而非单纯追求价格波动带来的盈利。
- **考试关键词**：Worried about price decrease / increase、Lock in a price、Reduce price risk、Protect against losses。
- **例子**：农民未来需要出售谷物，担心谷物跌价，今天卖出谷物远期合约锁定未来售价，属于 Hedger。
- **注意**：套期保值旨在降低特定风险，也可能放弃有利价格变动带来的额外收益；仍可能存在交易对手风险（Counterparty Risk）、数量或期限不匹配等风险。

### Speculator｜投机者

- **定义**：主动承担市场价格变动的风险，希望通过判断价格方向获得收益的交易者。
- **目的**：Profit from price movements（从价格波动中获利）。
- **例子**：交易者没有谷物现货或未来销售需求，只因预测谷物跌价而卖出谷物远期合约，通常属于 Speculator。
- **区别**：同为卖出远期合约，是否属于 Hedger，要看其是否在抵消**原有风险敞口**。

### Investor｜投资者

- **定义**：投入资金购买证券或其他资产，以获取收益、资本增值或满足投资目标的个人或机构。
- **目的**：Investment Return（投资回报），通常同时考虑风险与流动性。
- **注意**：Investor 与 Hedger 不一定在现实中互斥；投资者也可能进行套期保值。但在题目要求选择 **most appropriate label** 时，应根据案例最直接体现的交易目的选答案。

### Securitizer｜证券化者

- **定义**：参与将贷款、应收款等资产或其现金流汇集、重组，并以此为基础发行或安排发行证券的主体。
- **相关概念**：Securitization（资产证券化）、Asset-Backed Securities (ABS，资产支持证券)。
- **例子**：金融机构将一批住房抵押贷款汇集，形成可向投资者出售的证券。
- **不是套期保值**：证券化关注资产转化和融资结构；农民使用远期合约锁定未来售价不构成证券化。

### 四种角色对照

| 角色 | 英文 | 关键目的 | 判断线索 |
|---|---|---|---|
| 套期保值者 | Hedger | 降低已有风险 | 有现货或未来真实经营需求；锁定价格 |
| 投机者 | Speculator | 承担价格风险博取收益 | 主要根据行情判断建立风险头寸 |
| 投资者 | Investor | 获取投资回报 | 出资买入并持有资产或证券 |
| 证券化者 | Securitizer | 将资产现金流转化为证券 | 资产池、证券发行、现金流重组 |

## 2. Forward Contracts and Hedging｜远期合约与套期保值

### Forward Contract｜远期合约

- **定义**：双方约定在未来特定日期，以约定价格交易特定数量标的资产的合约；通常属于场外交易（Over-the-Counter, OTC）。
- **Forward Price / Delivery Price（远期约定价格）**：合约约定的未来交易价格；本题中是农民希望锁定的谷物售价。
- **Short Forward（卖出远期）**：承诺在未来按合约约定价格卖出标的。
- **Long Forward（买入远期）**：承诺在未来按合约约定价格买入标的。

### Short Hedge｜卖出套期保值

- **适用情形**：未来要卖出现货，担心现货价格下跌。
- **典型主体**：农民、商品生产商等。
- **操作**：卖出对应标的远期合约（Short Forward）以对冲未来现货销售收入下降的风险。

### Long Hedge｜买入套期保值

- **适用情形**：未来要采购标的，担心采购价格上涨。
- **典型主体**：未来需要购买燃油的航空公司。
- **操作**：买入对应标的远期合约（Long Forward）以对冲未来采购成本上升的风险。

| 经营需求 | 担心什么 | 典型操作 | 对冲方向 |
|---|---|---|---|
| 未来卖谷物 | 谷物跌价 | Sell Forward | Short Hedge |
| 未来买燃油 | 燃油涨价 | Buy Forward | Long Hedge |

### 例子：农民为什么属于 Hedger？

假设农民将在三个月后出售 1,000 吨谷物，并签订远期合约，约定每吨 2,000 元卖出。为便于理解，假设标的、数量、日期完全匹配，交易对手正常履约，不计成本。

| 三个月后的市场价 | 没有远期合约的销售收入 | 按远期约定的销售收入 |
|---|---:|---:|
| 1,500 元/吨 | 150 万元 | 200 万元 |
| 2,500 元/吨 | 250 万元 | 200 万元 |

- 价格下跌：远期合约保护农民免于按更低价格出售。
- 价格上涨：农民无法享受市场价上涨的额外收益。
- **核心**：农民为了稳定未来销售收入（减少价格风险），而不是单纯押注谷物价格下跌。

## 3. CFA Exam Traps｜考试陷阱与判断顺序

1. **先看原有风险敞口**：当事人是否已经持有现货，或有真实的未来买卖需求？
2. **再看交易目的**：为了 Lock in a price / Reduce risk，还是为了 Profit from price movements？
3. **最后看工具和方向**：Future sale + short forward；future purchase + long forward。
4. **不要把交易方向当作身份**：卖出远期不一定是投机，买入远期也不一定是投资。
5. **不要把证券化误认成套保**：Securitizer 涉及资产池与证券发行，不是简单的远期买卖。

**典型题识别**：A grain farmer worries about a fall in grain prices and enters a forward contract to sell grain at a predetermined price → **Hedger（套期保值者）**。

**一句话记忆**：Hedger reduces existing risk; Speculator takes risk for potential profit.

## 4. 复习清单

- [ ] 能解释 Hedger、Speculator、Investor、Securitizer 的区别
- [ ] 能识别农民卖出远期与航空公司买入远期分别在对冲什么风险
- [ ] 知道同一种交易工具可以用于 Hedging，也可以用于 Speculation
- [ ] 能解释套期保值为何可能放弃有利行情带来的额外收益

**交叉科目**：[[07-Fixed-Income/Fixed-Income-Basics|固定收益基础概念]]（Securitization）；Derivatives（远期合约机制）。
