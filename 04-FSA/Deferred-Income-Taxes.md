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

## 八、法定税率与有效税率（Statutory vs Effective Tax Rate）

### 1. 两种税率

- **Statutory Tax Rate（法定税率）**：税法规定的企业所得税税率。
- **Effective Tax Rate, ETR（有效税率）**：利润表中的所得税费用占税前会计利润的比率。

$
\text{Effective Tax Rate}=
\frac{\text{Income Tax Expense}}{\text{Pretax Accounting Income}}
$

特别注意：分子是 **Income Tax Expense（所得税费用）**，包括适用的当期与递延所得税影响；不是仅使用现金实缴所得税或当期应交所得税。

### 2. 哪些因素可能使 ETR 与法定税率不同？

| 影响因素 | 对 ETR 的典型影响 | 原因 |
|---|---|---|
| Permanent Differences（永久性差异） | 通常会造成差异 | 某些收入永久免税或费用永久不可扣除 |
| Different Tax Jurisdictions（不同税收辖区） | 通常会造成差异 | 跨国公司及海外子公司适用不同税率 |
| Temporary Differences（暂时性差异） | **在税率不变且完整确认递延所得税等简化条件下，通常不单独改变 ETR** | 当期税额变化被递延所得税费用 / 收益抵销 |

**重要限定：** 暂时性差异并非任何情况下都不会影响 ETR。税率变动、DTA 可回收性及估值备抵变化、确认豁免、不同税收辖区等因素都可能使 ETR 发生变化。

### 3. 永久性差异示例

税前会计利润 $100，内含永久免税收入 $10，税率 25%，无其他调整：

$
\text{Taxable Income}=100-10=90
$

$
\text{Income Tax Expense}=90\times25\%=22.5
$

$
\text{ETR}=\frac{22.5}{100}=22.5\%
$

因此 ETR 22.5% 低于法定税率 25%。

### 4. 暂时性差异示例：与保修费用 DTA 相联系

假设：
- 扣除保修费用后的税前会计利润：$9,000；
- 保修费用：$1,000，会计已经计提，税法规定未来实际支付时才能扣除；
- 应纳税所得额：$10,000；
- 税率：30%，并假设未来税率不变、DTA 可以全额确认、没有其他差异。

当期所得税（Current Tax Expense）：

$
10,000\times30\%=3,000
$

确认递延所得税资产（DTA）：

$
1,000\times30\%=300
$

当期确认 DTA 带来递延所得税收益，因此利润表的所得税费用：

$
\text{Income Tax Expense}=3,000-300=2,700
$

有效税率：

$
\text{ETR}=\frac{2,700}{9,000}=30\%
$

**结论：** 当期应交税款可能高于以会计利润计算的金额，但在上述假设下，递延所得税调整后 ETR 仍等于法定税率。

### 5. 这类 CFA 题目怎么判断？

问“以下哪一项最不可能使法定税率与有效税率产生差异？”

- A：未来不转回的税会差异 → Permanent Differences，会影响 ETR。
- B：存在海外子公司的跨国公司 → 可能受 Foreign Tax Rates 影响 ETR。
- C：Temporary Differences → 在标准简化情境下通常只是当期与递延所得税之间的时间分配，不单独改变 ETR。

**正确答案：C。**

### 6. 速记

- **Permanent Difference → ETR 通常改变。**
- **Foreign Tax Rate Differences → ETR 可能改变。**
- **Temporary Difference → Current Tax 与 Deferred Tax 的时间差；通常不单独改变 ETR（有前提）。**

## 九、递延所得税资产估值备抵（Valuation Allowance）

### 1. 定义与用途

在 **US GAAP（ASC 740）** 下，Valuation Allowance（估值备抵，VA）是对递延所得税资产（Deferred Tax Asset，DTA）的抵减项目（Contra-asset）。当已有证据表明部分或全部 DTA 的税收利益**更有可能无法实现（More Likely Than Not）**时，确认估值备抵。

- **Gross DTA（递延所得税资产总额）**：尚未扣除估值备抵的 DTA。
- **Valuation Allowance（估值备抵）**：预计无法实现的 DTA 部分。
- **Net DTA（递延所得税资产净额）**：扣除估值备抵后可列报的 DTA 金额。

估值备抵是 DTA 的抵减项，**不是 Deferred Tax Liability（递延所得税负债）**，不会因为计提 VA 就产生一项额外的欠税义务。

### 2. 核心公式

**公式一：递延所得税资产净额**

$
\text{Net DTA}=\text{Gross DTA}-\text{Valuation Allowance}
$

**公式二：估值备抵变动**

$
\Delta\text{VA}=\text{Ending VA}-\text{Beginning VA}
$

**公式三：估值备抵对当期所得税费用的增量影响**

若 **Gross DTA 及其他条件不变，且 VA 的变动全部计入当期损益**：

$
\Delta\text{Income Tax Expense}=\Delta\text{VA}
$

**公式四：净利润**

$
\text{Net Income}=\text{Pretax Income}-\text{Income Tax Expense}
$

