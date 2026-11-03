---
subject: Financial Statement Analysis
topic: BASE Account Reconciliation
status: "🟡 解析能懂，待独立验证"
created: 2026-11-03
last-reviewed:
tags: [CFA-L1, FSA, Cash-Flow, BASE, Direct-Method]
---

# BASE 法则：账户余额变动与现金流量表直接法

## 一句话理解

**BASE 是账户余额调节方法（Account Balance Reconciliation）**：期初余额 + 本期增加 − 本期减少 = 期末余额。它是便于解题的记忆框架，并非独立的会计准则。

## 核心公式

$$
\boxed{B+A-S=E}
$$

| 字母 | 英文 | 中文 |
|---|---|---|
| B | Beginning Balance | 期初余额 |
| A | Additions | 本期增加 |
| S | Subtractions | 本期减少 |
| E | Ending Balance | 期末余额 |

**注意：A、S 是所选账户的增加与减少，不能机械等同现金流入、现金流出。**

统一约定：

$$
\Delta X = Ending\ X-Beginning\ X
$$

## 典型应用一：存货（Inventory）

在无其他存货调整、损耗或非采购增加的简化题目中：

$$
Beginning\ Inventory+Purchases-COGS=Ending\ Inventory
$$

移项：

$$
\boxed{Purchases=COGS+\Delta Inventory}
$$

存货增加意味着采购超过销售成本，因此增加额需要加回 COGS。

## 典型应用二：应付账款（Accounts Payable, AP）

在应付账款只涉及赊购与付款的简化题目中：

$$
Beginning\ AP+Credit\ Purchases-Cash\ Paid=Ending\ AP
$$

因此：

$$
\boxed{Cash\ Paid=Credit\ Purchases-\Delta AP}
$$

若题目默认采购均经过应付账款账户、且没有其他调整，可将上面的 Purchases 代入：

$$
\boxed{Cash\ Paid\ to\ Suppliers=COGS+\Delta Inventory-\Delta AP}
$$

应付账款增加，说明更多款项尚未支付，所以现金支出相对采购金额较少。

## 典型应用三：应收账款（Accounts Receivable, AR）

在应收账款只涉及赊销与收款的简化题目中：

$$
Beginning\ AR+Credit\ Sales-Cash\ Collected=Ending\ AR
$$

移项：

$$
\boxed{Cash\ Collected=Credit\ Sales-\Delta AR}
$$

若题目默认收入全部进入应收账款、无坏账核销等其他变化，可用 Revenue 代替 Credit Sales：

$$
Cash\ Collected=Revenue-\Delta AR
$$

应收账款增加，意味着更多销售收入尚未收到现金。

## 典型应用四：应付利息和应付所得税

在费用与对应应付款项之间无其他调整的简化情形：

$$
Cash\ Interest\ Paid=Interest\ Expense-\Delta Interest\ Payable
$$

$$
Cash\ Taxes\ Paid=Income\ Tax\ Expense-\Delta Income\ Tax\ Payable
$$

注意实际题目可能还涉及递延所得税、资本化利息或其他调整，不能不加判断直接套用。

## 本次题目：Cash Paid to Suppliers

已知：
- COGS = $65,000
- Beginning AP = $21,000
- Ending AP = $48,000
- Inventory 增加 $3,000

**第一步：Inventory BASE**

$$
Purchases=65,000+3,000=\$68,000
$$

**第二步：AP BASE**

$$
\Delta AP=48,000-21,000=\$27,000
$$

$$
Cash\ Paid=68,000-27,000=\boxed{\$41,000}
$$

正确答案：**B，$41,000**。

## 速查：方向与含义

| 变动 | 对相应现金流量的方向影响（其他条件不变） |
|---|---|
| Inventory ↑ | Cash Paid to Suppliers ↑ |
| Inventory ↓ | Cash Paid to Suppliers ↓ |
| AP ↑ | Cash Paid to Suppliers ↓ |
| AP ↓ | Cash Paid to Suppliers ↑ |
| AR ↑ | Cash Collected from Customers ↓ |
| AR ↓ | Cash Collected from Customers ↑ |

## 考试常见陷阱

1. **BASE 的 Additions 不一定是现金收入**：例如 AP 增加是欠款增多。
2. **COGS ≠ Purchases ≠ Cash Paid**：销售成本、采购、现金支付属于不同环节。
3. **Revenue ≠ Cash Collected**：收入确认和现金收款不一定同步。
4. **把变化量定义清楚**：此处始终用期末减期初，避免符号颠倒。
5. **留意简化假设**：坏账核销、非现金交易、并购或外币折算可能影响账户余额，现实中需额外调整。
6. **先画账户再移项**：忘记公式时，回到 Beginning + Additions − Subtractions = Ending。

## 自测

- [ ] 不看笔记写出 B+A−S=E 的每个字母
- [ ] 从 Inventory BASE 推出 Purchases
- [ ] 从 AP BASE 推出 Cash Paid
- [ ] 从 AR BASE 推出 Cash Collected
- [ ] 解释为什么 AP 增加导致支付现金减少
- [ ] 独立做对一道新的直接法计算题

## 后续关联

- [[Balance-Sheet-Fundamentals|资产负债表基础概念]]
- [[Revenue-Recognition-and-Contract-Liabilities|收入确认与合同负债]]
