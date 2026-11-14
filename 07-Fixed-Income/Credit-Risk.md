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
