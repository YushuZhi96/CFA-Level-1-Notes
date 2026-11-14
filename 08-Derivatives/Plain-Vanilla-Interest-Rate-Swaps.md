---
subject: Derivatives
topic: Plain Vanilla Interest Rate Swap
status: "待复习"
created: 2026-11-14
last-reviewed:
tags: [CFA-L1, Derivatives, Swaps, Interest-Rate]
---

# 普通利率互换（Plain Vanilla Interest Rate Swap）

## 一句话理解

普通利率互换通常是双方以同一名义本金（Notional Principal）为基础，交换固定利息与浮动利息现金流；名义本金通常不实际交换，双方在每个结算日将应付利息净额结算，而浮动利率通常在计息期开始时确定、期末支付。

## 核心概念 / 定义

### 1. 什么是普通利率互换？

普通利率互换（Plain Vanilla Interest Rate Swap）是最基本的利率互换形式：一方支付固定利率（Fixed Rate），另一方支付浮动利率（Floating Rate），双方按约定名义本金计算利息。

例如：
- 名义本金：USD 10,000,000
- 固定利率：年化 4%
- 浮动利率：参考 LIBOR
- 付息频率：每半年一次

名义本金只是计算利息的参考金额，普通利率互换中通常不会在开始或结束时交换本金。

### 2. 名义本金（Notional Principal）

- 用于计算双方利息支付金额。
- 普通利率互换通常不交换名义本金。
- 不要与货币互换（Currency Swap）混淆：货币互换通常涉及不同货币本金的交换，具体依合约条款而定。

### 3. 净额结算（Netting）

在每个结算日，双方通常只支付两笔利息现金流的净额，而不是分别全额支付。

例如：
- 固定利率方本期应付 200,000 美元。
- 浮动利率方本期应付 230,000 美元。
- 净额为 30,000 美元，由浮动利率方支付给固定利率方。

### 4. 浮动利率的确定与支付时间

普通利率互换通常采用 **期初确定、期末支付（Set in Advance, Paid in Arrears）** 的安排。

- **利率重设日（Reset Date）**：通常在计息期开始时，确定该计息期适用的浮动参考利率。
- **计息期（Accrual Period）**：使用已确定的利率计算该期间利息。
- **支付日（Payment Date）**：通常在计息期结束时支付该期间利息。

因此，浮动利率支付通常取决于计息期开始时确定的 LIBOR，而不是支付日当天的 LIBOR。

示意：
1. 1月初：重设利率，确定1月至3月适用的 LIBOR。
2. 1月至3月：按该利率累计计算浮动利息。
3. 3月底：支付1月至3月的利息。

注：具体重设日可能按合约约定和市场惯例提前若干营业日；考试基础框架关注“期初定息、期末付息”。

## 公式与变量

设：
- (N)：名义本金（Notional Principal）
- (R_f)：固定互换利率（Fixed Swap Rate）
- (R_L)：本计息期开始时确定的 LIBOR
- (Delta)：计息期年化时间比例（Accrual Fraction）

固定利息：

$$
\text{Fixed Payment}=N\times R_f\times\Delta
$$

浮动利息：

$$
\text{Floating Payment}=N\times R_L\times\Delta
$$

净额结算金额：

$$
\text{Net Payment}=|\text{Floating Payment}-\text{Fixed Payment}|
$$

支付方向由应付金额较大的一方决定。

## 常见考试陷阱

1. **名义本金不交换**：普通利率互换通常只交换利息现金流。
2. **净额结算**：每个结算日通常只支付双方利息的净额。
3. **期初定息、期末付息**：浮动利率通常在计息期开始时确定，不是支付日当天才确定。
4. **Reset Date ≠ Payment Date**：前者确定利率，后者支付利息。
5. **Interest Rate Swap ≠ Currency Swap**：普通利率互换通常不交换本金；货币互换通常涉及本金交换。
6. LIBOR 是历史上常见的浮动参考利率；实际市场已在多个司法辖区转向其他基准利率，但若题目明确使用 LIBOR，应按题干设定理解。

## 典型题型 / 判断路径

题目问：Which statement regarding a plain vanilla interest rate swap is least likely to be correct?

- Notional amount does not need to be exchanged at the beginning or end → 正确。
- Interest payments are netted on each settlement date → 正确。
- Floating rate payments depend on LIBOR on the payment date → 错误。