因此，在上述简化前提下：

$
\text{VA}\uparrow
\Rightarrow\text{Net DTA}\downarrow
\Rightarrow\text{Tax Expense}\uparrow
\Rightarrow\text{Net Income}\downarrow
$

注意：以上第三个公式只是**估值备抵变动带来的所得税费用增量**，不是计算全部所得税费用的通用公式；涉及 OCI、权益或收购等特殊事项时，计入位置可能不同。

### 3. 什么时候需要估值备抵？

公司需要综合考虑未来 DTA 税收利益实现的正面和负面证据，例如：

- Future Taxable Income（未来应纳税所得额）是否充足；
- 历史及预计亏损是否持续；
- 税务亏损结转能否在到期前使用；
- Tax-planning Strategies（税务筹划策略）是否可行；
- 是否有可用的应纳税暂时性差异转回支持 DTA 实现。

**More Likely Than Not** 对应超过 50% 的判断门槛；是否计提 VA 以及金额，应根据证据评估，不是随意估算。

### 4. 题目案例：Gordon Co.（金额单位：千美元）

| 项目 | 原报告金额 | 假设提高 VA 后 |
|---|---:|---:|
| Gross DTA | 18,000 | 18,000 |
| Valuation Allowance | (1,250) | (2,000) |
| **Net DTA** | **16,750** | **16,000** |
| VA 增加额 | — | 750 |

$
\text{Original Net DTA}=18,000-1,250=16,750
$

$
\text{New Net DTA}=18,000-2,000=16,000
$

$
\Delta\text{VA}=2,000-1,250=750
$

假设新增 VA 全部计入损益，且其他项目不变，则：
- Net DTA **减少 750**；
- Income Tax Expense **增加 750**；
- Net Income **减少 750**。

**正确选项：C — Income Tax Expense（所得税费用）**。

### 5. 简化会计分录（US GAAP）

假设增加 VA 750 且该变化全部计入当期损益：

| 科目 | 借方 Debit | 贷方 Credit |
|---|---:|---:|
| Income Tax Expense（所得税费用） | 750 | |
| Valuation Allowance（估值备抵） | | 750 |

贷记估值备抵意味着抵减资产的余额增大，Net DTA 下降。

### 6. IFRS 与 US GAAP 对比

| 对比 | US GAAP（ASC 740） | IFRS（IAS 12） |
|---|---|---|
| DTA 可实现性 | 评估未来税收利益可实现程度 | 仅在未来很可能有足够应纳税利润可利用时确认 DTA |
| 可收回性不足 | 以 **Valuation Allowance** 抵减 DTA | 限制或减少已确认的 DTA，不采用完全相同的单列 VA 机制 |
| 核心目的 | 避免高估税收资产 | 避免高估税收资产 |

### 7. CFA 考试易错点

1. VA ↑ 不代表 DTA ↑，而是 **Net DTA ↓**。
2. VA 属于 **Contra-asset（抵减资产）**，不是 DTL。
3. VA 增加通常使所得税费用上升、净利润下降，但要注意入账位置和其他条件。
4. 题目单位若为 **$ thousands（千美元）**，计算金额需保持单位一致。
5. 若题目说 **valuation allowance is higher**，通常考其抵减作用，而不是新增的未来应纳税义务。

## 十、考试易错点

1. **DTA 不是“会计费用越大就一定产生”**；核心是未来是否存在可利用的税收扣除或其他可抵扣差异。
2. **DTL 不是当期应交税款**；它表示未来相关暂时性差异转回带来的税务负担。
3. **Temporary vs Permanent**：暂时性差异未来会转回；永久性差异不会。
4. **Warranty Expense**：会计先计提、税法以后扣 → DTA。
5. **Accelerated Tax Depreciation**：税法折旧先多扣、以后少扣 → 通常 DTL。
6. **不能将未提供的税率当作题目数据**；先判断性质，再算金额。
7. **Tax Base 不是账面价值**，二者差异才是递延所得税分析的核心。

## 十一、复习检查

- [ ] 能解释 Valuation Allowance 的含义并计算 Net DTA
- [ ] 能解释 VA 增加对 Income Tax Expense 与 Net Income 的影响
- [ ] 能区分 US GAAP 的 VA 与 IFRS 的 DTA 可回收性处理
- [ ] 能区分 Statutory Tax Rate 与 Effective Tax Rate
- [ ] 能解释 Permanent Differences 和 Foreign Tax Rates 为什么改变 ETR
- [ ] 能说明 Temporary Differences 通常不单独改变 ETR 的前提
- [ ] 能解释 DTA 与 DTL 的未来税收影响
- [ ] 能区分 Temporary Difference 和 Permanent Difference
- [ ] 能解释 Tax Base 与 Carrying Amount 的关系
- [ ] 能推导保修费用计提为什么形成 DTA
- [ ] 能根据税率计算简单的 DTA / DTL
- [ ] 能识别 IFRS 的可回收性条件与 US GAAP 的 Valuation Allowance
