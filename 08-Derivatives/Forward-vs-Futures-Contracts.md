---
subject: Derivatives
topic: Forward vs. Futures Contracts
status: "待复习"
created: 2026-11-14
last-reviewed:
tags: [CFA-L1, Derivatives, Forwards, Futures, Hedging]
---

# 远期与期货合约（Forward vs. Futures Contracts）

## 一句话理解

远期（Forward）和期货（Futures）都属于远期承诺（Forward Commitments），但远期通常是 OTC 定制合约，通常到期结算；期货是在交易所交易的标准化合约，通常通过保证金账户每日盯市结算（Daily Mark-to-Market）。

## 核心概念 / 定义

### 1. 远期合约（Forward Contract）

- 交易双方约定在未来某一日期，以预先确定的价格买卖一定数量的标的资产。
- 通常在场外市场（OTC）交易，条款可根据双方风险敞口定制。
- 典型情况下，盈亏在到期时结算；不采用期货式的每日变动保证金结算。
- 定制化使远期有机会更精确地匹配企业的实际风险敞口。

### 2. 期货合约（Futures Contract）

- 在交易所交易的标准化合约。
- 通常要求交易者缴纳初始保证金（Initial Margin）。
- 每个交易日结束时，交易所根据结算价格（Settlement Price）进行逐日盯市（Mark-to-Market）。
- 当日盈亏通过变动保证金（Variation Margin）反映在保证金账户中。

### 3. 两者共同点：远期承诺（Forward Commitments）

Forward 和 Futures 都约定未来交易，双方原则上都承担合同履约义务，因此都属于 Forward Commitments，而不是 Contingent Claims。

### 4. 远期与期货对比

| 比较维度 | Forward 远期 | Futures 期货 |
|---|---|---|
| 交易市场 | 通常 OTC | 交易所 Exchange |
| 合约条款 | 通常定制 Customized | 标准化 Standardized |
| 结算机制 | 通常到期结算 | 每日盯市 Daily Settlement |
| 保证金 | 视双边合同及抵押安排而定 | 通常有初始保证金和变动保证金制度 |
| 流动性 | 通常较低 | 通常较高 |
| 交易对手风险 | 通常较高，依赖双边信用与抵押安排 | 清算机制通常降低交易对手风险 |
| 主要优势 | 可匹配特定风险敞口 | 标准化、透明、流动性通常较高 |

## 公式与变量

期货每日盯市的简化盈亏：

\[
\text{Daily Gain/Loss}= (F_t-F_{t-1})\times Q
\]

其中：
- \(F_t\)：当日结算价格（Settlement Price）
- \(F_{t-1}\)：前一交易日结算价格；首日可用建仓价格
- \(Q\)：合约数量乘数后的合约规模（按合约报价单位换算）

多头（Long Futures）价格上涨时通常获利，价格下跌时通常亏损；空头（Short Futures）方向相反。

## 完美套期保值（Perfect Hedge）

远期合约可用于建立完美套期保值，因为其标的、金额、期限和交割安排可以定制，以匹配企业已有的风险敞口。

但“完美”通常建立在关键条件能够匹配的假设下，例如：
- 对冲工具与风险敞口的标的完全一致；
- 数量和期限匹配；
- 不存在显著基差风险、交易成本或对手方违约等干扰。

实际对冲未必能做到完全消除所有风险。

## 常见考试陷阱

1. **Forward 和 Futures 都属于 Forward Commitments**，不是只有 Forward 才属于远期承诺。
2. **Daily Settlement 是 Futures 的典型特征**，不是传统远期合约的典型结算机制。
3. 期货每日盯市依据交易所公布的结算价格（Settlement Price），盈亏通过保证金账户反映。
4. 远期合约通常在到期时结算；但 OTC 合同也可能通过抵押品协议定期交换担保品，不能将其与期货每日变动保证金机制简单等同。
5. Forward 的定制化有利于匹配风险敞口，因此可用于建立完美套期保值（Perfect Hedge）；但要实现完美对冲，标的、数量和期限等必须匹配。
6. 两者初始时都约定合约价格，但期货头寸会每日盯市，不能把“约定价格”误解为期货合约每天都不发生现金流结算。

## 典型题型 / 判断路径

题目：Which statement about forward and futures contracts is incorrect?

- Forward contracts can be used to create a perfect hedge. → 正确（在风险敞口与合约条款充分匹配的条件下）。
- Both forward and futures contracts are forward commitments. → 正确。
- Both forward price and futures price are subject to daily settlement. → 错误。每日结算是期货的典型机制，不是远期的典型机制。

**正确答案：C。**

## 易混知识点 / Obsidian 链接

- [[Exchange-Traded-and-OTC-Derivatives]]
- [[Contingent-Claims-and-Forward-Commitments]]

## 我的错因 / 验证记录

- [ ] 能区分远期到期结算与期货每日盯市
- [ ] 能解释 Settlement Price 与 Variation Margin 的作用
- [ ] 能说明远期为什么更容易匹配特定套保需求
- [ ] 能区分 Forward Commitment 与 Contingent Claim
