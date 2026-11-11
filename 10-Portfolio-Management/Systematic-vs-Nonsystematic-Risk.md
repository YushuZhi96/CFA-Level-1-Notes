---
subject: Portfolio Management
topic: Systematic Risk, Nonsystematic Risk and Diversification
status: "🟡 错题已解析，待独立验证"
created: 2026-11-11
last-reviewed: 2026-11-11
tags: [CFA-L1, Portfolio-Management, Systematic-Risk, Unsystematic-Risk, Diversification, CAPM]
---

# 系统性风险、非系统性风险与分散化（Systematic vs Nonsystematic Risk & Diversification）

[[10-Portfolio-Management/INDEX|← 返回投资组合管理目录]]

## 一句话理解

在标准的资本市场理论与 CAPM（Capital Asset Pricing Model，资本资产定价模型）框架下：

- **系统性风险（Systematic Risk）**：影响整个市场的共同风险，无法仅靠持有更多不同股票而消除；它是 CAPM 中获得风险溢价的风险。
- **非系统性风险（Nonsystematic / Unsystematic Risk）**：公司或资产特有的风险，可以通过分散化投资降低；在 CAPM 均衡下，不获得单独的风险溢价。
- **分散化的边际收益递减（Diminishing Marginal Benefit of Diversification）**：持有的、并非完全相关的股票越来越多时，非系统性风险通常**下降，但下降得越来越慢**。

## 一、两类风险的区别

| 维度 | 系统性风险（Systematic Risk） | 非系统性风险（Nonsystematic Risk） |
|---|---|---|
| 别称 | Market Risk（市场风险）、Non-diversifiable Risk | Idiosyncratic / Firm-Specific Risk（特有风险）、Diversifiable Risk |
| 来源 | 整体市场、宏观经济、利率与系统性冲击 | 企业经营、产品失误、管理层或个别事件 |
| 影响范围 | 许多资产共同受到影响 | 主要影响特定公司或少数资产 |
| 能否靠增加不同股票分散 | 不能消除 | 可以降低，充分分散时可接近零 |
| CAPM 均衡中的风险补偿 | 有 | 没有单独补偿 |
| 常用风险指标 | Beta（$\beta$） | 与市场无关的残差/特有风险 |

**易错边界：**“系统性风险无法被分散”不等于“投资者不能通过降低股票仓位、对冲等措施改变市场风险敞口”；只是说**仅靠持有更多市场内股票不能消除共同市场风险**。

## 二、为什么 CAPM 只补偿系统性风险？

证券市场线（Security Market Line, SML）的 CAPM 公式：

$$
\boxed{E(R_i)=R_f+\beta_i[E(R_M)-R_f]}
$$

- $R_f$：无风险收益率（Risk-Free Rate）；
- $\beta_i$：该资产对市场组合的系统性风险暴露（Beta）；
- $E(R_M)-R_f$：市场风险溢价（Market Risk Premium）。

这里的风险溢价由 **Beta** 决定，并没有给公司特有风险单独加价。这是因为理性投资者可以通过充分分散投资降低非系统性风险，均衡市场不为可免费分散掉的风险提供额外预期回报。

**注意**：这是 CAPM 的理论均衡结论；并非说现实中承担个股风险一定没有利润或完全没有风险溢价差异。

## 三、股票数量增加时，非系统性风险如何变化？

### 1. 先理解英文

| 英文 | 中文 | 趋势 |
|---|---|---|
| Increase at a decreasing rate | 以递减速度增加 | **仍在增加**，只是增速越来越慢 |
| **Decrease at a decreasing rate** | **以递减速度下降** | **仍在减少**，只是降幅越来越小 |
| Decrease at an increasing rate | 以递增速度下降 | 仍在减少，而且降幅越来越大 |

增加不同股票的初期，分散效果通常显著；持有较多股票后，进一步增加股票的边际分散效果会逐渐变小。因此正确描述是 **decrease at a decreasing rate**。

### 2. 简化模型（理解机制，不要求死背）

假设 $n$ 只股票**等权**，每只股票的收益率方差均为 $\sigma^2$，任意两只股票的两两相关系数均为 $\rho$，其中 $0\leq\rho<1$。

那么投资组合方差为：

$$
\boxed{\sigma_p^2=\rho\sigma^2+\frac{(1-\rho)\sigma^2}{n}}
$$

