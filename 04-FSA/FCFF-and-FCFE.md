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

## 7. 从 CFO（经营活动现金流）出发

若经营现金流 CFO 已反映利息支付（典型 US GAAP 情形），且不考虑额外特殊调整：

$$
\boxed{FCFF=CFO+Int(1-T)-FCInv}
$$

$$
\boxed{FCFE=CFO-FCInv+Net\ Borrowing}
$$

这与从 NI 出发的公式等价，因为在简化情况下：

$$
CFO=NI+NCC-WCInv
$$

若 IFRS 把利息支付分类在筹资活动，或题目有其他特殊项目，不能不加调整直接使用以上 CFO 版本。

### 固定资本净投资（Net Fixed Capital Investment）

购买设备的现金支出与出售旧设备的现金收入应当区分：

$$
\boxed{FCInv=Capital\ Expenditures-Proceeds\ from\ Asset\ Sales}
$$

题目只给出设备购买 5 million 和出售设备收款 2 million 时，净固定资本投资：

$$
FCInv=5-2=3\ million
$$

注意出售设备所产生的利润或亏损，不等于出售设备收到的现金。这里应使用 **Proceeds from Asset Sales（出售资产所得现金）**。

### 净借款（Net Borrowing）

$$
Net\ Borrowing=Debt\ Issued-Debt\ Repaid
$$

例如新借入 8 million，偿还本金 3 million，则净借款为 5 million。

### 计算示例（金额单位：million）

已知 CFO=30、Interest Expense=1、Tax Rate=40%、购买机器=5、出售设备收到现金=2、发行债务=8、偿还债务=3。

$$
FCFF=30+1(1-40\%)-(5-2)=\boxed{27.6}
$$

$$
FCFE=30-(5-2)+(8-3)=\boxed{32}
$$

可用转换关系核对：

$$
FCFE=FCFF-Int(1-T)+Net\ Borrowing=27.6-0.6+5=32
$$

## 8. NI 与 CFO 两种计算起点对照

| 起点 | FCFF | FCFE |
|---|---|---|
| Net Income（NI） | NI + NCC + Int(1-T) - FCInv - WCInv | NI + NCC - FCInv - WCInv + Net Borrowing |
| Cash Flow from Operations（CFO） | CFO + Int(1-T) - FCInv | CFO - FCInv + Net Borrowing |

**解题顺序：**先判断题目给的是 NI 还是 CFO；再求 FCInv、Net Borrowing；最后计算 FCFF、FCFE，并通过转换公式交叉验证。

- [ ] 能分别默写 NI 起点和 CFO 起点的两个公式
- [ ] 能计算出售设备后净固定资本投资
- [ ] 能区分 Debt Issued、Debt Repaid 与 Net Borrowing
