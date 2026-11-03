---
subject: Financial Statement Analysis
topic: Lease Accounting — IFRS 16 vs US GAAP ASC 842
status: "🟡 解析能懂，待独立验证"
created: 2026-11-03
last-reviewed:
tags: [CFA-L1, FSA, Lease-Accounting, IFRS-16, US-GAAP, ASC-842, Lessee, Lessor]
---

# 租赁会计（Lease Accounting）：IFRS 16 vs US GAAP ASC 842

## 一句话理解

租赁会计先分清身份：**Lessee（承租人）**是租入资产的一方，**Lessor（出租人）**是出租资产的一方。US GAAP ASC 842 下，承租人区分 **Operating Lease（经营租赁）** 与 **Finance Lease（融资租赁）**；IFRS 16 下，承租人主要采用**单一租赁会计模型**，而出租人仍区分融资租赁与经营租赁。

## 核心概念 / 定义

- **Right-of-Use Asset (ROU Asset，使用权资产)**：承租人在租赁期内使用标的资产的权利。
- **Lease Liability（租赁负债）**：承租人对未来租赁付款承担的现时义务。
- **Lease Commencement Date（租赁期开始日）**：标的资产可供承租人使用之日；与合同签订日（Inception Date）可能不同。
- **Finance Lease（融资租赁）**：从承租人角度更接近融资取得使用权；从出租人角度通常转移与所有权相关的几乎全部风险与报酬。
- **Operating Lease（经营租赁）**：不符合融资租赁分类的租赁，后续费用或出租方收入的处理不同。

## 一、承租人（Lessee）：IFRS 与 US GAAP 核心差异

| 比较 | IFRS 16 | US GAAP — Finance Lease | US GAAP — Operating Lease |
|---|---|---|---|
| 承租人分类 | 单一模型（多数租赁） | 融资租赁 | 经营租赁 |
| 初始 ROU Asset | 确认 | 确认 | 确认 |
| 初始 Lease Liability | 确认 | 确认 | 确认 |
| 负债初始计量 | 未付租赁付款额现值 | 未付租赁付款额现值 | 未付租赁付款额现值 |
| 利润表后续费用 | 单独折旧与利息 | 单独摊销与利息 | 通常单项租赁费用（Single Lease Cost） |
| 费用分布 | 通常前高后低 | 通常前高后低 | 通常相对均匀 |

此表描述典型情形，不考虑短期租赁等豁免、特殊变动租金和减值。

**关键：US GAAP 下经营租赁也通常需要确认租赁负债，并不是表外经营租赁。**

## 二、公式与变量

### 1. 租赁负债初始计量

$$
Lease\ Liability_{0}=PV(Unpaid\ Lease\ Payments)
$$

PV = Present Value（现值），折现率根据适用准则和资料确定。

### 2. 使用权资产的初始计量（简化）

$$
ROU\ Asset_{0}=Initial\ Lease\ Liability+Prepaid\ Lease\ Payments+Initial\ Direct\ Costs-Lease\ Incentives
$$

实际还需考虑适用准则下的具体定义和调整项目；使用权资产不必始终等于租赁负债。

### 3. 融资租赁利息费用

$$
Interest\ Expense=Beginning\ Lease\ Liability\times Discount\ Rate
$$

租赁付款中偿还本金部分减少租赁负债；利息和使用权资产折旧/摊销通常分别列报。

## 三、现金流量表分类（Cash Flow Classification）

### 2026 年传统 IAS 7 考试口径

| 项目 | IFRS 16（承租人） | US GAAP Finance | US GAAP Operating |
|---|---|---|---|
| 偿还租赁负债本金 | CFF | CFF | 经营租赁付款通常 CFO |
| 支付租赁负债利息 | CFO 或 CFF（IAS 7 传统口径） | CFO（通常） | 经营租赁付款通常 CFO |
| 未纳入租赁负债的可变租赁付款 | 通常 CFO | 通常 CFO | 通常 CFO |