**正确答案：C。**

记忆：
- Notional → 通常不交换。
- Interest cash flows → 通常净额结算。
- Floating rate → 期初确定（Reset），期末支付（Payment）。

## 易混知识点 / Obsidian 链接

- [[Exchange-Traded-and-OTC-Derivatives]]
- [[Contingent-Claims-and-Forward-Commitments]]

## 我的错因 / 验证记录

- [ ] 能解释普通利率互换为什么通常不交换名义本金
- [ ] 能说明净额结算的支付方向
- [ ] 能区分 Reset Date 与 Payment Date
- [ ] 能独立计算固定与浮动利息及净额


## 固定互换利率（Fixed Swap Rate / Par Swap Rate）

### 一句话理解

固定互换利率是使互换固定端与浮动端在起始时点的现值相等的平价固定利率。它不是各期限零息利率的简单算术平均数，而是由整条折现曲线、各期现金流时间和隐含远期利率共同决定。

### 核心定价逻辑

在互换起始日，标准平价互换的价值为零：

$$
PV_{\text{Fixed Leg}}=PV_{\text{Floating Leg}}
$$

因此，固定端的票息率需要设定为一个盈亏平衡利率（Breakeven Rate），使双方现金流的现值相等。

### 平价固定互换利率公式

在单一折现曲线（Single-Curve Framework）、名义本金归一化为 1、浮动端在起始日刚重设且无额外利差等标准假设下：

$$
S=\frac{1-DF_n}{\sum_{i=1}^{n}\alpha_i DF_i}
$$

其中：
- $S$：固定互换利率（Fixed Swap Rate / Par Swap Rate）。
- $DF_i$：第 $i$ 个结算日的折现因子（Discount Factor）。
- $\alpha_i$：第 $i$ 个固定端计息期间的年化计息因子（Accrual Factor）。
- $n$：结算期数。
- $DF_n$：最后一个结算日的折现因子。

分母是各期固定现金流支付系数的折现总和，也称年金因子（Annuity Factor）。

### 与零息利率、远期利率的关系

- 零息利率（Zero Rate）用于构建折现因子（Discount Factor）。
- 隐含远期利率（Implied Forward Rate）用于推算未来各浮动计息期间适用的参考利率。
- 固定互换利率综合考虑各期现金流和折现权重，因此不是各期限零息利率的简单算术平均数。
- 在标准单曲线框架下，固定互换利率可理解为与隐含远期浮动现金流现值等价的固定票息率。

### 本题判断

Which interpretation of fixed swap rate is least correct?

- A. A multiperiod breakeven rate making expected future floating and fixed cash flows indifferent to investors. → 正确，表达了平价互换利率的经济含义。
- B. Arithmetic mean of the zero rates on each settlement date. → 错误，忽略不同期限现金流的折现权重及计息期间。
- C. The internal rate of return of cash flows based on implied forward rates through the settlement periods. → 在本题的基础框架下可视为正确的等价描述。

**正确答案：B。**

### 常见考试陷阱

1. Fixed Swap Rate ≠ Arithmetic Mean of Zero Rates。
2. 不同结算日的现金流需要按对应折现因子折现，不能简单等权平均。
3. Zero Rates 用于折现；Forward Rates 用于推算未来浮动利率。
4. Fixed Swap Rate 是使固定端和浮动端现值相等的平价利率。
5. 上述闭式公式依赖单一折现曲线等简化假设；实际市场多曲线框架下，需要使用相应的折现曲线和远期曲线。

## 我的错因 / 验证记录

- [ ] 能解释为什么固定互换利率不是零息利率的算术平均值
- [ ] 能区分 Zero Rate、Forward Rate 和 Fixed Swap Rate
- [ ] 能理解折现因子和计息因子在公式中的作用


## 互换合约价值（Swap Contract Value）

### 1. 成立时的价值（Value at Initiation）

一份新签订、按市场条件公平定价且没有额外前期支付的互换合约，其初始价值通常为零：

$$
V_{\text{Swap},0}=0
$$

原因是固定互换利率（Fixed Swap Rate）被设定为使固定端和浮动端的现值相等：

$$
PV_{\text{Receive Leg}}=PV_{\text{Pay Leg}}
$$

因此，合约在成立时对双方都没有净价值优势。

### 2. 合约存续期间的价值（Value During the Life of the Swap）

