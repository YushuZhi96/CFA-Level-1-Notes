---
subject: Financial Statement Analysis
topic: Cash Flow Classification
status: "🟡 解析能懂，待独立验证"
created: 2026-11-03
last-reviewed:
tags: [CFA-L1, FSA, Cash-Flow, CFO, CFI, CFF, US-GAAP, IFRS]
---

# 现金流量表分类（Cash Flow Classification）——CFO、CFI、CFF 与 US GAAP / IFRS

## 一句话理解

现金流量表（Statement of Cash Flows）记录企业**一段期间**现金及现金等价物的流入和流出，按经营活动（CFO）、投资活动（CFI）、筹资活动（CFF）分类。

$$
Net\ Change\ in\ Cash=CFO+CFI+CFF+Effect\ of\ Exchange\ Rate\ Changes
$$

汇率变动对现金及现金等价物的影响通常单独列示，不是简单强塞入 CFO、CFI 或 CFF。

## 一、三大现金流分类

### 1. CFO：经营活动现金流（Cash Flow from Operating Activities）

企业主要创收活动及不能归为 CFI/CFF 的其他活动产生的现金流。

典型项目：
- Cash Received from Customers（销售收款）：流入
- Cash Paid to Suppliers（支付供应商）：流出
- Salaries / Wages Paid（支付员工工资）：流出
- Income Taxes Paid（支付所得税）：通常流出并归为 CFO
- US GAAP 下 Interest Paid、Interest Received、Dividends Received：通常 CFO（注意资本化利息、特殊分配等细节）

**考点：** Income Statement 上确认的收入费用并不等于现金收付，可能需要使用 BASE 法则转为现金流。

### 2. CFI：投资活动现金流（Cash Flow from Investing Activities）

取得和处置长期生产性资产，以及不属于现金等价物或交易性经营活动的相关投资等。

典型项目：
- Purchase of PP&E（购买厂房机器设备）：流出
- Sale of PP&E（出售设备）：流入
- Purchase of Long-term Investments（购买长期投资）：流出
- Sale of Long-term Investments（出售长期投资）：流入
- Loans Made to Other Entities（向其他企业提供贷款）：通常流出，收回本金通常流入（非金融机构普通企业的典型分类）

**考点：** 买设备是 CFI；卖设备收到的现金通常也是 CFI；处置损益可能出现在利润表，但现金流分类按实际收款判断。

### 3. CFF：筹资活动现金流（Cash Flow from Financing Activities）

导致企业权益资本及借款本金的规模或构成变化的现金活动。

典型项目：
- Proceeds from Share Issuance（发行股票收款）：流入
- Proceeds from Debt Issuance（发行债券、取得借款）：流入
- Repayment of Debt Principal（偿还债务本金）：流出
- Share Repurchase（股票回购）：流出
- Dividends Paid（支付股息）：US GAAP 下流出归 CFF
- Principal Portion of Lease Payments（租赁负债本金偿还）：通常归 CFF，须按适用准则判断

**考点：** 偿还**债务本金**是 CFF；利息支付在 US GAAP 下通常是 CFO，二者不能混淆。

## 二、US GAAP 与 IFRS（截至 2026 的传统 IAS 7 考试口径）

| 项目 | US GAAP | IFRS（2026 年现行 IAS 7 口径） |
|---|---|---|
| Interest Paid（支付利息） | CFO（不含须另行分类的资本化利息） | CFO 或 CFF |
| Interest Received（收到利息） | CFO | CFO 或 CFI |
| Dividends Received（收到股息） | CFO（典型情形；投资回报本金分配等例外另辨） | CFO 或 CFI |
| Dividends Paid（支付股息） | CFF | CFO 或 CFF |
| Income Taxes Paid（支付所得税） | 通常 CFO | 通常 CFO；若能明确识别与投资/筹资交易有关，可归 CFI/CFF |
| Bank Overdrafts（银行透支） | 通常不计入现金等价物；借入/偿还属于筹资现金流 | 若随时可偿还且构成日常现金管理组成部分，可计入现金及现金等价物 |

