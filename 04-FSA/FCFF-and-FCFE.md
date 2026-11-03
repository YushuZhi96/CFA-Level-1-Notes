# FCFF 与 FCFE：自由现金流公式

## 1. 定义
- **FCFF (Free Cash Flow to the Firm)**：企业自由现金流，面向股东和债权人。
- **FCFE (Free Cash Flow to Equity)**：股权自由现金流，面向普通股股东。

## 2. 从净利润出发的公式

$$
FCFF=NI+NCC+Int(1-T)-FCInv-WCInv
$$

$$
FCFE=NI+NCC-FCInv-WCInv+Net\ Borrowing
$$

变量：
- NI = Net Income（净利润）
- NCC = Non-cash Charges（非现金费用，例如折旧）
- Int = Interest Expense（利息费用）
- T = Tax Rate（税率）
- FCInv = Fixed Capital Investment（固定资本投资）
- WCInv = Working Capital Investment（经营性营运资本净投入）
- Net Borrowing = New Debt - Debt Repayment（净借款）

## 3. 相互转换

$$
FCFE=FCFF-Int(1-T)+Net\ Borrowing
$$

## 4. 为什么这样计算？
- 非现金折旧加回；资本性支出和营运资本投入扣除。
- FCFF 加回税后利息，因为它面向全部资本提供者。
- FCFE 从净利润出发不加回利息，但计入净借款。
- Dividend Paid（已支付股息）不直接扣减，因为自由现金流不等于已分配现金。

## 5. 简化示例
NI=90,000；折旧=8,000；营运资本投入=12,000；资本支出=40,000；利息费用=5,000；税率=30%；净借款=20,000。

$$
FCFF=90,000+8,000+5,000(1-30\%)-40,000-12,000=49,500
$$

$$
FCFE=90,000+8,000-40,000-12,000+20,000=66,000
$$

## 6. 考试易错点
- FCFF 要加回 **after-tax interest**，不是全额利息。
- FCFE 要考虑 **net borrowing**。
- WCInv 通常指非现金经营性营运资本的净增加，不是所有流动资产减流动负债的变化。
- 使用 CFO 起步的替代公式时，须留意 US GAAP / IFRS 对利息现金流的分类。
- 估值时 FCFF 通常配 WACC；FCFE 通常配 Cost of Equity。
