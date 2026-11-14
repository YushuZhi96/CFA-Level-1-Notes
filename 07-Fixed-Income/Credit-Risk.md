---
subject: Fixed Income
topic: Credit Risk
status: 持续复习
tags: [CFA-L1, Fixed-Income, Credit-Risk, Credit-Rating, Seniority, Recovery-Rate]
---

# Credit Risk｜信用风险专题

> 本专题整理发行人信用评级、债务工具评级、债务偿付优先级和违约回收率。与 [[Fixed-Income-Basics|Fixed Income Basics]] 及 [[CDS-Credit-Spread|CDS & Credit Spread]] 关联。

## 1. Issuer Rating vs. Issue Rating｜发行人评级与债务工具评级

### Issuer Rating｜发行人信用评级

衡量发行人整体的信用状况与履行金融义务的能力，重点是发行人整体违约风险（Default Risk）。

### Issue Rating｜债务工具评级

针对某一具体债务工具或债券发行的评级。除发行人整体信用状况外，还会考虑该债务的担保、偿付优先级、结构性次级、担保人及其他信用增级安排。

### CFA 核心基准关系

在 CFA Level I 的典型框架中，发行人的信用评级通常以其 **Senior Unsecured Debt（优先无担保债务）** 的评级作为基准：

\[
\boxed{Issuer\ Rating\approx Senior\ Unsecured\ Debt\ Rating}
\]

原因：优先无担保债务没有特定抵押物提供额外保护，同时其偿付优先级高于次级债务，通常被用作衡量发行人一般信用风险的基准。

**注意**：这是一项典型考试规则，不代表所有评级机构、所有发行人和所有债券的评级必然相同。实际 Issue Rating 可能因抵押、担保、结构性次级或其他条款而相对发行人评级上调或下调（Notching）。

## 2. Three Debt Seniority Types｜三种债务类型

### Senior Secured Debt｜优先有担保债务

- **Senior**：在相关债务偿付顺序中具有较高优先级。
- **Secured**：有特定资产或担保权益提供信用保护。
- 违约时，债权人可依据担保文件及适用法律对抵押品主张权利。
- 因抵押品和优先受偿保护，回收率（Recovery Rate）通常较高；其 Issue Rating 可能高于 Issuer Rating。

### Senior Unsecured Debt｜优先无担保债务

- **Senior**：偿付优先级通常高于次级债务。
- **Unsecured**：没有特定抵押资产作为担保。
- 在 CFA 的典型框架中，其评级通常作为 Issuer Rating 的基准。

### Subordinated Debt｜次级债务

- 偿付顺序低于相关优先债务（Senior Debt）。
- 发行人违约或清算时，通常要在优先债务受偿后才能获得偿付。
- 在其他条件相同的情况下，预期回收率通常较低，信用风险较高，其 Issue Rating 可能低于 Issuer Rating。

## 3. Simplified Seniority Ranking｜简化偿付优先级

在仅比较本题涉及的三类公司债务、且不存在特殊法定优先权或其他复杂结构时，可记为：

1. **Senior Secured Debt**：有担保的优先债务，通常有抵押品保护。
2. **Senior Unsecured Debt**：优先无担保债务。
3. **Subordinated Debt**：次级债务，偿付顺序靠后。

实际破产清偿顺序必须结合担保权益、债务合同、法定优先权、司法辖区及具体资本结构判断；不能把上述简化顺序机械套用于所有情形。

## 4. Recovery Rate｜回收率

**Recovery Rate（回收率）**：发生违约后，债权人最终收回的金额占违约债权金额的比例。

\[
\boxed{Recovery\ Rate=\frac{Amount\ Recovered}{Exposure\ at\ Default}}
\]

简化示例（仅用于说明）：

| 债务类型 | 假设回收金额 | 假设回收率 |
|---|---:|---:|
| Senior Secured | 80 | 80% |
| Senior Unsecured | 50 | 50% |
| Subordinated | 20 | 20% |

以上数字不是固定行业规律。实际回收率受抵押品价值、清偿成本、破产程序、资本结构和经济环境影响。

## 5. 本题归档：Issuer Rating 对应哪类债务？

**题目**：The credit rating of an issuing company is the same as that of its:

- A. Senior secured obligation
- B. Subordinated debt
- C. Senior unsecured debt

**正确答案：C. Senior unsecured debt（优先无担保债务）。**

解题逻辑：

- Senior secured obligation 有抵押资产提供额外保护，具体债券评级可能高于发行人基准评级。
- Subordinated debt 的偿付顺序靠后，具体债券评级可能低于发行人基准评级。
- Senior unsecured debt 在典型 CFA 框架中作为发行人一般信用风险的评级基准。

## 6. CFA Exam Quick Review｜考前速记

| 题目关键词 | 优先联想 |
|---|---|
| Issuer Rating | 发行人整体信用风险 |
| Senior Unsecured | 发行人评级的典型基准 |
| Senior Secured | 抵押品保护、回收率通常较高 |
| Subordinated | 偿付顺序靠后、回收率通常较低 |
| Issue Rating | 具体债务工具评级 |
| Recovery Rate | 违约后实际收回金额占违约敞口的比例 |