从数学上把它理解为：

$$
\underbrace{\rho\sigma^2}_{\text{共同波动部分，分散化后仍存在}}
+
\underbrace{\frac{(1-\rho)\sigma^2}{n}}_{\text{随股票数量增加而下降的部分}}
$$

如果定义 $K=(1-\rho)\sigma^2>0$，增加 1 只股票后，第二部分方差的下降量为：

$$
\frac{K}{n}-\frac{K}{n+1}=\boxed{\frac{K}{n(n+1)}}
$$

当 $n$ 越大，下降量越小：这就解释了 **decrease at a decreasing rate**。

极限：

$$
\lim_{n\to\infty}\frac{(1-\rho)\sigma^2}{n}=0
$$

因此总方差趋向于 $\rho\sigma^2$；在这一简化模型中，这代表不能靠增加股票数量消除的共同波动部分。

**重要前提**：现实资产方差、相关系数和权重并不总相同；“越多越好”不是无条件成立的规律。选入高度相关的新股票，分散效果可能很有限。这里的分解是教学模型，不能不加条件地把任意投资组合的标准差拆成两项直接相加。

### 3. 数字例子

假设各股票标准差均为 $20\%$，两两相关系数为 $0.25$，则：

$$
\sigma_p^2=0.25(0.20)^2+\frac{0.75(0.20)^2}{n}
=0.01+\frac{0.03}{n}
$$

| 股票数量 $n$ | 共同波动部分（方差） | 可分散部分（方差） | 总方差 |
|---|---:|---:|---:|
| 1 | 0.0100 | 0.0300 | 0.0400 |
| 2 | 0.0100 | 0.0150 | 0.0250 |
| 5 | 0.0100 | 0.0060 | 0.0160 |
| 10 | 0.0100 | 0.0030 | 0.0130 |
| 20 | 0.0100 | 0.0015 | 0.0115 |

可分散部分持续减少，但越往后下降越少。

## 四、本次两道 CFA 题（概念与错因）

### 题目 1：系统性风险与非系统性风险

问：*Which of the following statements about systematic risk and nonsystematic risk is correct?*

- Statement 1: *Systematic risk can be diversified by constructing a diversified portfolio.* → **错误**：被分散的是非系统性风险，不是系统性风险。
- Statement 2: *Investors are compensated for bearing nonsystematic risk.* → **错误**：CAPM 均衡中没有对可分散的特有风险支付单独风险溢价。

**答案：C — None of them（两项均不正确）。**

### 题目 2：股票数量增加时非系统性风险如何变化

问：*As the number of stocks in the portfolio increases, the unsystematic risk of a portfolio tends to:*

- **A. increase at a decreasing rate.** → 错误：它表示“越来越慢地增加”，方向反了。
- **B. decrease at a decreasing rate.** → **正确**：风险下降，但下降速度越来越慢。
- **C. decrease at an increasing rate.** → 错误：它表示下降速度越来越快，与常见分散化边际效益递减相反。

**答案：B。此前错选 A，错因是混淆 increase 和 decrease 的方向，而不是是否存在边际效应。**

## 五、与已有笔记联系

- [[CML-and-SML|CML 与 SML]]：SML 为什么用 Beta 衡量系统性风险；CML 为什么用标准差衡量有效组合的总风险。
- [[Markowitz-Efficient-Frontier|Markowitz 有效前沿]]：相关系数与协方差如何影响组合风险和分散效果。
- [[Variance-and-Standard-Deviation|方差与标准差]]：风险分解的公式中用的是**方差**；总标准差需对总方差开平方。

## 六、考试速记与复习检查

- **Systematic = Non-diversifiable = Compensated in CAPM**。
- **Nonsystematic = Diversifiable = Not separately compensated in CAPM**。
- **More diversified stocks → unsystematic risk decreases at a decreasing rate**。
- CML 横轴：$\sigma$（总风险）；SML 横轴：$\beta$（系统性风险）。

- [ ] 能分辨系统性与非系统性风险的中英文别称
- [ ] 能解释 CAPM 为何只对系统性风险提供补偿
- [ ] 能准确翻译 increase/decrease at a decreasing/increasing rate
- [ ] 能说明分散化效果为什么边际递减
- [ ] 能在简单等权同方差相关模型下理解 $K/n$ 与边际下降量