**注意：** IFRS 18 自 2027-01-01 或以后开始的年度期间起生效，并对 IAS 7 的利息、股息现金流分类作了修订；复习时不要直接把 2026 年题库的传统选择分类机械套用到 IFRS 18 新期间。租赁本金的 CFF 处理应与利息现金流分类分开记忆。

## 四、出租人（Lessor）：两套准则的区别

| 项目 | IFRS 16 Lessor | US GAAP ASC 842 Lessor |
|---|---|---|
| 主要分类 | Finance / Operating | Sales-type / Direct Financing / Operating |
| Operating Lease | 一般继续确认标的资产，并在租赁期内确认租金收入 | 一般继续确认标的资产及租赁收入 |
| Finance 或融资性质租赁 | 通常终止确认标的资产并确认 Net Investment in Lease（租赁净投资） | 按 Sales-type 或 Direct Financing 的相应规则确认租赁净投资、损益及利息收入 |

**不要把承租人的 IFRS 单一模型套用到出租人：IFRS 出租人仍有两种分类。**

## 五、典型题型 / 判断路径

本次题目询问：在 **US GAAP** 下，承租人使用 Operating Lease 而不是 Finance Lease，最不可能出现什么结果？

- A 更低的 Interest Expense：Operating Lease 通常不单独列示利息费用，作为考试的常见对照成立。
- B 租赁开始日更低的 Lease Liability：**不成立**。两类租赁的负债都按未来未付租赁付款额现值初始计量，在相同条款下通常相同。
- C 更低的 Amortization Expense：Operating Lease 通常不单独列示使用权资产摊销费用；融资租赁单独确认。

**正确答案：B。**

说明：经营租赁负债在后续计量中仍有利息增计的计算过程，只是利润表通常列示单项租赁费用。因此不能错误地理解为经营租赁完全没有利息成本。

## 六、常见考试陷阱

1. **经营租赁 ≠ 完全不入表**：ASC 842 下绝大多数承租人经营租赁确认 ROU Asset 和 Lease Liability。
2. **开始日负债不因 Operating/Finance 分类本身而降低**：同样条款下起点通常一致。
3. **单项租赁费用 ≠ 经济上没有利息或资产使用成本**：关键是列报和费用模式。
4. **IFRS 的 Lessee 单一模型 ≠ Lessor 单一模型**：出租人仍区分 Operating/Finance。
5. **Operating 租赁付款在 US GAAP 通常 CFO；Finance 租赁本金 CFF、利息通常 CFO**。
6. 与旧 US GAAP ASC 840 区别：旧规则下多数经营租赁可以不在承租人资产负债表确认；不要和 ASC 842 混淆。
7. 碰到租赁费用计算，要检查折现率、付款时点和租赁期；首期/期末现金流的计算可能不同。

## 七、直观理解 / 记忆方法

- **Lessee：IFRS 单一，US GAAP 两类**。
- **Both US GAAP lease types: ROU Asset + Lease Liability at commencement**。
- **Finance: Interest + Amortization；Operating: Single Lease Cost**。
- **Lessor：IFRS 仍分 Finance / Operating**。

## 八、易混知识点 / Obsidian 链接

- [[Cash-Flow-Classification-US-GAAP-IFRS|现金流分类（CFO、CFI、CFF）]]
- [[Common-Size-Statements-and-Financial-Ratios|财务比率分析]]
- [[Balance-Sheet-Fundamentals|资产负债表基础]]

## 我的错因 / 验证记录

本题关键是将“经营租赁不单列利息与摊销费用”与“经营租赁不确认负债”区分开。后者是旧准则常见印象，不适用于现行 ASC 842 的一般承租人租赁。

- [ ] 能区分 Lessee / Lessor
- [ ] 能解释 IFRS 承租人模型和 US GAAP 双分类
- [ ] 能写出 Lease Liability = PV(Lease Payments)
- [ ] 能解释 Operating Lease 仍然入表
- [ ] 能判断两类租赁在 CFO/CFF 的分类差异
- [ ] 能独立完成一道同类新题