**记忆口诀**：

- Senior Secured：优先 + 有抵押。
- Senior Unsecured：优先 + 无抵押，是典型 Issuer Rating 基准。
- Subordinated：次级，排在优先债务之后。

## 关联笔记

- [[Fixed-Income-Basics|Fixed Income Basics]]
- [[CDS-Credit-Spread|CDS & Credit Spread]]


## 7. Notching Adjustment｜信用评级微调

**Notching（评级微调）**：评级机构以发行人信用评级（Issuer Rating）为参考，根据某一具体债务工具的偿付优先级、担保、结构性次级和预期回收情况，对该债务工具评级向上或向下调整。

- **Upward Notching（向上微调）**：例如债务有高质量抵押品或强担保，预期回收率相对更高，具体债务评级可能高于发行人评级。
- **Downward Notching（向下微调）**：例如次级债务（Subordinated Debt）在清偿顺序中靠后，预期回收率可能更低，具体债务评级可能低于发行人评级。

### High-Yield vs. Investment-Grade｜高收益债与投资级债的微调幅度

CFA 考试的典型结论：

\[
\boxed{Notching_{High\text{-}Yield}>Notching_{Investment\text{-}Grade}}
\]

高收益债（High-Yield / Speculative-Grade Debt）的信用质量较弱、违约风险通常较高。发生违约时，抵押品和债务偿付优先级造成的回收率差异，对债权人的预期损失及具体债务风险更为重要。因此，评级机构通常会对高收益债进行幅度更大的评级微调。

投资级债（Investment-Grade Debt）违约风险相对较低，债务层级之间回收率差异对评级的影响通常较小，因此微调幅度通常较小。

**CFA 题型复盘：**

题目：For a high-yield debt, the extent of notching adjustment is most likely:

- A. bigger than investment-grade.
- B. smaller than investment-grade.
- C. same as investment-grade.

**正确答案：A. bigger than investment-grade.**

**速记**：High-Yield → recovery / seniority differences matter more → larger notching.

**注意**：这是典型评级方法和考试比较关系，不表示每一只高收益债的实际 notch 数都必然大于每一只投资级债；具体调整仍由评级机构的评级方法、资本结构、抵押品和担保情况决定。

## 8. Expected Loss｜预期损失、PD、LGD 与 Recovery Rate

### 四个核心概念

- **PD (Probability of Default)**：违约概率，某一期间内发生违约的概率。
- **LGD (Loss Given Default)**：违约损失率，发生违约后无法收回的敞口比例。
- **RR (Recovery Rate)**：回收率，发生违约后可收回的敞口比例。
- **EL (Expected Loss)**：预期损失，按违约概率加权后的平均损失。

回收率与违约损失率互补：

\[
\boxed{LGD=1-RR}
\]

若以违约敞口比例表示预期损失率：

\[
\boxed{EL\ Rate=PD\times LGD=PD\times(1-RR)}
\]

若计算金额：

\[
\boxed{Expected\ Loss=PD\times LGD\times EAD}
\]

其中 **EAD (Exposure at Default)** 是违约风险暴露金额。若涉及损失发生时间和现值，还需要按题目要求折现；本节基础题暂不考虑折现。

### 例题：由 PD 和 EL 求 Recovery Rate

**题目**：一家跨国公司的 Default Probability 为10%，Expected Loss 为4%。发生违约时的 Recovery Rate 是多少？

已知：

\[
PD=10\%,\quad EL\ Rate=4\%
\]

代入：

\[
4\%=10\%\times(1-RR)
\]

\[
1-RR=\frac{4\%}{10\%}=40\%
\]

\[
\boxed{RR=60\%}
\]

**正确答案：B. 60%。**

### 用金额直觉理解

假设 EAD = 100：

- 违约概率为10%，对应预期违约敞口为10。
- 预期损失为4。
- 违约时损失率为 \(4/10=40\%\)。
- 回收率为 \(1-40\%=60\%\)，即违约时预计收回6。

### 公式变形：考试常用

\[
\boxed{EL=PD\times LGD}
\]

\[
\boxed{LGD=\frac{EL}{PD}}
\]

\[
\boxed{RR=1-\frac{EL}{PD}}
\]

以上 EL 与 PD 均使用相同期间、相同敞口口径的比例数值。

**易错点**：
1. Recovery Rate 不是 \(EL/PD\)，而是 \(1-EL/PD\)。
2. \(EL/PD\) 得到的是 LGD（违约损失率）。
3. 若题目给的是预期损失金额而非损失率，需要先除以 EAD，或直接使用 \(EL=PD\times LGD\times EAD\)。
4. PD、LGD、RR、EL 的期间和敞口口径必须一致。

### CFA 考题复盘

**题型1：High-Yield Debt 的 Notching Adjustment 与 Investment-Grade 相比如何？**

正确：通常更大（Bigger），因为在高收益债中，偿付优先级和回收率差异对信用风险及评级更重要。

**题型2：PD=10%，EL Rate=4%，求 Recovery Rate。**

正确：

\[
RR=1-\frac{4\%}{10\%}=60\%
\]

