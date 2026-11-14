---
subject: Derivatives
topic: Futures Price vs. Forward Price
status: "待复习"
created: 2026-11-14
last-reviewed:
tags: [CFA-L1, Derivatives, Futures, Forwards, Pricing]
---

# 期货价格与远期价格的差异（Futures Price vs. Forward Price）

## 一句话理解

在其他条件相同的情况下，期货与远期价格的差异取决于**期货价格与利率的相关性（Correlation between Futures Prices and Interest Rates）**。正相关时，期货价格通常高于远期价格；负相关时，期货价格通常低于远期价格；不相关时，两者通常相等。

## 为什么会有差异？

关键在于每日盯市（Daily Mark-to-Market）：

- **期货（Futures）**：每天结算盈亏，盈利会提前收到并可再投资，亏损则需要提前支付。
- **远期（Forward）**：通常在到期时集中结算，期间不进行期货式的每日盈亏结算。

因此，期货头寸的每日现金流会与当时的利率发生联系，利率与期货价格的相关性会影响再投资或融资收益。

## 三种相关性情形

### 1. 正相关（Positive Correlation）

当期货价格上涨时，利率也较高：
- 期货多头（Long Futures）每日收到盈利。
- 收到的盈利可以在较高利率环境下再投资，获得较高利息。
- 当期货价格下跌时，利率相对较低，多头需要支付亏损，但融资成本相对较低。

因此，期货多头相较于远期多头具有有利的现金流时点效应。为使两种合约在起始时价值相当，期货价格通常高于远期价格。

**结论：Futures Price > Forward Price。**

### 2. 负相关（Negative Correlation）

当期货价格上涨时，利率反而较低：
- 多头收到的盈利只能在较低利率下再投资。
- 当期货价格下跌时，利率较高，多头需要在较高利率环境下筹措资金支付亏损。

每日结算的现金流时点效应对期货多头不利，因此期货价格通常低于远期价格。

**结论：Futures Price < Forward Price。**

### 3. 不相关（Uncorrelated）

若期货价格与利率不相关，提前收到盈利或支付亏损的利率时点优势平均而言不明显。

**结论：Futures Price ≈ Forward Price。**

## 方向速查表

| 期货价格与利率相关性 | 期货价格与远期价格关系 |
|---|---|
| 正相关 Positive Correlation | Futures Price > Forward Price |
| 负相关 Negative Correlation | Futures Price < Forward Price |
| 不相关 Uncorrelated | Futures Price ≈ Forward Price |

## 本题判断

If the futures price is higher than an identical forward price, the reason might be that:

- Futures prices and interest rates are positively correlated → 正确。
- Futures prices and interest rates are negatively correlated → 错误，通常会使期货价格低于远期价格。
- Futures prices and interest rates are uncorrelated → 错误，通常两者价格相等。

**正确答案：A. Futures prices and interest rates are positively correlated.**

## 非常重要的易混点：利率期货报价

不要把本题的“期货价格与利率正相关”与短期利率期货的常见报价公式混淆：

$$
\text{Short-term Interest Rate Futures Quote}=100-\text{MRR}
$$

在这种短期利率期货报价惯例中，报价与 MRR 是**负相关**的，因为参考利率上升，报价下降。

而本题讨论的是一般期货价格与市场利率之间的相关性如何影响 Futures Price 与 Forward Price 的相对水平。这是每日盯市现金流的估值效应，两者讨论的不是同一个变量关系。

## 相关概念

- **凸性调整（Convexity Adjustment）**：由于期货每日结算与远期到期结算的差异，在利率与期货价格存在相关性时，两者价格可能出现差异。
- **再投资收益（Reinvestment Gain）**：提前收到的期货盈利可以按当时利率再投资。
- **融资成本（Funding Cost）**：期货亏损需要提前支付，可能产生融资成本。

## 记忆口诀

- Positive correlation → Futures above Forwards.
- Negative correlation → Futures below Forwards.
- No correlation → Futures approximately equal Forwards.

## 我的错因 / 验证记录

- [ ] 能解释为什么每日盯市使期货价格与远期价格可能不同
- [ ] 能根据相关性判断 Futures 与 Forward 的价格高低
- [ ] 能区分一般期货价格与利率的相关性、以及短期利率期货的 100 − MRR 报价关系
