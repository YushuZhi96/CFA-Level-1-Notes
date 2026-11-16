---
subject: Quantitative Methods
topic: Excess Return
status: "待复习"
created: 2026-11-16
last-reviewed:
tags: [CFA-L1, Quantitative-Methods, LM01]
---

# 超额收益率（Excess Return）

> **题目编号：** Quant-Q004  
> **所属模块：** LM01 — Returns of Financial Assets and Instruments（金融资产与金融工具的收益）  
> **正确答案：** B

## 一句话理解

超额收益率（Excess Return）衡量某项投资相对于指定基准（Benchmark）的收益表现。基准可以是无风险利率（Risk-free Rate），也可以是市场指数等其他参考收益率；实际超额收益可以为正、为零或为负。

## 核心概念 / 定义

### 1. Excess Return（超额收益率）

超额收益率是投资收益相对于某个基准收益的差异或相对表现。必须先明确比较基准，才能解释超额收益。

常见基准包括：

- Risk-free Rate（无风险利率）：用于衡量投资超过无风险资产的收益。
- Market Index（市场指数）：用于衡量投资相对于市场基准的表现。

### 2. Risk Premium（风险溢价）

风险溢价是投资者事前为承担风险而要求的额外预期收益（Expected Compensation）。它是必要收益率构成中的一个概念，不等同于事后实现的超额收益率。

### 3. Benchmark Return（基准收益率）

基准收益率是用于比较投资表现的参考收益率。不同基准会产生不同的超额收益结果。

## 公式与变量

### 近似超额收益（Approximate Excess Return）

$$
ER_{\text{approx}} = R_i - R_b
$$

### 精确超额收益（Precise Excess Return）

$$
ER_{\text{precise}} = \frac{1+R_i}{1+R_b}-1
$$

其中：

- $R_i$：投资资产收益率（Investment Return）
- $R_b$：基准收益率（Benchmark Return）
- $ER$：超额收益率（Excess Return）

**理解：** 近似超额收益是两个收益率的简单差值；精确超额收益比较投资财富与基准财富的增长因子之比。

## 直观理解 / 记忆方法

假设某股票收益率为 12%，市场指数收益率为 8%。

近似超额收益：

$$
ER_{\text{approx}} = 12\%-8\%=4\%
$$

精确超额收益：

$$
ER_{\text{precise}} = \frac{1.12}{1.08}-1
\approx 3.70\%
$$

如果将无风险利率 3% 作为基准，则结果会不同：

$$
ER_{\text{approx}} = 12\%-3\%=9\%
$$

因此，超额收益必须结合基准解释。

## 常见考试陷阱

### 本题题干

Which of the following statements concerning excess return is most accurate?

以下关于超额收益率的陈述，哪一项最准确？

**A.** The excess return is the additional return investors require for bearing risk, and it is by definition non-negative.

错误。前半句描述的是风险溢价（Risk Premium），即投资者事前要求的风险补偿；超额收益是相对于基准实际实现的表现，可以为负数。

**B.** The excess return measures an investment's performance relative to a benchmark, which may be the risk-free rate or another reference rate such as a market index.

正确。超额收益衡量投资相对于指定基准的表现，基准可以是无风险利率，也可以是市场指数等其他参考收益率。

**C.** The precise excess return always equals the simple difference between the asset return and the risk-free rate.

错误。精确超额收益不是简单收益率相减，而是增长因子之比减去 1；此外，基准也不一定只能是无风险利率。

## 典型题型 / 判断路径

| 题目关键词 | 对应概念 |
|---|---|
| Relative to a benchmark | Excess Return |
| Above the risk-free rate | Excess Return using risk-free benchmark |
| Relative to a market index | Benchmark-relative / active performance |
| Additional return required for bearing risk | Risk Premium |
| By definition non-negative | 错误：realized excess return may be negative |
| Precise excess return | Growth-factor ratio, not simple difference |

**快速判断：**

1. 先找比较基准（Benchmark）。
2. 判断题目问的是实际相对表现（Excess Return），还是事前要求的风险补偿（Risk Premium）。
3. 如果强调 precise，使用增长因子之比；如果强调 approximate，使用简单收益率差。

## 易混知识点 / Obsidian 链接

- [[Risk-Premium-and-Required-Rate-of-Return|Risk Premium and Required Rate of Return]]
- [[Arithmetic-and-Geometric-Mean-Return|Arithmetic Mean Return vs. Geometric Mean Return]]
- Benchmark Return（基准收益率）
- Active Return（主动收益）
- Risk-free Rate（无风险利率）

## 我的错因 / 验证记录

- 本题正确答案：**B**。
- 核心考点：区分超额收益率与风险溢价；区分近似超额收益与精确超额收益。
- [ ] 能解释为什么实际超额收益可以为负
- [ ] 能区分 Risk Premium 与 Excess Return
- [ ] 能计算近似超额收益和精确超额收益
- [ ] 能识别不同基准对超额收益结果的影响