**简化记忆：**
- US GAAP：付息 CFO、收息 CFO、收股息 CFO、付股息 CFF、付所得税 CFO。
- IFRS（2026 传统）：收息/收股息 CFO 或 CFI；付息 CFO 或 CFF；付股息 CFO 或 CFF。
- IFRS 允许的选择并非随意每年更改，应保持一致分类。

参考：CFA Institute 2026《Analyzing Statements of Cash Flows I》、IAS 7、KPMG IFRS vs US GAAP Cash Flows。
来源：
- https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/analyzing-statements-of-cash-flows-i
- https://kpmg.com/us/en/articles/2022/ifrs-accounting-standards-us-gaap.html

## 三、IFRS 18 导致的 2027 年规则变化（重点避免混淆）

IFRS 18 对 IAS 7 的修改一般对 **2027 年 1 月 1 日或以后开始的年度报告期间**生效，允许提前应用。对**不以投资特定资产或向客户提供融资为指定主营业务**的普通企业：

| 现金流 | 2027 年起新规则 |
|---|---|
| Interest Received | CFI |
| Dividends Received | CFI |
| Interest Paid | CFF |
| Dividends Paid | CFF |

对于将投资或向客户提供融资作为特定主营业务的企业，利息和收到的股息等分类需要根据 IFRS 18 与修改后的 IAS 7 进一步判断；支付股息仍是 CFF。

因此考题如果明确给出年份、准则版本，应优先按题目要求。**2026 题库的传统 IAS 7 记忆表与 2027 新规则不要混用。**

参考 IFRS Foundation 官方说明：
https://www.ifrs.org/content/dam/ifrs/publications/amendments/english/2024/effect-analysis-ifrs18-april2024.pdf

## 四、本次例题：Gordon Co.（US GAAP）

已知（百万美元）：

| 现金流项目 | 金额 | 归类 |
|---|---:|---|
| Proceeds from Issuance of Shares | +200 | CFF |
| Redemption of Debenture Loan (Principal) | −170 | CFF |
| Dividend Payment | −10 | CFF |
| Tax Payment | −10 | CFO |

要求：2019 年筹资活动现金流（CFF）。

$$
CFF=200-170-10=\boxed{+\$20\ million}
$$

**正确答案 A**。错误答案 $10 million 是将所得税支付也从 CFF 中扣除。US GAAP 下本题的所得税付款应归 CFO。

## 五、三类现金流快速判断方法

1. 先识别是否发生**真实现金收付**，不要把非现金交易计入 CFO/CFI/CFF 的金额。
2. 判断是否主要为经营收付（CFO）、长期资产/投资买卖（CFI）、融资与资本返还（CFF）。
3. 若出现 Interest、Dividend、Income Tax，先确认 US GAAP 还是 IFRS，以及准则适用年份。
4. 最后统一现金流入记正号，现金流出记负号，求对应分类净现金流。

## 六、与 BASE 法则的关系

- **现金流分类**：知道现金交易金额，判断它归 CFO、CFI、CFF 哪一类。
- **BASE（B+A−S=E）**：不知道现金支付金额时，根据期初余额、本期变动和期末余额推导现金额。

例如：
- Cash Paid to Suppliers = COGS + ΔInventory − ΔAP（简化）
- Dividends Paid 需先由 Retained Earnings 求 Dividends Declared，再由 Dividends Payable 求现金支付（简化）

参见：[[BASE-Account-Reconciliation|BASE 法则：账户余额变动与直接法]]。

## 七、易错点与自测

- [ ] 能区分 CFO、CFI、CFF 三类典型现金活动
- [ ] 能解释偿还债务本金和支付利息为何可能分类不同
- [ ] 记住 US GAAP 下利息支付、利息收取、股息收取通常 CFO，股息支付 CFF
- [ ] 记住 IFRS（2026 口径）下利息/股息的分类选择
- [ ] 知道 2027 IFRS 18 对 IAS 7 的分类修改，避免跨版本混淆
- [ ] 能把 Gordon Co. 的 Tax Payment 排除在 CFF 之外
