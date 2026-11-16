---
subject: Quantitative Methods
topic: Maturity Risk Premium
status: "待复习"
created: 2026-11-16
last-reviewed:
tags: [CFA-L1, Quantitative-Methods, LM01, Fixed-Income]
---

# 期限风险溢价（Maturity Risk Premium）

> **题目编号：** Quant-Q003  
> **所属模块：** LM01 — Returns of Financial Assets and Instruments（金融资产与金融工具的收益）  
> **正确答案：** A

## 一句话理解

期限风险溢价（Maturity Risk Premium, MRP）是投资者因持有较长期限债务证券、承担更高利率风险等期限相关风险，而要求获得的额外收益补偿。

## 核心概念 / 定义

### 1. Maturity Risk Premium（期限风险溢价）

长期债券的市场价格对利率变化通常更敏感。若市场利率上升，长期债券价格通常比短期债券价格下跌得更多。因此，投资者可能要求额外收益，以补偿持有长期债券所承担的期限相关风险。

### 2. T-bill vs. T-bond

- **T-bill（Treasury Bill，短期国库券）**：美国财政部发行的短期债务证券，期限通常为一年以内。
- **T-bond（Treasury Bond，长期国债）**：美国财政部发行的长期债务证券，期限通常超过十年。

两者都由美国财政部发行，通常被视为违约风险可以忽略的政府证券。它们的期限不同，长期证券通常具有更高的利率风险。

### 3. Interest Rate Risk（利率风险）

利率风险是指市场利率变化导致债券价格波动的风险。一般而言，在其他条件相同的情况下，债券期限越长、久期（Duration）越高，价格对收益率变化越敏感。

## 公式与变量

本题考查的是收益率组成部分的概念辨析，而非数值计算。可用概念性分解帮助理解：

$$
R \approx R_{\text{Real Risk-free}} + IP + DRP + LP + MRP
$$

其中：

- $R_{\text{Real Risk-free}}$：实际无风险利率（Real Risk-free Rate）
- $IP$：通货膨胀溢价（Inflation Premium）
- $DRP$：违约风险溢价（Default Risk Premium）
- $LP$：流动性溢价（Liquidity Premium）
- $MRP$：期限风险溢价（Maturity Risk Premium）

**注意：** 这是用于理解债券必要收益率构成的概念性分解。不同债券的具体组成取决于其风险特征；市场收益率还可能反映对未来短期利率的预期。

## 直观理解 / 记忆方法

比较 T-bill 与 T-bond：

| 对比维度 | T-bill | T-bond |
|---|---|---|
| 期限 | 短期，通常一年以内 | 长期，通常超过十年 |
| 发行人 | 美国财政部 | 美国财政部 |
| 违约风险 | 通常可忽略 | 通常可忽略 |
| 利率风险 | 相对较低 | 通常较高 |
| 期限风险补偿 | 相对较低 | 通常较高 |

**核心逻辑：** 长期债券对利率变化更敏感，投资者可能要求额外补偿，因此期限风险溢价可以解释 T-bill 与 T-bond 之间的收益率差异。

## 常见考试陷阱

### 本题题干

A portfolio manager is explaining the difference in the rates of return between T-bill and T-bond. Which of the following is the most appropriate component?

一位投资组合经理正在解释短期国库券（T-bill）与长期国债（T-bond）之间收益率的差异。以下哪一个组成部分最适合解释这种差异？

**A. Maturity risk premium（期限风险溢价）**

正确。T-bond 期限更长，通常承担更高的利率风险，投资者可能要求额外的期限风险补偿。

**B. Default risk premium（违约风险溢价）**

错误。两者均由美国财政部发行，通常被视为违约风险可以忽略，因此违约风险溢价不是解释两者收益率差异的主要组成部分。

**C. The real risk-free rate of return（实际无风险收益率）**

错误。实际无风险利率是无风险收益率体系中的基础组成部分，不是本题所强调的期限差异来源。

## 典型题型 / 判断路径

| 题目关键词 | 对应概念 |
|---|---|
| Difference between short-term and long-term Treasury yields | Maturity Risk Premium |
| Longer maturity | Greater interest rate risk |
| Greater sensitivity to interest rate changes | Duration / Interest Rate Risk |
| Risk of issuer failing to pay | Default Risk Premium |
| Compensation for expected inflation | Inflation Premium |
| Real return with negligible risk | Real Risk-free Rate |

**快速判断：**

1. 比较同一主权发行人的短期与长期债券，优先考虑期限风险溢价。
2. 题目强调发行人可能无法偿债，考虑违约风险溢价。
3. 题目强调购买力被通胀侵蚀，考虑通货膨胀溢价。
4. 题目强调实际、无风险的时间价值，考虑实际无风险利率。

## 易混知识点 / Obsidian 链接

- [[Risk-Premium-and-Required-Rate-of-Return|Risk Premium and Required Rate of Return]]
- Risk-free Rate（无风险利率）
- Default Risk Premium（违约风险溢价）
- Inflation Premium（通货膨胀溢价）
- Liquidity Premium（流动性溢价）
- Duration（久期）

## 我的错因 / 验证记录

- 本题正确答案：**A**。
- 核心考点：区分期限风险溢价、违约风险溢价与实际无风险利率。
- [ ] 能解释长期债券为什么通常具有更高的利率风险
- [ ] 能区分 Maturity Risk Premium 与 Default Risk Premium
- [ ] 能说明久期与债券价格对利率变化敏感度之间的关系
