---
subject: Financial Statement Analysis
topic: Deferred Income Taxes
status: "🟡 解析能懂，待独立验证"
created: 2026-11-04
last-reviewed:
tags: [CFA-L1, FSA, Deferred-Taxes, DTA, DTL]
---

# 递延所得税（Deferred Income Taxes）

## 一、首先理解：会计与税法确认时间可能不同

- **Accounting Profit / Pretax Accounting Income（会计税前利润）**：按照会计准则确认的收入减费用。
- **Taxable Income（应纳税所得额）**：按照税法计算的所得，决定当期应交所得税。
- **Income Tax Expense（所得税费用）**：财务报表中报告的当期所得税费用及递延所得税影响之和。
- **Taxes Payable（应交所得税）**：根据当期应纳税所得额和税法计算的当期税额。

会计利润不一定等于应纳税所得额。核心原因之一是**确认时间不同**。

## 二、DTA 与 DTL 的本质区别

| 项目 | DTA | DTL |
|---|---|---|
| 英文全称 | Deferred Tax Asset | Deferred Tax Liability |
| 中文 | 递延所得税资产 | 递延所得税负债 |
| 未来影响 | 未来可抵减所得税 | 未来需要缴纳更多所得税 |
| 典型费用时间差异 | 会计先确认费用，税法以后扣除 | 税法先允许扣除，会计以后确认费用 |
| 常见实例 | 计提但未支付的保修费用、符合条件的坏账准备 | 税法加速折旧快于会计折旧 |

**记忆：**
- **DTA：现在不能扣、以后可扣 → 未来少交税。**
- **DTL：现在先扣、以后少扣 → 未来多交税。**

这些只是典型费用情形。判断完整资产 / 负债项目时，应结合账面价值与计税基础。

## 三、暂时性差异与永久性差异

### 1. Temporary Difference（暂时性差异）

资产或负债的账面价值（Carrying Amount）与计税基础（Tax Base）存在差异，并将在未来通过资产收回或负债清偿产生所得税影响。

- **Deductible Temporary Difference（可抵扣暂时性差异）**：未来会产生税前扣除，通常形成 DTA（还需满足确认条件）。
- **Taxable Temporary Difference（应纳税暂时性差异）**：未来会增加应纳税金额，通常形成 DTL（存在特定确认例外）。

### 2. Permanent Difference（永久性差异）

某些收入或费用在会计与税法中的处理永久不同，未来不会转回，因此通常不产生 DTA 或 DTL。

例：税法永久不允许扣除的某些罚款（取决于当地税法）。

### 3. 快速判断表

| 情形 | 是否未来转回 | 主要结果 |
|---|---|---|
| 保修费用会计当期计提，未来实际支付时税前扣除 | 是 | Deductible Temporary Difference → DTA |
| 税法折旧比会计折旧快，未来差额转回 | 是 | Taxable Temporary Difference → DTL |
| 税法永久不允许税前扣除的罚款 | 否 | Permanent Difference，不产生递延所得税 |

## 四、计税基础（Tax Base）怎么理解？

### 1. 资产的计税基础
通常指未来收回资产账面价值时，按税法允许抵扣的金额。

典型例子：某设备账面价值为 800，计税基础为 600。
- 未来按账面价值收回资产时，税法可扣除的成本较少。
- 应纳税暂时性差异 = 800 − 600 = 200。
- 在简化假设下形成 DTL。

### 2. 负债的计税基础
一般可理解为：

$$
\text{Tax Base of Liability}
=
\text{Carrying Amount}
-
\text{Future Tax Deduction}
$$

例如预提保修负债账面金额为 1,000，未来支付时可扣除 1,000：

$$
\text{Tax Base}=1,000-1,000=0
$$

因此：

$$
\text{Deductible Temporary Difference}=1,000-0=1,000
$$

这对应的是 DTA，而不是 DTL。

## 五、递延所得税的常用计算公式

对于简单的单项暂时性差异：

$$
\text{DTA}
=
\text{Deductible Temporary Difference}
\times
\text{Applicable Tax Rate}
$$

