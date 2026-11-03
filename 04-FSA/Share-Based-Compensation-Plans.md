---
subject: Financial Statement Analysis
topic: Share-Based Compensation Plans
status: "🟡 解析能懂，待独立验证"
created: 2026-11-03
last-reviewed:
tags: [CFA-L1, FSA, Share-Based-Compensation, IFRS-2, US-GAAP, Equity-Compensation]
---

# 股份支付计划（Share-Based Compensation Plans）

## 一句话理解

**股份支付（Share-Based Compensation / Share-Based Payment）**是企业以股票、期权或与股价相关的权利来交换员工服务或其他商品与服务的安排。授予时不需要立即支付现金，不代表没有费用或没有经济成本。

## 核心概念 / 定义

### 1. 常见股份支付工具

| 英文 | 中文 | 含义 |
|---|---|---|
| Stock Grant / Share Grant | 股票授予 | 直接授予股票，可能要求员工完成服务或满足业绩条件 |
| Share Options | 股票期权 | 员工按约定行权价（Exercise Price）购买股票的权利 |
| Stock Appreciation Rights (SARs) | 股票增值权 | 获得与股价上涨幅度相关的收益，可能现金结算或权益结算 |

### 2. 结算方式（Settlement Types）

- **Equity-Settled（权益结算）**：以权益工具作为对价，典型员工权益结算奖励通常根据授予日公允价值（Grant-Date Fair Value）计量，在服务期内确认薪酬费用（Compensation Expense），同时增加权益。
- **Cash-Settled（现金结算）**：通常确认负债，并在每个报告日重新计量公允价值直至结算，公允价值变动影响损益。
- SARs 并非一律现金结算；应根据合同确定结算方式。

### 3. 计量与等待期

- **Grant Date（授予日）**：奖励授予条款达成必要约定的日期。
- **Measurement Date（计量日）**：用于确定相关公允价值的日期，不能无条件与授予日划等号。
- **Vesting Period（等待期 / 归属期）**：员工需要提供服务或满足条件以取得奖励的期间。
- **Fair Value（公允价值）**：IFRS 与 US GAAP 下股份支付计量的重要基础，但现金结算与权益结算的后续计量不同。

## 公式与变量

假设授予 1,000 份权益结算股票期权，每份授予日公允价值为 $5，服务期 2 年，预计全部归属且服务均匀提供：

$$
Total\ Compensation\ Cost=1,000\times\$5=\$5,000
$$

$$
Annual\ Compensation\ Expense=\frac{\$5,000}{2}=\$2,500
$$

**适用条件：** 仅为简化示例，实际费用需要结合归属条件、预计归属数量、离职变化和奖励条款等调整。

## 直观理解 / 记忆方法

- **No Current Cash Outlay（当期没有现金支出）**：权益结算股票期权在授予时一般不需要现金支付，是保留现金（Cash Conservation）的优点。
- **No Current Cash Outlay ≠ No Compensation Expense**：不支付现金也仍可能确认薪酬费用、减少净利润。
- **Alignment of Interests（利益一致性）**：员工获得与股价挂钩的激励，可能使员工与股东的利益更一致。
- **Share Dilution / EPS Dilution（股份稀释 / 每股收益稀释）**：未来行权增加普通股数量，可能降低原股东持股比例与每股收益。
- 这类激励也可能促使管理层过分关注短期股价或承担过高风险，因此并非完全没有缺点。

## IFRS 2 信息披露要求（Disclosure Requirements）

### 1. Share Options（股票期权）

- IFRS 2 第 45(b) 段：披露不同状态股票期权的数量和加权平均行权价格（Weighted Average Exercise Price），例如期初发行在外、本期授予、行权、失效以及期末在外等。
- IFRS 2 第 47(a) 段：披露本期授予股票期权在计量日的加权平均公允价值（Weighted Average Fair Value）和估值方法、期权定价模型的重要输入变量。

### 2. Other Equity Instruments（其他权益工具）

- IFRS 2 第 47(b) 段：披露除股票期权以外本期授予权益工具的**数量、计量日加权平均公允价值及估值方法**。

**重要区别：** 股票期权并非不披露数量或公允价值，而是与其他权益工具适用不同的具体披露条款。若 SARs 以现金结算，需结合其负债结算属性适用相关规定，不可机械当作其他权益工具。

## 财务报表影响（Financial Statement Effects）

典型员工权益结算奖励，在员工提供服务期间：

| 报表 | 主要影响 |
|---|---|
| Income Statement（利润表） | 确认 Compensation Expense，其他条件不变时 Net Income 降低 |
| Balance Sheet（资产负债表） | 费用通常减少留存收益，同时确认相应权益项目增加；不能直接断言总权益必然增加 |
| Cash Flow Statement（现金流量表） | 确认非现金费用本身不导致现金流出；间接法计算 CFO 时通常加回非现金费用 |

现金结算奖励则可能带来未来实际现金流出，并需按负债的公允价值变化重新计量。

## 常见考试陷阱

1. **No Current Cash Outlay 是 Advantage（优点）而不是 Disadvantage（缺点）**。
2. 不需要当期现金支出不代表没有经济成本，更不代表不影响净利润。
3. IFRS 与 US GAAP 均以公允价值计量为股份支付会计处理的重要原则，但具体结算方式、估值日期与后续计量有所不同。
4. 股份支付有助于 Alignment of Interests，但也可能带来 Share Dilution 和激励扭曲。
5. 区分 **Weighted Average Exercise Price（加权平均行权价）** 与 **Weighted Average Fair Value（加权平均公允价值）**。
6. Share Options 不属于 IFRS 2 第 47(b) 段所述的其他权益工具，但另有数量和公允价值披露要求。

## 典型题型 / 判断路径

- 题目询问 IFRS 2 中“数量与计量日加权平均公允价值”的特定披露组合：先区分第 47(a) 段的股票期权与第 47(b) 段的其他权益工具。
- 题目询问股票期权不需要当期现金支出是不是缺点：这是典型优点，**不是缺点**。
- 题目询问费用确认：即使权益结算、授予时没有现金流出，服务期内仍可能产生薪酬费用。
- 题目询问结算性质：先判断 Equity-Settled 或 Cash-Settled，再判断影响权益还是负债。

## 易混知识点 / Obsidian 链接

- [[Earnings-Per-Share-EPS|每股收益（EPS）：股票期权的潜在稀释]]
- [[Cash-Flow-Classification-US-GAAP-IFRS|现金流分类：非现金费用与实际现金支付]]
- [[Common-Size-Statements-and-Financial-Ratios|财务比率：净利润与权益变化]]

## 我的错因 / 验证记录

**题目一：IFRS 2 披露要求。** 正确选项为 Share Options（股票期权），因为题干使用第 47(b) 段对其他权益工具的特定组合表述；注意股票期权也需要披露数量与公允价值。

**题目二：股份支付优缺点。** 正确答案 C。错误陈述把“没有当期现金支出”说成股票期权的缺点；实际上通常是优点，但授予不等于没有薪酬费用。

- [ ] 能独立解释三种股权激励工具
- [ ] 能区分 Equity-Settled 与 Cash-Settled
- [ ] 能计算简单的薪酬费用
- [ ] 能区分 IFRS 2 第 45、47(a)、47(b) 段
- [ ] 能解释当期不支付现金与确认费用的区别
- [ ] 能独立完成一道同类新题
