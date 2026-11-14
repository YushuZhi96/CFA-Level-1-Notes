---
subject: Fixed Income
topic: Bond Premium and Discount Amortization
status: "🟡 解析能懂，待独立验证"
created: 2026-11-03
last-reviewed:
tags: [CFA-L1, Fixed-Income, Bonds, Effective-Interest-Method, Amortization]
---

# 债券溢价与折价摊销（Bond Premium and Discount Amortization）

## 一、先理解三个发行价格

债券（Bond）发行价格与面值（Face Value）的关系：

| 发行方式 | 发行价格与面值 | Coupon Rate 与 YTM |
|---|---|---|
| 折价发行（Issued at Discount） | Issue Price < Face Value | Coupon Rate < YTM |
| 平价发行（Issued at Par） | Issue Price = Face Value | Coupon Rate = YTM |
| 溢价发行（Issued at Premium） | Issue Price > Face Value | Coupon Rate > YTM |

- **Face Value / Par Value（面值）**：债券到期时发行人需要偿还的本金。
- **Coupon Rate（票面利率）**：债券合同约定的利率，用于计算每期现金票息。
- **Yield to Maturity, YTM（到期收益率）**：根据当前债券价格和约定现金流反推的到期收益率；新发行债券的 YTM 通常反映市场对可比债券要求的收益率。

## 二、两个必须分清的金额

### 1. 票面利息支付（Coupon Payment）

每期实际支付给债券持有人的现金利息：

$$
\text{Coupon Payment}
=
\text{Face Value}\times\text{Coupon Rate}
$$

### 2. 利息费用（Interest Expense）

发行人按实际利率法（Effective Interest Method）确认的会计利息费用：

$$
\text{Interest Expense}
=
\text{Beginning Carrying Value}\times\text{Market Yield at Issuance}
$$

在债券发行时确定的有效利率 / 市场收益率通常在债券存续期内保持不变；但由于债券账面价值逐期变化，每期确认的利息费用也会变化。

**关键区别：**
- Coupon Payment：按面值 × 票面利率计算，代表实际支付的现金利息。
- Interest Expense：按期初债券账面价值 × 实际利率计算，代表当期确认的利息费用。

## 三、核心公式：债券账面价值的变化

$$
\begin{aligned}
\text{Ending Carrying Value}
={}&\text{Beginning Carrying Value}\\
&+\text{Interest Expense}\\
&-\text{Coupon Payment}
\end{aligned}
$$

也可以理解为：

**期末债券账面价值 = 期初账面价值 + 利息费用 − 现金票息。**

两者之间的差额就是当期摊销的折价或溢价。

## 四、折价发行（Discount Bond）

折价发行时：

$$
\text{Issue Price}<\text{Face Value}
$$

因此：

$$
\text{YTM}>\text{Coupon Rate}
$$

因为市场要求的收益率高于债券票面利率，债券必须以低于面值的价格发行，才能使投资者获得市场要求的收益率。

### 计算示例

假设：
- Face Value = $1,000
- Issue Price / Beginning Carrying Value = $950
- Coupon Rate = 5%
- YTM = 6%

**第一步：计算现金票息**

$$
\text{Coupon Payment}=1,000\times5\%=\$50
$$

**第二步：计算利息费用**

$$
\text{Interest Expense}=950\times6\%=\$57
$$

**第三步：计算期末账面价值**

$$
950+57-50=\$957
$$

由于 Interest Expense（$57）大于 Coupon Payment（$50），差额 $7 会增加债券负债的账面价值。

### 折价摊销的方向

- 利息费用 > 现金票息。
- 折价逐期摊销，债券负债账面价值逐渐增加。
- Carrying Value 从低于面值逐步上升。
- 到期时账面价值收敛至 Face Value（假设按期正常偿还且无其他调整）。
- 因为期初账面价值逐期增加、有效利率不变，所以每期 Interest Expense 通常逐期增加。

记忆：**Discount → Carrying Value 上升 → Interest Expense 上升。**

## 五、溢价发行（Premium Bond）

溢价发行时：

