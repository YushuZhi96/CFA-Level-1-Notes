---
subject: Alternative Investments
topic: Leverage and Leveraged Returns
status: "🟡 待独立验证"
created: 2026-11-12
last-reviewed: 2026-11-12
tags: [CFA-L1, Alternative-Investments, Hedge-Funds, Leverage, Leveraged-Returns]
---

# 杠杆与杠杆收益率（Leverage and Leveraged Returns）

[[09-Alternative-Investments/INDEX|返回另类投资目录]]

## 一句话理解

对冲基金（Hedge Fund）可能利用**借款杠杆（Borrowing Leverage）**扩大投资头寸。若资产收益率高于借款利率，借款有望提高自有资本收益率；若低于借款利率，杠杆会拖累自有资本回报，且可能放大亏损。

## 核心概念 / 定义

- **Equity Capital (E)｜自有资本**：投资者实际承担风险的自有资金；计算杠杆后的自有资本收益率时作为分母。
- **Debt (D)｜借款资本**：投资使用的借入资金，需要承担融资利息。
- **Total Assets (A)｜总投资资产**：在简化融资结构下，$A=E+D$。
- **Asset Return ($R_A$)｜资产收益率**：整个投资资产组合在扣借款利息前的收益率。
- **Borrowing Rate / Cost of Debt ($R_D$)｜借款利率/借款成本**：为借款支付的利息率。
- **Leveraged Return on Equity ($R_E$)｜杠杆后权益收益率**：资产收益扣除利息后，相对于自有资本的收益率。

## 公式与变量

假设借入资金与自有资本投资同一资产组合，且无其他费用、税收和外部现金流。

$$
A=E+D
$$

投资收益扣除融资利息后的自有资本收益率：

$$
R_E=\frac{(E+D)R_A-DR_D}{E}
$$

整理得到考试快捷公式：

$$
\boxed{R_E=R_A+\frac{D}{E}(R_A-R_D)}
$$

变量：
- $R_E$：Leveraged Return on Equity，杠杆后自有资本收益率。
- $R_A$：Asset Return，资产收益率。
- $R_D$：Borrowing Rate，借款利率。
- $D/E$：Debt-to-Equity Ratio，债务与自有资本的比率。

**适用条件**：该式为单期、借款用于同一资产组合、融资利率已知、不考虑税费、管理费、追缴保证金及其他融资限制的简化模型。实际杠杆投资需考虑追加保证金、被迫平仓、融资再定价等风险。

## 两个最容易混淆的杠杆比率

- **Debt-to-Equity Ratio（$D/E$）｜债务权益比**：借款除以自有资本。
- **Assets-to-Equity Ratio（$A/E$）｜资产权益倍数**：总资产除以自有资本。

在 $A=E+D$ 时：

$$
\boxed{\frac{A}{E}=1+\frac{D}{E}}
$$

**判断重点**：题目说“adds 50% leverage”时，必须结合语境辨别其定义。本次题目将增加的借款理解为自有资本的 50%，对应 $D/E=0.5$、$A/E=1.5$；不能无条件把所有题目中的 50% 杠杆都视为同一口径。

## 杠杆增加还是减少收益？

根据公式 $R_E=R_A+(D/E)(R_A-R_D)$：

1. 当 $R_A>R_D$，新增杠杆提高自有资本收益率。
2. 当 $R_A=R_D$，借款成本抵消借入资产带来的收益，简化情形下杠杆不改变自有资本收益率。
3. 当 $R_A<R_D$，杠杆拖累自有资本收益率，并可能放大负收益。

融资成本通常需要支付，即使投资资产当期出现亏损也不能忽略。因此杠杆同时放大潜在收益和损失，不能把较高的**Leveraged Return**误判为没有额外风险。

## 常见考试陷阱

- **Return denominator**：求杠杆后权益收益率时除以 $E$，而不是总投资资产 $A$。
- **Borrowing cost**：资产总收益必须减去 $D\times R_D$ 的利息成本。
- **Leverage definition**：区分 $D/E$ 与 $A/E$，题目也可能使用其他杠杆定义。
- **Asset return vs. Equity return**：资产收益率不等于杠杆后的投资者权益收益率。
- **Loss amplification**：杠杆并非必然增加收益；收益率低于融资成本时会拖累表现。
- **Units**：金额单位应一致，收益率应与计算期间相匹配。

## 典型题型 / 判断路径

1. 确定自有资本 $E$，按题干杠杆口径计算借款 $D$。
2. 计算总投资额 $A=E+D$。
3. 用 $A\times R_A$ 计算资产收益，并扣除 $D\times R_D$ 借款利息。
4. 用净收益除以自有资本 $E$，或使用快捷公式交叉验证。
5. 确认答案求的是**自有资本收益率**，不是资产回报率。

## 易混知识点 / Obsidian 链接

- [[Alternative-Investments-Basics|另类投资基础：管理与风险]]：杠杆是策略灵活性来源之一，也构成杠杆风险。
- [[Hedge-Fund-Fee-Structures|对冲基金费用结构]]：借款利息（Borrowing Cost）不同于基金管理费（Management Fee）或业绩报酬（Incentive Fee）。若题目同时出现多种费用，需要按约定分别处理。

## 我的错因 / 验证记录

- 原题截图没有显示已选答案，不记录为独立答对或答错。
- 需要验证：能否准确区分 $D/E$ 与 $A/E$，并记得扣除融资利息。
- 复习状态：🟡 待独立验证。

## 复习检查清单

- [ ] 能独立写出 $R_E=R_A+(D/E)(R_A-R_D)$。
- [ ] 能明确区分 Debt-to-Equity 与 Assets-to-Equity。
- [ ] 能解释为何杠杆可同时放大收益和亏损。
- [ ] 能独立完成不同借款比例和融资成本的变式题。
