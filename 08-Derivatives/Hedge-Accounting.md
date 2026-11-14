---
subject: Derivatives
topic: Hedge Accounting
status: "待复习"
created: 2026-11-14
last-reviewed:
tags: [CFA-L1, Derivatives, Hedge-Accounting, Risk-Management]
---

# 套期会计（Hedge Accounting）

## 一句话理解

套期会计通过将衍生品与被套期项目的损益或现金流影响按规则配比，减少财务报表中因经济对冲而产生的会计波动。CFA 一级需要区分三类：公允价值套期（Fair Value Hedge）、现金流量套期（Cash Flow Hedge）和境外经营净投资套期（Net Investment Hedge）。

## 三种套期类型

### 1. 公允价值套期（Fair Value Hedge）

**对冲对象：** 已确认资产或负债的公允价值变动风险，或未确认的确定承诺（Firm Commitment）中可归属于特定风险的公允价值变动。

核心判断：关注的是**已经存在的项目，其公允价值会发生变化**。

例子：
- 企业持有铁矿石库存，担心未来价格下跌，卖出铁矿石期货进行对冲。
- 库存价格下降导致资产公允价值下降；空头期货头寸可能产生收益，抵消库存价值损失。

### 2. 现金流量套期（Cash Flow Hedge）

**对冲对象：** 已确认资产或负债相关的特定风险所导致的未来现金流变动，或高度可能发生的预期交易（Highly Probable Forecast Transaction）的现金流变动。

核心判断：关注的是**未来现金流金额或支付额的不确定性**。

例子：
- 企业发行浮动利率债券，未来利息支出会随参考利率变化。
- 企业签订利率互换（Interest Rate Swap），收取浮动利率、支付固定利率。
- 互换收到的浮动利息抵消债券支付的浮动利息，使净利息支出转为固定利率，从而降低未来现金流的不确定性。

会计提示（基础框架）：
- 有效套期部分的衍生品损益通常先计入其他综合收益（Other Comprehensive Income, OCI）。
- 当被套期现金流影响损益时，再按适用规则将相关金额重分类至损益。
- 无效套期部分通常计入当期损益。

### 3. 境外经营净投资套期（Net Investment Hedge）

**对冲对象：** 境外经营净投资（Net Investment in a Foreign Operation）的汇率风险。

核心判断：关注的是**境外子公司净资产折算价值的汇率变动风险**。

例子：
- 美国母公司持有外国子公司的股权或净资产。
- 母公司使用货币互换（Currency Swap）等工具对冲该境外经营净投资的汇率风险。
- 这属于 Net Investment Hedge，而不是普通的 Cash Flow Hedge。

## 三类套期对比

| 类型 | 对冲对象 | 典型关键词 | 典型例子 |
|---|---|---|---|
| Fair Value Hedge | 已确认资产/负债的公允价值变动 | Fair Value Change | 持有库存，卖出期货防止价格下跌 |
| Cash Flow Hedge | 未来现金流变动 | Cash Flow Variability | 浮动利率债务，收浮动付固定的利率互换 |
| Net Investment Hedge | 境外经营净投资的汇率风险 | Foreign Operation / FX | 对冲外国子公司净资产折算风险 |

## 本题判断

题目：Which scenario stands for a cash flow hedge?

- **A. 浮动利率债券发行人收取浮动、支付固定的利率互换**：对冲未来浮动利息支出的变化，属于 Cash Flow Hedge。
- **B. 钢铁公司卖出期货保护已持有铁矿石库存**：对冲已确认库存的公允价值变动，属于 Fair Value Hedge。
- **C. 美国出口商用货币互换对冲外国子公司的股权汇率风险**：对冲境外经营净投资，属于 Net Investment Hedge。

**正确答案：A。**

## 常见考试陷阱

1. 浮动利率债务 + Receive Floating / Pay Fixed Swap → 通常是 Cash Flow Hedge：用浮动收款抵消浮动债务利息支出。
2. 已持有存货 + 卖出商品期货防止价格下跌 → 通常是 Fair Value Hedge：对冲已确认资产的公允价值变化。
3. 外国子公司净投资 + 对冲汇率风险 → Net Investment Hedge。
4. 不能只看使用了哪一种衍生品来判断套期类型；同一种衍生品可能用于不同的套期目的。要看被对冲的风险和被套期项目。
5. Cash Flow Hedge 不是“任何未来发生的现金流都算”；要看是否对冲符合条件的现金流变动风险。

## 易混知识点 / Obsidian 链接

- [[Plain-Vanilla-Interest-Rate-Swaps]]
- [[Forward-vs-Futures-Contracts]]

## 我的错因 / 验证记录

- [ ] 能区分 Fair Value Hedge 与 Cash Flow Hedge
- [ ] 能识别 Net Investment Hedge
- [ ] 能解释为什么浮动利率债务配 Receive Floating / Pay Fixed Swap 是现金流量套期
