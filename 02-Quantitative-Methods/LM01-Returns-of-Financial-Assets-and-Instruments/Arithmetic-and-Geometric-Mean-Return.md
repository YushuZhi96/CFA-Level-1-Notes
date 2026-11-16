---
subject: Quantitative Methods
topic: Arithmetic and Geometric Mean Return
status: "待复习"
created: 2026-11-16
last-reviewed:
tags: [CFA-L1, Quantitative-Methods, LM01]
---

# 算术平均收益率与几何平均收益率（Arithmetic Mean Return vs. Geometric Mean Return）

> **题目编号：** Quant-Q001  
> **所属模块：** LM01 — Returns of Financial Assets and Instruments（金融资产与金融工具的收益）  
> **正确答案：** B

## 一句话理解

算术平均收益率（Arithmetic Mean Return）是各期收益率的简单平均；几何平均收益率（Geometric Mean Return）是考虑复利后的每期平均增长率。收益率波动越大，在其他条件相同的情况下，两者的差距通常越大。

## 核心概念 / 定义

### 1. Arithmetic Mean Return（算术平均收益率）

将各期收益率直接相加，再除以期间数量。它不把前一期的收益重新计入下一期的平均计算。

### 2. Geometric Mean Return（几何平均收益率）

将各期增长因子（1 + return）连乘，再开 n 次方，最后减去 1。它反映投资在多个期间内的复合增长率（Compound Growth Rate），考虑了投资基数随收益变化而变化的影响。

### 3. Compounding Effect（复利效应）

每一期的收益或亏损都会改变下一期的投资基数，因此多期收益不能简单地把各期收益率相加。

### 4. Volatility Drag（波动损耗）

当收益率存在波动时，复合增长会受到波动影响。对于相同算术平均收益率的收益序列，波动越大，几何平均收益率通常越低，算术平均与几何平均之间的差距越大。

## 公式与变量

### 算术平均收益率

$$
AM = \frac{1}{n}\sum_{t=1}^{n} r_t
$$

### 几何平均收益率

$$
GM = \left[\prod_{t=1}^{n}(1+r_t)\right]^{1/n}-1
$$

**变量说明：**

- $r_t$：第 t 期收益率（Periodic Return）
- $n$：期间数量（Number of Periods）
- $\prod$：连乘符号（Product）
- $AM$：算术平均收益率（Arithmetic Mean Return）
- $GM$：几何平均收益率（Geometric Mean Return）

**适用条件：** 几何平均收益率用于概括多个期间的复合增长表现；各期增长因子需要能够进行连乘。通常要求各期收益率大于 -100%。

### 两者关系

$$
AM \geq GM
$$

当各期收益率完全相同时，$AM=GM$；当各期收益率存在波动时，通常 $AM>GM$。

小幅收益率条件下，可用下式帮助理解波动对复合收益的影响（近似关系，不替代几何平均精确公式）：

$$
GM \approx AM - \frac{1}{2}\sigma^2
$$

其中 $\sigma^2$ 为各期收益率的方差（Variance）。

## 直观理解 / 记忆方法

假设初始投资为 100 元，第一年收益率为 +20%，第二年收益率为 -20%。

| 期间 | 收益率 | 期末投资价值 |
|---|---:|---:|
| 初始 | — | 100 |
| 第一年 | +20% | 120 |
| 第二年 | -20% | 96 |

算术平均收益率：

$$
AM = \frac{20\%+(-20\%)}{2}=0\%
$$

几何平均收益率：

$$
GM = [(1+20\%)(1-20\%)]^{1/2}-1
$$

$$
GM = \sqrt{0.96}-1 \approx -2.02\%
$$

**理解：** 一涨一跌并不会回到原点。上涨 20% 后，投资基数变为 120；随后下跌 20%，损失 24，最终只剩 96。算术平均为 0%，但实际复合年收益率约为 -2.02%。

## 常见考试陷阱

### 本题题干

Which of the following statements concerning the arithmetic mean return and the geometric mean return is most accurate?

以下关于算术平均收益率与几何平均收益率的陈述，哪一项最准确？

**A.** The arithmetic mean return reflects the fact that the invested base changes over time as a result of capital appreciation and depreciation.

错误。投资基数因资本增值或贬值而随时间变化，是几何平均收益率所反映的复利特征，不是算术平均收益率的特点。

**B.** The difference between the arithmetic and the geometric mean return widens as the variability of the periodic returns increases.

正确。各期收益率波动性（Variability）增加时，在其他条件相同的情况下，算术平均收益率与几何平均收益率之间的差距通常扩大。

**C.** The geometric mean return is computed as the simple average of (1 + r_t) across all periods, minus 1.

错误。这是把几何平均误写成简单平均。几何平均应先将各期增长因子连乘，再开 n 次方，最后减去 1。

## 典型题型 / 判断路径

看到以下关键词时，优先判断对应概念：

| 题目关键词 | 对应知识点 |
|---|---|
| Simple average of periodic returns | Arithmetic Mean |
| Compound growth rate | Geometric Mean |
| Invested base changes over time | Geometric Mean |
| Variability of periodic returns increases | AM–GM gap widens |
| Long-term multi-period performance | Geometric Mean |
| Average return for one period | Arithmetic Mean |

**快速判断：**

1. 题目问各期收益率的简单平均：使用算术平均。
2. 题目问多期实际复合增长：使用几何平均。
3. 题目问收益率波动增加的影响：记住几何平均相对算术平均会受到更明显的波动损耗。

## 易混知识点 / Obsidian 链接

- Arithmetic Mean Return（算术平均收益率）
- Geometric Mean Return（几何平均收益率）
- Compounding Effect（复利效应）
- Volatility Drag（波动损耗）
- Variance（方差）

## 我的错因 / 验证记录

- 本题正确答案：**B**。
- 核心考点：收益率波动性与算术平均、几何平均之间的关系。
- [ ] 不看解析能独立解释 AM 与 GM 的区别
- [ ] 能独立计算多期几何平均收益率
- [ ] 能解释为什么收益率波动会扩大 AM–GM 差距
- [ ] 能独立完成一道同类新题

## 参考资料

- CFA Institute, [2027 Level I Topic Outlines](https://www.cfainstitute.org/sites/default/files/2027levelitopicoutline_online.pdf)
- CFA Institute, [2027 Level I Curriculum Errata Notice](https://www.cfainstitute.org/sites/default/files/docs/programs/cfa-program/candidate-resources/2027-cfa-program-level-1-notice.pdf)
