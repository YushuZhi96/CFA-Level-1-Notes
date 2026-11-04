---
subject: Financial Statement Analysis
topic: Non-GAAP Financial Measures
status: "🟡 解析能懂，待独立验证"
created: 2026-11-04
last-reviewed:
tags: [CFA-L1, FSA, Non-GAAP, SEC, Disclosure]
---

# 非 GAAP 财务指标与 SEC 披露要求（Non-GAAP Financial Measures）

## 一、一句话理解

**Non-GAAP Financial Measures（非 GAAP 财务指标）**是企业在依照公认会计原则（GAAP）形成的指标基础上，作出特定调整后披露的补充性财务指标。它们可能有助于理解经营业绩，但也可能因调整口径不一致或选择性剔除费用而误导投资者。

**GAAP 指标不能被 Non-GAAP 指标替代。**

## 二、基础概念对比

| 项目 | GAAP Measures | Non-GAAP Measures |
|---|---|---|
| 中文 | 公认会计准则财务指标 | 非 GAAP 财务指标 |
| 编制基础 | 适用会计准则 | 管理层定义的调整口径，仍须满足披露规定 |
| 常见例子 | Net Income、GAAP EPS、Operating Income | Adjusted Net Income、Adjusted EPS、Adjusted EBITDA |
| 主要用途 | 提供标准化的财务表现 | 补充解释特定调整后的财务表现 |
| 主要风险 | 会计估计等判断仍会影响数据 | 调整项目选择性、跨期不可比、误导性呈现 |

- **SEC（Securities and Exchange Commission，美国证券交易委员会）**：美国证券市场的重要监管机构。
- **SEC Filings（SEC 申报文件）**：上市公司向 SEC 提交的报告等文件。
- **Reconciliation（调节表 / 勾稽调节）**：从最直接可比的 GAAP 指标出发，列出调整项目，推导 Non-GAAP 指标。

## 三、SEC 对 Non-GAAP 指标的主要要求

针对适用的 SEC 申报文件，重点掌握：

| 要求 | 英文 | 考试判断 |
|---|---|---|
| 展示最直接可比的 GAAP 指标 | Most Directly Comparable GAAP Measure | 需要 |
| 提供 GAAP 与 Non-GAAP 的调节 | Reconciliation | **需要** |
| 解释管理层认为该指标对投资者有用的原因 | Explanation of Usefulness | **需要** |
| 不得以误导性方式呈现 Non-GAAP 指标 | Not Misleading | **需要遵守** |
| 对非经常性等标签存在限制 | Nonrecurring / Infrequent / Unusual | 不得误导性标记 |

在 SEC 申报文件中，Non-GAAP 披露受到 Regulation S-K Item 10(e) 等规则约束；其他公开披露还可能涉及 Regulation G。具体适用要求取决于披露场景。

### 为什么要解释“有用性”（Usefulness）？

公司不能只披露调整后利润数字而不说明目的。管理层应解释该指标为何提供了对投资者有用的财务状况或经营业绩信息，以及适用的其他使用信息。

### 对“非经常性”的限制

企业不能把事实上具有重复发生特征的项目随意称为 **Nonrecurring（非经常性）**、**Infrequent（不频繁）** 或 **Unusual（异常）**。

例如，按适用 SEC 规则，在相关 Non-GAAP 申报披露中，将某项费用 / 损失描述成非经常性时，需要考虑过去两年是否发生过类似项目，以及未来两年内是否合理可能再次发生。

注意：**不能误导性地标记为 Nonrecurring，不代表该项目在所有情况下都一律不得进行任何 Non-GAAP 调整。** 还需符合其他相关要求。

## 四、Reconciliation 调节表：如何计算？

假设公司披露（单位：百万美元）：

| 项目 | 金额 |
|---|---:|
| GAAP Net Income（净利润） | 100 |
| 加回某项重组费用（Restructuring Expense） | +20 |
| 减去相关所得税影响（Tax Effect） | −5 |
| **Adjusted Net Income（调整后净利润）** | **115** |

简化关系：

$$
\begin{aligned}
\text{Adjusted Net Income}
={}&\text{GAAP Net Income}\\
&+\text{Permitted Adjustments}\\
&-\text{Related Tax Effects}
\end{aligned}
$$

本例：

$$
100+20-5=115
$$

这只是演示调节过程，**不是表示所有重组费用都允许作为合法、合理的 Non-GAAP 调整**。企业仍需说明调整的性质、合理性并遵守 SEC 规定。

## 五、财务分析师为什么要关注 Non-GAAP？

1. 比较 GAAP 与 Non-GAAP 利润差距是否持续扩大。
2. 检查剔除的费用是否真的偶发，还是每年反复发生。
3. 核对调整项目对税费的影响及计算口径。
4. 判断不同公司、不同年度的 Adjusted EPS 等是否可比。
5. 不能仅因调整后利润更高就认定经营改善，应同时阅读 GAAP 报表及附注。

## 六、本次 CFA 题目：判断 SEC 披露要求

题目问：在美国，公司在 SEC 申报文件中报告 Non-GAAP 指标时，哪项表述正确？

- **A 正确**：应提供 Non-GAAP 指标与最直接可比 GAAP 指标的调节（Reconciliation）。
- **B 错误**：公司并非无需解释指标有用性；通常需要说明为何认为其对投资者有用。
- **C 错误**：不能随意将合理预期会重复发生的项目标记为 Nonrecurring，并据此进行误导性披露。

**正确答案：A。**

## 七、考试速记与易错点

- **Non-GAAP → Comparable GAAP + Reconciliation + Usefulness Explanation。**
- Reconciliation 不等于简单展示两个结果，必须说明中间调整项目。
- SEC 监管的是信息的透明度和不误导性，而非禁止所有 Non-GAAP 指标。
- Nonrecurring 是一种需要依据的性质判断，不是管理层想怎么命名就怎么命名。
- Adjusted Earnings 越高，不一定代表财务表现越好；应检查剔除项目是否经常发生。

## 八、自测

- [ ] 能区分 GAAP 与 Non-GAAP 指标
- [ ] 能解释 Reconciliation 的作用
- [ ] 能说出 SEC 申报披露的三个重点：Comparable GAAP、Reconciliation、Usefulness
- [ ] 能识别误导性 Nonrecurring 标签
- [ ] 能读懂简单的 GAAP-to-Non-GAAP 调节表
