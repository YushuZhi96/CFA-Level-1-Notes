---
subject: Derivatives
topic: Contingent Claims and Forward Commitments
status: "待复习"
created: 2026-11-14
last-reviewed:
tags: [CFA-L1, Derivatives, Contract-Types]
---

# 或有索取权与远期承诺（Contingent Claims vs. Forward Commitments）

## 一句话理解

**或有索取权（Contingent Claims）**的收益取决于未来标的价格或事件，典型代表是期权；**远期承诺（Forward Commitments）**则要求交易双方按约定在未来履行合同，典型代表是远期、期货和互换。

## 核心概念 / 定义

### 1. 或有索取权（Contingent Claims）

指收益或履约结果取决于未来某种状态或标的资产表现的衍生品。CFA 一级基础分类中，最典型的代表是**期权（Options）**。

- 期权买方支付期权费（Option Premium），获得权利，而不是必须履行的义务。
- 买方可以根据到期时的市场条件决定是否行权（Exercise）。
- 看涨期权（Call Option）：赋予买方按约定价格买入标的的权利。
- 看跌期权（Put Option）：赋予买方按约定价格卖出标的的权利。
- 期权买方通常可以选择不行权；若不考虑其他费用，其最大损失通常为已支付的期权费。

### 2. 远期承诺（Forward Commitments）

指交易双方约定在未来某一时间，按照预先约定的条款进行交易或交换现金流的衍生品。

典型代表：
- 远期（Forwards）
- 期货（Futures）
- 互换（Swaps）

双方原则上都承担合同义务，而不是由一方单方面选择是否履约。市场价格变化会影响合约价值，但通常不会自动免除合同义务。

## 两类衍生品对比

| 比较维度 | 或有索取权 Contingent Claims | 远期承诺 Forward Commitments |
|---|---|---|
| 典型工具 | 期权 Options | 远期 Forwards、期货 Futures、互换 Swaps |
| 核心特征 | 权利，买方可选择是否行权 | 双方承担合同约定的履约义务 |
| 买方/持有人 | 有权行权，也可放弃 | 按合同约定承担履约义务 |
| 价值驱动 | 取决于标的价格或相关事件 | 取决于标的价格、利率等市场变量 |
| 典型风险 | 买方期权费损失；卖方承担或有履约义务 | 合约价值变化及交易对手履约风险 |

## 用例子理解

假设某股票当前价格为 100 元。

**期权（Option）**：你支付 5 元期权费，买入行权价为 100 元的看涨期权。到期股价为 120 元时，你可以选择行权；若到期股价为 80 元，你可以放弃行权。买方有权利，没有必须买入股票的义务。

**远期（Forward）**：你与交易对手约定三个月后以 100 元买入该股票。到期时无论市场价格为 120 元还是 80 元，双方原则上都应按合约约定履行。

## 常见考试陷阱

1. **Equity forwards（股票远期）不是 Contingent Claims**，它属于 Forward Commitments。
2. **Currency swaps（货币互换）属于 Forward Commitments**，双方约定交换不同货币的现金流或本金。
3. **Stock options（股票期权）属于 Contingent Claims**，因为期权买方可以选择是否行权。
4. 不要把“合约价值随市场价格变化”理解成“或有索取权”。远期、期货和互换的价值同样会随市场变量变化；分类关键在于合约权利义务结构。
5. 期权买方有权利而无行权义务；期权卖方（Writer）则承担相应的或有履约义务。

## 典型题型 / 判断路径

题目：The contingent claims most likely include:

- Equity forwards → Forward Commitments
- Currency swaps → Forward Commitments
- Stock options → Contingent Claims

**正确答案：C. Stock options（股票期权）。**

快速记忆：
- **Option = Right, not obligation（权利，而非义务）**
- **Forward / Futures / Swaps = Contractual obligation（合同履约义务）**

## 易混知识点 / Obsidian 链接

- [[Long-Short-Call-Put]]
- [[Exchange-Traded-and-OTC-Derivatives]]

## 我的错因 / 验证记录

- [ ] 不看解析能区分 Contingent Claims 与 Forward Commitments
- [ ] 能解释为什么远期和互换不属于 Contingent Claims
- [ ] 能独立完成一道同类分类题