互换价值不会在整个合同期限内固定不变。市场利率、折现曲线和剩余现金流变化后，原互换的价值也会变化。

从某一方的角度：

$$
V_{\text{Swap},t}=PV_{\text{Receive Leg},t}-PV_{\text{Pay Leg},t}
$$

注意：
- 原合同的固定互换利率通常保持不变。
- 浮动利率会按合同约定定期重设。
- Swap Value 会随着市场条件变化而波动。

### 3. Swap 与一系列 Forward / FRA 的关系

一份多期利率互换可以理解为一系列不同结算期间的远期利率协议（Forward Rate Agreements, FRAs）。

在成立时：
- 单独每一期的组成远期合约可能具有正、负或零的初始价值。
- 互换整体的初始价值等于所有组成远期合约价值之和。
- 对公平定价的互换，这些组成合约的价值相互抵销，组合价值为零。

$$
V_{\text{Swap},0}=\sum_{i=1}^{n}V_{\text{Forward},i,0}=0
$$

因此，**每份组成远期的价值不必为零，但所有组成远期的价值总和必须为零**（在公平定价的互换成立时）。

### 4. 本题判断

The swap contract value:

- A. is zero at initiation. → 正确。标准公平定价互换初始价值为零。
- B. is fixed over the life of the contract. → 错误。互换价值会随市场利率和剩余现金流变化；固定的是合同约定的固定互换利率，而不是 Swap Value。
- C. is the same with the value of each component forward contract. → 错误。互换价值等于所有组成远期合约价值的总和，而不是等于每一份组成远期的价值。

**正确答案：A。**

### 易混概念速查

| 概念 | 成立时 | 存续期间 |
|---|---|---|
| Fixed Swap Rate | 按市场条件确定 | 原合同通常固定 |
| Floating Rate | 按当期参考利率确定 | 按合同定期重设 |
| Swap Value | 公平定价时通常为零 | 随市场条件变化 |
| Individual Component Forward Value | 可以非零 | 随市场条件变化 |
| Combined Component Forward Values | 合计为零 | 合计等于 Swap Value |

### 我的错因 / 验证记录

- [ ] 能解释为什么公平定价互换初始价值为零
- [ ] 能区分 Fixed Swap Rate 与 Swap Value
- [ ] 能解释互换价值为什么会随市场利率变化
- [ ] 能区分单份组成远期价值与全部组成远期价值之和


## 互换价值的计算（Calculation of Swap Value）

互换价值等于未来各期**净现金流（Net Cash Flows）**的现值之和。也可以分别计算收取端与支付端的现值，再相减。

从某一方的角度：

$$
V_{\text{Swap},t}
=
\sum_{i=1}^{n}DF(t,T_i)\times E_t[NCF_i]
$$

其中：
- $DF(t,T_i)$：从估值日 $t$ 到第 $i$ 个支付日 $T_i$ 的折现因子。
- $E_t[NCF_i]$：在估值日 $t$ 对第 $i$ 期净现金流的预期；净现金流按该方视角定义为收取金额减去支付金额。
- $n$：剩余结算期数。

等价表达：

$$
V_{\text{Swap},t}
=
PV_{\text{Receive Leg},t}
-
PV_{\text{Pay Leg},t}
$$

### 本题判断

The swap value is calculated by:

- A. Adding up the present value of the fixed payments in the future. → 不完整，只计算固定端，忽略另一端。
- B. Adding up the present value of the floating payments in the future. → 不完整，只计算浮动端，忽略另一端。
- C. Adding up the present value of the net cash payments in the future. → 正确，计算每期净现金流并折现，再将各期现值加总。

**正确答案：C。**

### 现金流方向提醒

- 若从固定利率支付方（Pay Fixed）的角度，净现金流 = 收到的浮动现金流 − 支付的固定现金流。
- 若从固定利率收取方（Receive Fixed）的角度，净现金流 = 收到的固定现金流 − 支付的浮动现金流。
- 因此 Swap Value 的正负取决于观察者持有哪一侧；不要脱离交易方向只写一个固定正负号。

### 易错点

1. Swap Value 不是固定端现值单独一项。
2. Swap Value 也不是浮动端现值单独一项。
3. 应计算收取端与支付端的差额，或直接计算每期净现金流的现值总和。
4. 每个结算日通常先对双方应付利息进行净额结算（Net Settlement）；估值时则把未来净现金流折现到当前。
