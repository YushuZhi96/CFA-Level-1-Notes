---
subject: Financial Statement Analysis
topic: Defined Benefit vs Defined Contribution Pension Plans
status: "🟡 解析能懂，待独立验证"
created: 2026-11-03
last-reviewed:
tags: [CFA-L1, FSA, Pension, Defined-Benefit, Defined-Contribution]
---

# 两种养老金计划的区别（Defined Benefit vs. Defined Contribution Plans）

## 一、先记住最核心的区别

- **Defined Benefit Plan（设定受益计划，DB Plan）**：企业承诺员工退休后获得多少福利（Benefit），企业需要估计并承担相应的养老金义务。
- **Defined Contribution Plan（设定提存计划，DC Plan）**：企业承诺向养老金计划缴纳多少金额（Contribution），员工最终获得多少退休福利，通常取决于累计缴款及投资表现。

记忆：
- DB = Guarantee the Benefit（承诺福利）。
- DC = Guarantee the Contribution（承诺缴款）。

## 二、核心对比表

| 比较维度 | Defined Benefit Plan（DB） | Defined Contribution Plan（DC） |
|---|---|---|
| 中文 | 设定受益计划 | 设定提存计划 |
| 企业承诺 | 约定员工退休后获得的福利金额 / 计算方式 | 约定企业缴纳的金额或比例 |
| 退休福利金额 | 按计划公式确定，通常与工资、工龄等因素有关 | 取决于缴款累计额及投资回报 |
| 企业主要义务 | 需要估计未来福利义务，并确保计划按规定履行 | 按期缴纳约定的提存金额 |
| 投资风险（Investment Risk） | 主要由雇主 / 计划发起人承担 | 通常主要由员工承担 |
| 精算风险（Actuarial Risk） | 主要由雇主 / 计划发起人承担 | 通常主要由员工承担 |
| 资产负债表 | 确认净设定受益负债或净资产 | 通常确认尚未缴纳的应付提存款 |
| 计算重点 | DBO 与 Plan Assets 的差额 | 当期应缴金额及尚未缴纳金额 |

## 三、分别怎么理解？

### 1. 设定受益计划（Defined Benefit Plan）

企业承诺的是员工未来能获得的养老金福利，而不是只承诺缴一笔固定金额。

例如：公司承诺员工退休后，每年领取一定金额的养老金。企业需要估计：
- 员工未来工资及工龄等相关因素；
- 退休年龄及预计领取年限；
- 未来需要支付的养老金金额；
- 折现率、死亡率等精算假设；
- 养老金计划资产未来表现。

因此，企业需要计算 **Defined Benefit Obligation（DBO，设定受益义务现值）**，并与计划资产（Plan Assets）比较。

简化净头寸：

$$
\text{Net Defined Benefit Position}
=
\text{DBO}
-
\text{Fair Value of Plan Assets}
$$

- DBO > Plan Assets：通常形成 Net Defined Benefit Liability（净设定受益负债）。
- Plan Assets > DBO：形成 Plan Surplus（计划盈余），可能确认净资产，但受 Asset Ceiling（资产上限）限制。

### 2. 设定提存计划（Defined Contribution Plan）

企业承诺的是缴款金额，例如每月按员工工资的 8% 缴纳养老金。

企业按约定缴纳后，员工退休时最终能获得多少，取决于：
- 企业和员工累计缴款；
- 养老金账户的投资回报；
- 投资期间及市场表现。

企业通常不承诺员工最终养老金金额。因此，企业一般将当期应缴的提存款确认为费用；若报告日尚未缴纳，则确认相应负债。

## 四、风险由谁承担？

这是 CFA 常见比较点。

| 风险 | DB Plan | DC Plan |
|---|---|---|
| 投资风险（Investment Risk） | 主要由雇主承担 | 通常由员工承担 |
| 精算风险（Actuarial Risk） | 主要由雇主承担 | 通常由员工承担 |
| 提前离职 / 未归属风险（Early Termination / Vesting Risk） | 员工可能因未达到归属条件而失去部分预期福利，取决于计划条款 | 员工也可能受未归属缴款条款影响，取决于计划条款 |

**特别区分：**
- “员工承担投资风险”通常是 DC Plan 的典型特征。
- “员工可能因提前离职而失去尚未归属的福利（Unvested Benefits）”是计划归属条款（Vesting Rules）带来的风险，不能与投资风险混为一谈。
- 是否会失去福利、失去多少，取决于计划文件及适用法律，不应理解为所有 DB 计划都必然如此。

## 五、常见英文关键词

| 关键词 | 中文 | 对应理解 |
|---|---|---|
| Benefit | 福利 / 退休待遇 | DB 的承诺重点 |
| Contribution | 缴款 / 提存 | DC 的承诺重点 |
| Benefit Obligation | 福利义务 | DB 需要估计的未来义务 |
| Defined Benefit Obligation (DBO) | 设定受益义务现值 | DB 养老金义务的现值 |
| Plan Assets | 计划资产 | 用于支付养老金福利的资产 |
| Investment Risk | 投资风险 | 计划资产投资表现不确定的风险 |
| Actuarial Risk | 精算风险 | 寿命、工资、退休时间等精算假设变化带来的风险 |
| Vesting | 权益归属 | 员工满足服务年限等条件后取得福利权益 |
| Unvested Benefits | 尚未归属的福利 | 员工尚未满足归属条件、可能无法取得的福利 |

## 六、本次 CFA 题目：哪项不是 DB Plan 的特征？

题目问：Which is least likely to be a characteristic of a defined benefit plan?

- A. Benefit obligation would be projected.（需要预测福利义务。）——是 DB 特征，因为企业必须估计未来福利义务。
- B. Employers need only to guarantee the contribution.（雇主只需保证缴款金额。）——这是 DC Plan 的特征，不是 DB Plan。
- C. Employees bear early termination risk.（员工可能承担提前离职风险。）——在计划存在归属条件时，员工可能失去尚未归属的部分福利；具体取决于计划条款。

**正确答案：B。**

## 七、考试速记

1. DB：承诺退休福利（Benefit），企业承担主要投资及精算风险，需要估计 DBO。
2. DC：承诺缴款金额（Contribution），员工通常承担主要投资风险。
3. DB 的资产负债表重点：DBO − Plan Assets，形成净养老金负债 / 资产（净资产受 Asset Ceiling 限制）。
4. DC 的资产负债表重点：报告日尚未缴纳的应付提存款。
5. Early Termination / Vesting Risk 与 Investment Risk 不同；提前离职是否影响福利取决于归属条款。

## 八、复习检查

- [ ] 能用一句话区分 DB 与 DC 的企业承诺
- [ ] 能区分两种计划的投资风险与精算风险
- [ ] 能解释 DB 为什么需要预测 DBO
- [ ] 能说出 DC 计划下企业通常确认什么负债
- [ ] 能解释 Vesting 与 Early Termination Risk
- [ ] 能独立完成本次题目及类似比较题