$$
\text{Issue Price}>\text{Face Value}
$$

因此：

$$
\text{Coupon Rate}>\text{YTM}
$$

债券票面利率高于市场要求收益率，投资者愿意支付高于面值的价格购买。

### 计算示例

假设：
- Face Value = $1,000
- Issue Price / Beginning Carrying Value = $1,050
- Coupon Rate = 8%
- YTM = 6%

**第一步：计算现金票息**

$$
\text{Coupon Payment}=1,000\times8\%=\$80
$$

**第二步：计算利息费用**

$$
\text{Interest Expense}=1,050\times6\%=\$63
$$

**第三步：计算期末账面价值**

$$
1,050+63-80=\$1,033
$$

由于 Interest Expense（$63）小于 Coupon Payment（$80），差额 $17 会减少债券负债的账面价值。

### 溢价摊销的方向

- 利息费用 < 现金票息。
- 溢价逐期摊销，债券负债账面价值逐渐减少。
- Carrying Value 从高于面值逐步下降。
- 到期时账面价值收敛至 Face Value（假设按期正常偿还且无其他调整）。
- 因为期初账面价值逐期下降、有效利率不变，所以每期 Interest Expense 通常逐期下降。

记忆：**Premium → Carrying Value 下降 → Interest Expense 下降。**

## 六、折价与溢价完整对照表

| 比较项目 | Discount（折价） | Premium（溢价） |
|---|---|---|
| 发行价格 | 低于面值 | 高于面值 |
| Coupon Rate 与 YTM | Coupon < YTM | Coupon > YTM |
| 利息费用与现金票息 | Interest Expense > Coupon Payment | Interest Expense < Coupon Payment |
| 摊销方向 | 增加负债账面价值 | 减少负债账面价值 |
| 账面价值变化 | 逐步上升至面值 | 逐步下降至面值 |
| 利息费用随时间 | 通常逐期上升 | 通常逐期下降 |
| 到期偿还本金 | Face Value | Face Value |

## 七、到期偿还与现金流量表（Bond Redemption at Maturity）

无论债券最初以折价、平价还是溢价发行，发行人到期偿还的本金通常都是 **Face Value（面值）**，不是最初发行价格。

例如：
- 折价发行收到 $950，到期偿还 $1,000。
- 溢价发行收到 $1,050，到期偿还 $1,000。

偿还债券本金属于筹资活动现金流出（Cash Flow from Financing Activities, CFF）。注意：这里说的是**本金偿还**；现金利息支付的现金流分类需要根据适用会计准则判断，不能把本金偿还与利息支付混为一谈。

## 八、会计分录的直观理解

### 1. 折价发行

发行时收到现金少于面值，折价作为债券负债账面金额的抵减项。后续每期：
- 借记 Interest Expense（利息费用）；
- 贷记 Cash（支付票息）；
- 两者差额贷记 Bond Discount / 增加债券账面价值。

### 2. 溢价发行

发行时收到现金高于面值，溢价增加债券初始账面金额。后续每期：
- 借记 Interest Expense（利息费用）；
- 贷记 Cash（支付票息）；
- 两者差额借记 Bond Premium / 减少债券账面价值。

具体科目呈现会因教材采用“债券折价 / 溢价单独账户”还是“债券净额账面价值”而不同；核心是期末 Carrying Value 的变化公式。

## 九、CFA 常见考试陷阱

1. **Coupon Rate 不等于 YTM**：票面利率决定现金票息，YTM 是债券价格所隐含的收益率。
2. **Discount：Interest Expense > Coupon Payment**，差额使债券账面价值增加。
3. **Premium：Interest Expense < Coupon Payment**，差额使债券账面价值减少。
4. **有效利率不变不代表利息费用不变**：Interest Expense = Beginning Carrying Value × YTM；账面价值变动会使利息费用随之变化。
5. **到期偿还的是 Face Value**，不是发行价格。
6. **CFF 的面值偿还指本金**；现金利息支付应另按准则分类。
7. 期末账面价值正常情况下逐渐收敛至面值，计算时若出现几分钱差异，可能是四舍五入造成。

