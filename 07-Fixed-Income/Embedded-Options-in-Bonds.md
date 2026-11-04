---
subject: CFA Level I
topic: Embedded Options in Bonds
status: 已整理
tags: [CFA-L1, Fixed-Income, Bonds, Embedded-Options]
---

# Embedded Options in Bonds｜嵌入式期权债券

## 1. 核心概念

**Embedded Option（嵌入式期权）**：附加在债券合同中的期权条款，会改变债券对发行人或投资者的价值。

比较时，假设债券的发行人信用风险、期限、票面利率等其他条件相同。

## 2. 三种债券对比

| 债券类型 | 中文 | 期权权利归属 | 相对普通债券的价值 | 相对普通债券的价格 | 相对普通债券的收益率 |
|---|---|---|---|---|---|
| Option-Free Bond | 无期权债券 | 无嵌入式期权 | 基准 | 基准 | 基准 |
| Callable Bond | 可赎回债券 | 发行人（Issuer） | 普通债券价值 − 看涨期权价值 | 更低 | 更高 |
| Putable Bond | 可回售债券 | 投资者（Investor） | 普通债券价值 + 看跌期权价值 | 更高 | 更低 |

### Callable Bond｜可赎回债券

- 发行人拥有在约定日期或条件下提前赎回债券的权利。
- 该权利对发行人有利、对投资者不利。
- 投资者承担债券被提前赎回的风险，因此通常要求更高收益率（Higher Yield）。
- 价值关系：\(V_{Callable}=V_{Option-Free}-V_{Call}\)。

### Putable Bond｜可回售债券

- 投资者拥有在约定日期或条件下，按约定价格将债券卖回给发行人的权利。
- 该权利为投资者提供保护，因此增加债券对投资者的价值。
- 投资者愿意为这项保护支付价格，表现为债券价格更高、要求收益率更低（Lower Yield）。
- 价值关系：\(V_{Putable}=V_{Option-Free}+V_{Put}\)。

## 3. 价格与收益率关系

债券价格（Bond Price）与收益率（Yield）反向变动：

\[
Price\uparrow \Rightarrow Yield\downarrow
\]

\[
Price\downarrow \Rightarrow Yield\uparrow
\]

因此，在其他条件相同的情况下：

- Callable Bond：价格低于普通债券，收益率高于普通债券。
- Putable Bond：价格高于普通债券，收益率低于普通债券。

## 4. 考试记忆

- **Callable：Issuer has the right to call**——发行人有权赎回，对投资者不利，要求更高收益率。
- **Putable：Investor has the right to put**——投资者有权回售，对投资者有利，接受更低收益率。
- **Option-Free：No embedded option**——无嵌入式期权，作为比较基准。

记忆口诀：**发行人拿到期权，投资者要补偿；投资者拿到期权，投资者愿意让利。**

## 5. 本题考点

题干：Compared with an equivalent option-free bond, a putable bond always has a(n) ______.

正确答案：**B. Lower yield（较低收益率）**。

原因：可回售权（Put Option）属于投资者，增加债券价值；在其他条件相同的情况下，债券价格更高，因此收益率更低。

注意：这里的比较建立在债券其他关键特征相同的前提下，不能脱离可比条件，单独比较不同债券的实际收益率。