$$
\text{DTL}
=
\text{Taxable Temporary Difference}
\times
\text{Applicable Tax Rate}
$$

税率应采用预计暂时性差异转回时适用、且符合相关准则规定的税率。题目没有给出税率时，只能判断 DTA 或 DTL 的类型，不能计算金额。

在不考虑递延所得税其他特殊项目的简化情形下：

$$
\text{Income Tax Expense}
=
\text{Current Tax Expense}
+
\text{Deferred Tax Expense}
$$

递延所得税费用可能为负数（递延所得税收益）；若相关交易计入 OCI 或权益，其所得税影响也可能相应在 OCI 或权益列报，不能一概计入利润表。

## 六、本题案例：保修费用（Warranty Expense）

Gordon Co. 在 2019 年会计报表中计提产品保修费用 $1,000；税法规定，只有实际支付保修款项时，才允许税前扣除。

### 第一步：会计如何确认？
- Warranty Expense（保修费用）当期增加 $1,000。
- Warranty Liability（保修负债）增加 $1,000。
- 即使当期没有支付现金，权责发生制下仍需确认费用和负债。

### 第二步：税法如何处理？
- 2019 年尚未支付，不能扣除这 $1,000。
- 未来实际支付时，才允许税前扣除。

### 第三步：判断差异
- 费用的会计确认早于税法扣除。
- 将来会获得税前扣除，是**可抵扣暂时性差异（Deductible Temporary Difference）**。
- 因此形成 **Deferred Tax Asset（DTA）**，不是 DTL，也不是永久性差异。

### 第四步：如果税率为 30%（仅作演示）

$$
\text{DTA}=1,000\times30\%=300
$$

注：原题没有提供税率，因此本题只要求判断类型，不要求计算 $300；30% 是辅助理解的假设。

### 第五步：未来实际支付时
- 会计上冲减 Warranty Liability，不重复确认同一笔保修费用；
- 税法允许税前扣除；
- 暂时性差异转回，相关 DTA 随之转回。

**本题正确答案：A. a deferred tax asset.**

## 七、IFRS 与 US GAAP 的确认差异（简要）

| 比较 | IFRS（IAS 12） | US GAAP（ASC 740） |
|---|---|---|
| DTA 可回收性 | 在未来很可能有足够应纳税利润可利用时确认 DTA | 通常先确认 DTA，再评估 Valuation Allowance（估值备抵） |
| DTA 不能充分利用时 | 仅确认预计可回收部分，或减少已确认金额 | 在部分税收利益更可能无法实现时确认估值备抵 |
| 核心考点 | Probable Future Taxable Profit | Valuation Allowance / More-likely-than-not |

此处仅作 CFA 一级识别层面的简要对比；具体税收亏损结转、初始确认豁免等情形另有要求。

## 八、考试易错点

1. **DTA 不是“会计费用越大就一定产生”**；核心是未来是否存在可利用的税收扣除或其他可抵扣差异。
2. **DTL 不是当期应交税款**；它表示未来相关暂时性差异转回带来的税务负担。
3. **Temporary vs Permanent**：暂时性差异未来会转回；永久性差异不会。
4. **Warranty Expense**：会计先计提、税法以后扣 → DTA。
5. **Accelerated Tax Depreciation**：税法折旧先多扣、以后少扣 → 通常 DTL。
6. **不能将未提供的税率当作题目数据**；先判断性质，再算金额。
7. **Tax Base 不是账面价值**，二者差异才是递延所得税分析的核心。

## 九、复习检查

- [ ] 能解释 DTA 与 DTL 的未来税收影响
- [ ] 能区分 Temporary Difference 和 Permanent Difference
- [ ] 能解释 Tax Base 与 Carrying Amount 的关系
- [ ] 能推导保修费用计提为什么形成 DTA
- [ ] 能根据税率计算简单的 DTA / DTL
- [ ] 能识别 IFRS 的可回收性条件与 US GAAP 的 Valuation Allowance