## 十、本次题目记录

题目问哪项最不准确，正确答案 **B**。

- A 正确：到期偿还本金按 Face Value，属于筹资活动现金流出。
- B 错误：溢价债券账面价值逐期下降，YTM 固定，因此 Interest Expense 通常逐期下降，而不是增加。
- C 正确：折价债券摊销时 Interest Expense 大于 Coupon Payment，负债账面价值逐期增加。

- [ ] 能区分 Coupon Rate、Coupon Payment 和 YTM
- [ ] 能写出债券期末账面价值变化公式
- [ ] 能独立计算折价债券第一期利息费用与期末账面价值
- [ ] 能独立计算溢价债券第一期利息费用与期末账面价值
- [ ] 能判断折价 / 溢价摊销方向及利息费用变化趋势
- [ ] 能解释到期偿还本金为何按 Face Value 计入 CFF


## 十一、出售债券的资本利得与摊销后账面价值（Capital Gain and Carrying Value）

### 1. 为什么以 Carrying Value 为基准？

对于以**摊余成本／有效利率法（Amortized Cost / Effective Interest Method）**衡量持有期间收益的题目，原始折价或溢价会随着时间逐期摊销。出售时要区分：

- **Amortized Carrying Value（摊销后账面价值）**：原始购买成本加上累计折价摊销，或减去累计溢价摊销。
- **Selling Price（卖出价格）**：实际出售债券所获得的价格（比较时需采用一致的净价、应计利息口径）。
- **Capital Gain / Loss（资本利得／损失）**：出售价格与出售时的摊销后账面价值之间的差额。

\[
\boxed{Capital\ Gain\ (Loss)=Selling\ Price-Carrying\ Value}
\]

当结果大于零为 Capital Gain（资本利得），小于零为 Capital Loss（资本损失）。

### 2. Discount Bond｜折价债券

\[
\boxed{Carrying\ Value=Original\ Purchase\ Price+Cumulative\ Discount\ Amortization}
\]

**例题**：面值1,000，三年前以900购买；截至出售日累计摊销折价60。

- Original Purchase Price = 900。
- Cumulative Discount Amortization = 60。
- Carrying Value = 900 + 60 = **960**。
- 如果第三年卖出价格为980：

\[
Capital\ Gain=980-960=\boxed{20}
\]

**为什么不直接算 980 − 900 = 80？** 因为其中60的账面增值已经按有效利率法反映为持有期间的折价摊销收益；本题要衡量的是超出摊销后账面价值的卖出利得。请将这种分类与以原始购买价计算的整个持有期价格差额区分开。

### 3. Premium Bond｜溢价债券

\[
\boxed{Carrying\ Value=Original\ Purchase\ Price-Cumulative\ Premium\ Amortization}
\]

溢价债券按有效利率法摊销时，账面价值逐期下降，通常向面值靠拢。

### 4. 考试对比与速判

| 债券 | 累计摊销对 Carrying Value 的影响 | 资本利得的比较基准 |
|---|---|---|
| Discount Bond（折价） | 原始买价 + 累计折价摊销 | 出售时 Carrying Value |
| Premium Bond（溢价） | 原始买价 − 累计溢价摊销 | 出售时 Carrying Value |

**本题原文的判断**：

> An investor sold a fixed-rate coupon bond which he purchased at discount 3 years ago. To measure the capital gain, the investor should compare the selling price with ...

- **A 错误**：折价债券应加上（plus）累计折价摊销，而不是减去（minus）。
- **B 错误**：原始购买价格忽略了持有期间已确认的折价摊销。
- **C 正确**：出售价格与出售时的 **Carrying Value** 比较。

**CFA 记忆句**：折价摊销要加，溢价摊销要减；计算这类资本利得时，比较 **Selling Price − Carrying Value**。

**口径提醒**：这里遵循题目的摊销后账面价值与利得分类框架；实际会计确认和税务资本利得的计算还取决于债券分类、税务成本基础及适用规则。不能将本题的 Capital Gain 公式不加条件地用于所有账户和税务情形。
