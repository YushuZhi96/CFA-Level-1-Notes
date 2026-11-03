---
subject: Financial Statement Analysis
topic: Defined Benefit Pension Plans and Net Pension Position
status: "🟡 解析能懂，待独立验证"
created: 2026-11-03
last-reviewed:
tags: [CFA-L1, FSA, Long-Term-Liabilities, Pension, IAS-19]
---

# 设定受益养老金计划与净养老金头寸（Defined Benefit Pension Plan & Net Pension Position）

## 一、核心概念

**Defined Benefit Pension Plan（设定受益养老金计划）**：企业承诺员工退休后获得约定的养老金福利。企业承担养老金义务及相关精算风险、投资风险，实际需要承担的成本可能随计划资产表现、折现率、员工寿命等因素变化。

与之对比：

- **Defined Contribution Plan（设定提存计划）**：企业按约定向计划缴纳固定金额；缴费完成后，员工退休福利主要取决于缴费及投资表现，企业通常不再承担进一步的养老金支付义务（除非另有法定义务或推定义务）。

## 二、两个必须区分的金额

### 1. 养老金义务现值（Present Value of Defined Benefit Obligation, DBO）

企业根据员工已提供的服务，预计未来需要支付的养老金福利，按照适用折现率折算到报告日的现值。

直观理解：**未来承诺要支付的钱，折算成今天值多少钱。**

### 2. 计划资产公允价值（Fair Value of Plan Assets）

养老金计划已经积累并持有、专门用于支付员工福利的资产在报告日的公允价值，例如计划持有的股票、债券和现金。

直观理解：**养老金计划目前已经准备了多少钱。**

## 三、核心公式：净养老金头寸（Net Pension Position）

先比较企业的养老金义务和计划资产：

$$
\text{Net Pension Position} = \text{DBO} - \text{Fair Value of Plan Assets}
$$

其中：
- DBO 大于 Plan Assets：形成净养老金负债（Net Defined Benefit Liability）。
- Plan Assets 大于 DBO：形成计划盈余（Plan Surplus），可能形成净养老金资产（Net Defined Benefit Asset），但还要考虑资产上限（Asset Ceiling）。

可以记成一句话：

**净负债 = 未来需要支付的养老金 − 已经为养老金准备的计划资产。**

### 情况一：计划资产不足（Deficit）

假设：
- DBO = €12 million
- Plan Assets = €8 million

$$
12-8=€4\\ million
$$

计划资金比养老金义务少 €4 million，因此确认净养老金负债（Net Defined Benefit Liability）€4 million。

### 情况二：计划资产超过义务（Surplus）

假设：
- DBO = €15 million
- Plan Assets = €18 million

$$
15-18=-€3\\ million
$$

计算结果为负数，表示计划盈余 €3 million。若符合资产确认条件，可能确认净养老金资产（Net Defined Benefit Asset）；但**实际可确认资产受 Asset Ceiling 限制**，不能只凭负数结果就断定全部 €3 million 都能确认为资产。

## 四、为什么要用“净额”列示？

在符合适用会计准则的确认及抵销条件时，资产负债表（Balance Sheet）确认的是设定受益计划的净负债或净资产，而不是把 DBO 和计划资产简单作为两项独立项目相加列示。

| 计算结果 | 资产负债表列报 |
|---|---|
| DBO > Plan Assets | Net Defined Benefit Liability（净设定受益负债） |
| Plan Assets > DBO | Net Defined Benefit Asset（净设定受益资产），受 Asset Ceiling 限制 |

注意：这里是同一设定受益计划的净额计算，不代表企业可以把不同养老金计划的资产和负债任意互相抵销。不同计划之间是否可以抵销，需要满足准则规定的法律上可执行抵销权等条件。

## 五、资产上限（Asset Ceiling）

当计划资产超过 DBO 时，形成计划盈余（Plan Surplus）。但企业只有在能够通过退款（Refund）或减少未来缴款（Reduction in Future Contributions）等方式取得经济利益的范围内，才能确认净养老金资产。

因此：

$$
Recognized\\ Net\\ Pension\\ Asset
\\leq Plan\\ Surplus
$$

并且还受资产上限（Asset Ceiling）约束。简单记忆：**算出养老金盈余，不代表全部盈余都能确认为企业资产。**

## 六、与两种养老金计划的区别

| 比较 | Defined Benefit Plan | Defined Contribution Plan |
|---|---|---|
| 中文 | 设定受益计划 | 设定提存计划 |
| 企业承诺 | 约定员工未来获得的福利 | 约定企业缴纳的金额 |
| 主要风险 | 企业承担较多投资及精算风险 | 员工承担较多投资结果风险 |
| 资产负债表 | 确认净设定受益负债 / 资产 | 通常确认尚未缴纳的应付提存款 |
| 计算重点 | DBO − Plan Assets | 当期应缴金额及未缴余额 |

## 七、本题完整演算：Golden Corporation

题目数据（单位：€ thousands）：

| 项目 | 金额 |
|---|---:|
| Present Value of Pension Liabilities / DBO | €12,000 |
| Fair Value of Plan Assets | €8,000 |

计算：

$$
Net\\ Pension\\ Liability=12,000-8,000=€4,000
$$

因此，Golden 的资产负债表应列示 €4 million 的退休福利净负债，而不是分别将 €12 million 负债与 €8 million 计划资产作为两项独立金额列示。

正确选项：**B — €4 million is shown as retirement benefit obligations.**

## 八、常见考试陷阱

1. **DBO 不等于净养老金负债**：DBO 是养老金义务现值；还要减去计划资产公允价值，才得到净头寸。
2. **Plan Assets 不是企业可自由使用的普通现金**：它们属于养老金计划并用于支付员工福利。
3. **DBO > Plan Assets**：净负债；**Plan Assets > DBO**：计划盈余，可能形成净资产。
4. **净资产确认有 Asset Ceiling 限制**：盈余不一定能全部确认为资产。
5. **不能随意跨计划抵销**：不同设定受益计划之间的抵销需要满足准则条件。
6. **Defined Benefit 与 Defined Contribution 不同**：前者承诺福利金额，后者承诺缴费金额。

## 九、复习检查

- [ ] 能解释 DBO 与 Plan Assets 分别代表什么
- [ ] 能独立计算 Net Pension Liability / Asset
- [ ] 能判断净养老金负债与净养老金资产
- [ ] 能解释 Asset Ceiling 为什么限制净养老金资产
- [ ] 能区分 Defined Benefit Plan 与 Defined Contribution Plan
- [ ] 能解释资产负债表为什么列示净额
