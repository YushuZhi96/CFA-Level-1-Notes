---
subject: Fixed Income
topic: Macaulay Duration
status: 持续复习
created: 2026-11-01
last-reviewed: 2026-11-14
tags: [CFA-L1, Fixed-Income, Duration, Calculation, Immunization]
---

# Macaulay Duration｜麦考利久期专项：原理、计算与考试速判

> 属于 [[Duration-Study-Guide|Duration 久期总专题]]。本文件专门讲 Macaulay Duration 的现金流现值、现值权重、完整计算、金融计算器和 Immunization 应用。

## 一、概念与直觉

**Macaulay Duration（麦考利久期）**：债券所有未来现金流的现值加权平均收款时间（Present-Value-Weighted Average Time），通常以年为单位。

- Maturity（到期期限）：最后一次现金流距离今天有多久。
- Macaulay Duration：把各笔票息和本金按现值权重加权之后，平均多久收到现金流。
- 对普通正现金流固定票息债券，久期通常小于到期期限；零息债券的麦考利久期等于到期期限。

## 二、核心公式：现金流 → 现值 → 权重 → 久期

**1. 第 t 期现金流现值（Present Value）**

\[
\boxed{PV(CF_t)=\frac{CF_t}{(1+r)^t}}
\]

其中 r 是与计息周期匹配的每期折现率，t 是距离收到现金流的期数。每往回折现一年（年度付息情况下），就除以一次 1+r。

**2. 债券价格（Bond Price）**

\[
\boxed{P=\sum_{t=1}^{N}PV(CF_t)}
\]

**3. 现值权重（Present Value Weight）**

\[
\boxed{w_t=\frac{PV(CF_t)}{P}}
\]

全部现金流的现值权重相加为1（100%）。注意不是用未折现的现金流计算权重。

**4. Macaulay Duration**

\[
\boxed{D_{Mac,\ periods}=\sum_{t=1}^{N}t\,w_t}
\]

如果 t 是付息期数，每年有 m 期，则：

\[
\boxed{D_{Mac,\ years}=\frac{\sum_{t=1}^{N}t\,w_t}{m}}
\]

如果时间 t 已经以年为单位，就直接按年加权，不必再除以 m。

## 三、完整例题：2年期、票面5%、YTM6%

题目：A 2-year 5% annual-pay corporate bond has a yield of 6%.

假设面值（Face Value）100，票面利率（Coupon Rate）5%，每年付息一次，YTM 6%。每年票息为 100×5%=5。

### 第一步：列现金流

| 时间 | 票息 | 本金 | 现金流 CF |
|---|---:|---:|---:|
| 第1年末 | 5 | 0 | **5** |
| 第2年末 | 5 | 100 | **105** |

第二年收到105，是因为最后一次票息5与到期本金100同时支付。

### 第二步：计算每期现金流现值

第一年：仅折现一次。

\[
PV_1=\frac5{1.06}=\boxed{4.7170}
\]

第二年：需要折现两次。

\[
PV_2=\frac{105}{(1.06)^2}=\boxed{93.4496}
\]

**为什么平方？** 第2年末的现金流需要连续向前折现两年，即 105÷1.06÷1.06。

### 第三步：计算当前债券价格

\[
P=4.7170+93.4496=\boxed{98.1666}
\]

票面利率5%低于YTM6%，所以这是折价债券（Discount Bond），价格低于100，结果方向合理。

### 第四步：计算现金流现值权重

| 时间 | CF | PV | PV Weight |
|---|---:|---:|---:|
| 第1年 | 5 | 4.7170 | 4.7170/98.1666 ≈ **4.81%** |
| 第2年 | 105 | 93.4496 | 93.4496/98.1666 ≈ **95.19%** |
| 合计 | 110 | 98.1666 | **100%** |

### 第五步：时间乘权重再加总

\[
D_{Mac}=1\times\frac{4.7170}{98.1666}+2\times\frac{93.4496}{98.1666}
\]

\[
\boxed{D_{Mac}\approx1.9519\text{ years}\approx1.95\text{ years}}
\]

直觉：95%以上的债券价值来自第2年末，所以平均收款时间非常接近2年；但第1年末已经收到少量票息，因此久期稍短于2年。

## 四、BA II Plus 金融计算器怎样帮忙？

采用 P/Y=1、C/Y=1、END 模式，这道年度付息债券输入：

| 按键 | 数值 |
|---|---:|
| N | 2 |
| I/Y | 6 |
| PMT | 5 |
| FV | 100 |
| CPT → PV | −98.1666 |

**注意：TVM 的 CPT → PV 算出来的是债券价格，不是 Macaulay Duration。**

算出债券价格之后，还要用两笔现金流的现值计算权重，并做时间加权。PV 为负仅反映现金流输入方向，计算现值权重时用价格绝对值。

## 五、为什么这道题要选持有1.95年？

**Duration Matching（久期匹配）/ Immunization（免疫策略）**：

对于标准固定票息债券，在利率小幅变动、适当的再投资和其他简化假设下，持有期限（Investment Horizon）等于 Macaulay Duration 时，价格风险（Price Risk）与票息再投资风险（Coupon Reinvestment Risk）的**一阶影响近似抵消**。

\[
\boxed{Investment\ Horizon\approx D_{Mac}}
\]

| 持有期限和久期关系 | 哪种利率风险通常占主导 |
|---|---|
| Horizon < Macaulay Duration | Market Price Risk（价格风险） |
| Horizon = Macaulay Duration | 两种效应一阶近似抵消 |
| Horizon > Macaulay Duration | Reinvestment Risk（再投资风险） |

- 利率上升：债券价格通常下降，再投资收益可能提高。
- 利率下降：债券价格通常上涨，再投资收益可能降低。
- 注意：不是任何大小的利率变化都能完全抵消；还受凸性、现金流变化、曲线非平行变动等影响。

**本题选项辨析**：

- A：持有1.98年，两种风险抵消 → 错，因为久期约1.95年。
- B：持有1.98年，价格风险主导 → 错，1.98年高于久期，再投资风险更可能主导。
- C：持有1.95年，两种风险抵消 → **正确**。

## 六、半年付息时的处理

若债券每半年付息一次、YTM按半年复利的名义年化口径给出：

- N = 年数×2。
- PMT = 面值×年度票面利率÷2。
- 每期折现率 r = 年化YTM÷2。
- 按期数 t 计算现值和权重；得到加权平均的“半年期数”后，再除以2变成年数。

例如加权结果为3.8个半年期，久期为 3.8÷2=1.9年。

## 七、CFA 考试易错点与速判

1. **Weighted Average Time / PV Weights** → Macaulay Duration。
2. 不是直接用未折现现金流占比作权重，而是用 Present Value 权重。
3. 到期最后一期现金流 = Coupon + Face Value。
4. 久期与到期期限不总相等；正票息固定债通常久期更短。
5. YTM 与付息周期要匹配；每半年付息时注意期数单位和年单位换算。
6. 估计小幅YTM变化的**百分比价格影响**应优先考虑 Modified Duration；现金流随利率改变时考虑 Effective Duration。
7. Horizon = Macaulay Duration → 标准免疫框架下一阶价格风险与再投资风险近似抵消。
8. 1.95与1.98这样接近的选项，应使用足够精度的现值权重，最后才四舍五入。

## 八、5道自测

1. 第1年现金流5、YTM6%，PV是多少？答：5/1.06≈4.7170。
2. 第二年现金流为什么是105？答：票息5＋本金100。
3. 价格P是多少？答：约98.1666。
4. Macaulay Duration是多少？答：约1.9519年。
5. Horizon为1.98年时哪种风险更可能主导？答：Reinvestment Risk。

## 关联

[[Duration-Study-Guide|Duration 总专题]] · [[Modified-Duration]] · [[Key-Rate-Duration]] · [[Fixed-Income-Basics]]


## YTM 如何影响 Macaulay Duration？

对于其他条件相同的普通固定票息债券（相同票息率、到期期限、付息频率及可比风险）：

- YTM 上升，未来现金流折现更重，尤其是较远期现金流的现值下降得更多。
- 远期现金流占债券总价格的现值权重通常下降，较早现金流的相对权重提高。
- 因此，Macaulay Duration（现值加权平均收款时间）通常缩短。

\[
\boxed{YTM\uparrow\Rightarrow D_{Mac}\downarrow}
\]

**特殊情况：Zero-Coupon Bond（零息债券）**只有到期时的一笔现金流，因此其 Macaulay Duration 始终等于到期期限，不会因为 YTM 改变而缩短。

注意：这里讨论的是固定现金流、无嵌入式期权债券的标准比较。含 Callable / Putable 等期权时，利率变化可能改变预期现金流，应结合 Effective Duration 分析。
