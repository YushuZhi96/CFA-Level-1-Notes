---
subject: Financial Statement Analysis
topic: FSA Formula Handbook
status: "🟡 公式整理，待独立运用"
created: 2026-11-04
tags: [CFA-L1, FSA, Formulas, Financial-Ratios, DuPont]
---

# CFA 一级财报公式总表（FSA Formula Handbook）

> 这份笔记是 **FSA 的统一公式入口**：集中放公式、变量解释、经济含义、使用条件与常见陷阱。各专题笔记继续保留详细理论和更多案例。百分比指标通常可写为 0.27 或 27%；周转率和流动比率通常使用“倍 / 次”。

## 一、基础：三大报表与会计恒等式

### 1. 会计恒等式（Accounting Equation）

$$
\text{Assets}=\text{Liabilities}+\text{Equity}
$$

- Assets：资产，企业拥有或控制的经济资源。
- Liabilities：负债，企业现时义务。
- Equity：股东权益，资产扣除负债后的剩余权益。

由此可求股东权益：

$$
\text{Equity}=\text{Assets}-\text{Liabilities}
$$

### 2. 留存收益（Retained Earnings）

$$
\text{Ending RE}=\text{Beginning RE}+\text{Net Income}-\text{Dividends}
$$

- Net Income：本期净利润。
- Dividends：本期确认的股利分配。
- RE：留存收益。该式为未考虑其他调整的简化形式；留存收益并不等于现金余额。

## 二、短期偿债能力（Liquidity Ratios）

三者的分母均为 **Current Liabilities（流动负债）**，但分子越来越严格。

### 1. 流动比率（Current Ratio）

$$
\text{Current Ratio}=
\frac{\text{Current Assets}}{\text{Current Liabilities}}
$$

含义：每 1 元流动负债有多少流动资产覆盖。流动资产包含现金、短期证券、应收账款、存货、预付费用等，不能全部看成现金。

### 2. 速动比率（Quick Ratio / Acid-test Ratio）

$$
\text{Quick Ratio}=
\frac{\text{Cash}+\text{Marketable Securities}+\text{Receivables}}
{\text{Current Liabilities}}
$$

含义：不依赖销售存货等方式，用流动性更强的资产覆盖短期负债。通常剔除 Inventory（存货）和 Prepaid Expenses（预付费用）；若还有其他不够流动的资产，也应根据题目口径判断。

### 3. 现金比率（Cash Ratio）

$$
\text{Cash Ratio}=
\frac{\text{Cash and Cash Equivalents}+\text{Short-term Marketable Securities}}
{\text{Current Liabilities}}
$$

含义：单靠现金、现金等价物和可迅速变现的短期有价证券覆盖短期负债的程度。若 Cash 已包含 Cash Equivalents，不要重复加计。

通常：

$$
\text{Current Ratio}\geq\text{Quick Ratio}\geq\text{Cash Ratio}
$$

### 4. 营运资本（Working Capital）

$$
\text{Working Capital}=\text{Current Assets}-\text{Current Liabilities}
$$

这是**金额**，不是比率。

## 三、利润率、周转率与回报率（Profitability, Activity & Returns）

### 1. 毛利率（Gross Profit Margin）

$$
\text{Gross Profit Margin}=\frac{\text{Gross Profit}}{\text{Revenue}}
$$

其中 Gross Profit = Revenue − COGS（营业成本）。衡量销售收入扣除销售成本后剩余的比例。

### 2. 营业利润率（Operating Profit Margin）

$$
\text{Operating Profit Margin}=\frac{\text{Operating Income}}{\text{Revenue}}
$$

反映主营经营活动的获利能力；不同报表的 Operating Income 口径需核对。

### 3. 净利润率（Net Profit Margin）

$$
\text{Net Profit Margin}=\frac{\text{Net Income}}{\text{Revenue}}
$$

含义：每 1 元营业收入最终转化成多少净利润。

### 4. 总资产周转率（Total Asset Turnover）

$$
\text{Total Asset Turnover}=
\frac{\text{Revenue}}{\text{Average Total Assets}}
$$

含义：每 1 元平均资产创造多少收入。**Revenue 是期间流量，Assets 是时点存量**，通常要用平均资产：

$$
\text{Average Assets}=
\frac{\text{Beginning Assets}+\text{Ending Assets}}{2}
$$

### 5. 资产回报率（Return on Assets, ROA）

$$
\text{ROA}=\frac{\text{Net Income}}{\text{Average Total Assets}}
$$

常见简化口径。部分教材/分析目的可能对分子作税后利息调整，做题依题目指定口径。

### 6. 股东权益回报率（Return on Equity, ROE）

$$
\text{ROE}=\frac{\text{Net Income}}{\text{Average Shareholders' Equity}}
$$

含义：每 1 元平均账面股东权益，企业赚了多少净利润。

$$
\text{Average Equity}=
\frac{\text{Beginning Equity}+\text{Ending Equity}}{2}
$$

## 四、杜邦分析（DuPont Analysis）：把三个公式连起来

### 1. 权益乘数（Equity Multiplier）

$$
\text{Equity Multiplier}=
\frac{\text{Average Total Assets}}{\text{Average Equity}}
$$

含义：资产相对于股东权益的倍数，反映财务杠杆程度。两者须使用一致期间的平均余额。

### 2. 三因素杜邦公式（Three-factor DuPont Identity）

$$
\boxed{
\text{ROE}=
\text{Net Profit Margin}\times
\text{Total Asset Turnover}\times
\text{Equity Multiplier}
}
$$

展开各项：

$$
\frac{\text{Net Income}}{\text{Revenue}}
\times
\frac{\text{Revenue}}{\text{Average Assets}}
\times
\frac{\text{Average Assets}}{\text{Average Equity}}
=
\frac{\text{Net Income}}{\text{Average Equity}}
$$

理解：ROE 可从 **盈利能力（Margin）× 资产使用效率（Turnover）× 杠杆（Multiplier）** 三方面解释。

要求总资产周转率时，直接变形：

$$
\boxed{
\text{Total Asset Turnover}=
\frac{\text{ROE}}
{\text{Net Profit Margin}\times\text{Equity Multiplier}}
}
$$

### 3. 简化例题：反推资产周转率

假设某公司（金额单位：百万美元）：

| 项目 | 期初 | 期末 |
|---|---:|---:|
| Assets（资产） | 127,136 | 120,406 |
| Liabilities（负债） | 69,153 | 64,628 |

另有 ROE = 27%，Net Profit Margin = 23%。

**步骤一：求每年权益**

$$
\text{Beginning Equity}=127,136-69,153=57,983
$$

$$
\text{Ending Equity}=120,406-64,628=55,778
$$

**步骤二：求平均资产和平均权益**

$$
\text{Average Assets}=\frac{127,136+120,406}{2}=123,771
$$

$$
\text{Average Equity}=\frac{57,983+55,778}{2}=56,880.5
$$

**步骤三：求权益乘数**

$$
\text{Equity Multiplier}=\frac{123,771}{56,880.5}\approx2.176
$$

**步骤四：反推周转率**

$$
\text{Total Asset Turnover}=
\frac{0.27}{0.23\times2.176}\approx0.54
$$

资产周转率约 **0.54 次（或 54%）**。它表示每 1 美元平均资产创造约 0.54 美元收入，**不是净利润率**。

### 4. 两因素杜邦公式（Two-factor ROE Identity）

$
\text{ROE}=\text{ROA}\times\text{Financial Leverage}
$

这里采用：

$
\text{ROA}=\frac{\text{Net Income}}{\text{Average Assets}}
\qquad
\text{Financial Leverage}=
\frac{\text{Average Assets}}{\text{Average Equity}}
$

两式相乘时，Average Assets 约掉，得到 Net Income / Average Equity，即 ROE。**该等式要求 ROA 使用净利润口径，且资产与权益使用相同期间的平均余额。** 如果 ROA 用税后利息调整的不同口径，就不能不加调整地直接相乘。

### 5. 五因素杜邦分析（Five-factor DuPont Analysis）

在三因素 DuPont 中，将 Net Profit Margin 进一步拆分为 Tax Burden、Interest Burden 和 EBIT Margin：

$
\boxed{
\text{ROE}=
\text{Tax Burden}\times
\text{Interest Burden}\times
\text{EBIT Margin}\times
\text{Asset Turnover}\times
\text{Equity Multiplier}
}
$

| 因素 | 英文全称 | 定义 | 经济含义 |
|---|---|---|---|
| TB | Tax Burden（税收负担系数） | NI / EBT | 税前利润最终留下多少净利润 |
| IB | Interest Burden（利息负担系数） | EBT / EBIT | 利息等融资成本后的利润保留比例 |
| EBIT Margin | EBIT Margin（息税前利润率） | EBIT / Revenue | 每单位收入带来多少息税前利润 |
| AT | Asset Turnover（资产周转率） | Revenue / Average Assets | 平均资产创造收入的效率 |
| EM | Equity Multiplier（权益乘数） | Average Assets / Average Equity | 财务杠杆程度 |

**术语：** NI = Net Income（净利润）；EBT = Earnings Before Taxes（税前利润）；EBIT = Earnings Before Interest and Taxes（息税前利润）；Revenue = 营业收入。

#### 为什么第三项必须是 EBIT Margin？

$
\begin{aligned}
\text{ROE}
={}&\frac{\text{NI}}{\text{EBT}}
\times\frac{\text{EBT}}{\text{EBIT}}
\times\frac{\text{EBIT}}{\text{Revenue}}\\
&\times\frac{\text{Revenue}}{\text{Average Assets}}
\times\frac{\text{Average Assets}}{\text{Average Equity}}\\
={}&\frac{\text{NI}}{\text{Average Equity}}
\end{aligned}
$

EBT、EBIT、Revenue、Average Assets 顺次约掉，最后留下 ROE 的定义式。

**易错点：** 若保留 Tax Burden 与 Interest Burden，却把第三项错写成 EBT Margin（EBT / Revenue），EBIT 就不能正确约分，五因素恒等式不再成立。

上述拆分在 EBT、EBIT 等分母有意义且口径一致时适用；出现零值或特殊损益分类时需谨慎解读比率。

## 五、偿债能力与杠杆（Solvency & Leverage）

### 1. 资产负债率（Debt Ratio）

$$
\text{Debt Ratio}=\frac{\text{Total Liabilities}}{\text{Total Assets}}
$$

衡量资产中有多少由负债融资；分子是 Total Liabilities，不限于有息债务。

### 2. 债务权益比（Debt-to-Equity Ratio）

$$
\text{Debt-to-Equity}=\frac{\text{Total Debt}}{\text{Total Equity}}
$$

衡量有息债务与股东权益的比例。请区分 **Total Debt（通常指有息债务）** 和 **Total Liabilities（总负债）**，以题目定义为准。

### 3. 债务资本比率（Debt-to-Capital Ratio）

$$
\text{Debt-to-Capital}=
\frac{\text{Total Debt}}{\text{Total Debt}+\text{Total Equity}}
$$

衡量资本结构中债务融资所占比例；和 Debt-to-Equity 的分母不同。

### 4. 利息保障倍数（Interest Coverage）

$$
\text{Interest Coverage}=\frac{\text{EBIT}}{\text{Interest Expense}}
$$

EBIT = Earnings Before Interest and Taxes（息税前利润）。反映经营收益覆盖利息费用的程度。

### 5. 固定支出覆盖率（Fixed Charge Coverage Ratio, FCC）

该指标衡量企业通过经营收益覆盖 **Interest（利息）及 Lease Payments（租赁付款等固定支出）** 的能力。CFA 常见的传统简化形式是：

$
\boxed{
\text{FCC}=
\frac{\text{EBIT}+\text{Lease Payments}}
{\text{Interest Expense}+\text{Lease Payments}}
}
$

- EBIT：Earnings Before Interest and Taxes（息税前利润）。
- Interest Expense：利息费用。
- Lease Payments：租赁付款额，简化公式通常假定相关租赁费用已从 EBIT 中扣除，因而先加回。

**为什么分子加回租赁费用？** 为了计算在支付利息和租赁支出前可用于覆盖固定支出的收益；分母则表示需要覆盖的固定支出规模。

**例子：** EBIT = 500，利息费用 = 100，租赁付款 = 50，则：

$
\text{FCC}=\frac{500+50}{100+50}\approx3.67
$

意味着收益约可覆盖相关固定支出的 3.67 倍。比率越高通常表示覆盖能力越强，但不是现金流量的直接度量。

**会计准则提醒：** 该公式是传统简化口径。IFRS 16 与 US GAAP ASC 842 下租赁费用与利息可能被不同方式列报，计算时应按题目给定的费用口径调整，避免重复加回或重复计入。

#### 与其他指标的区别

| 指标 | 主要衡量 |
|---|---|
| ROE（股东权益回报率） | 股东权益产生利润的能力 |
| EBIT Margin（息税前利润率） | 收入转化为息税前利润的比例 |
| Interest Coverage（利息保障倍数） | 盈利对利息费用的覆盖 |
| Fixed Charge Coverage（固定支出覆盖率） | 盈利对利息及租赁等固定支出的覆盖 |

## 六、经营效率（Activity Ratios）

### 1. 存货周转率（Inventory Turnover）

$$
\text{Inventory Turnover}=\frac{\text{COGS}}{\text{Average Inventory}}
$$

衡量存货成本一年内周转多少次；分子使用 COGS，非 Revenue。

### 2. 应收账款周转率（Receivables Turnover）

$$
\text{Receivables Turnover}=
\frac{\text{Net Credit Sales}}{\text{Average Receivables}}
$$

衡量应收款回收效率。若未提供赊销收入，某些题目以 Revenue 近似，注意题目口径。

## 七、每股收益（Earnings Per Share, EPS）

### 基本每股收益（Basic EPS）

$$
\text{Basic EPS}=
\frac{\text{Net Income}-\text{Preferred Dividends}}
{\text{Weighted Average Common Shares Outstanding}}
$$

先扣除属于优先股股东的股息，再用发行在外普通股加权平均股数相除。Diluted EPS（稀释每股收益）的 If-converted / Treasury Stock Method 见 [[Earnings-Per-Share-EPS]]。

## 八、现金流与自由现金流（Cash Flows）

### 1. 企业自由现金流（FCFF）

$$
\text{FCFF}=
\text{NI}+\text{NCC}+\text{Interest}(1-T)
-\text{FCInv}-\text{WCInv}
$$

- NI：Net Income（净利润）。
- NCC：Non-cash Charges（非现金费用）。
- FCInv：Fixed Capital Investment（固定资本投资）。
- WCInv：Working Capital Investment（非现金营运资本投入）。
- T：所得税率。
- Interest(1−T)：税后利息，转回提供给债权人的税后融资成本。

### 2. 股权自由现金流（FCFE）

$$
\text{FCFE}=\text{NI}+\text{NCC}-\text{FCInv}-\text{WCInv}+\text{Net Borrowing}
$$

Net Borrowing = 净借款（新增债务减偿还本金）。两个公式是常见简化形式，实际现金流分类及其他调整见 [[FCFF-and-FCFE]]。

## 九、递延所得税（Deferred Taxes）

### 1. 递延所得税资产（DTA）与负债（DTL）

$$
\text{DTA}=\text{Deductible Temporary Difference}\times\text{Applicable Tax Rate}
$$

$$
\text{DTL}=\text{Taxable Temporary Difference}\times\text{Applicable Tax Rate}
$$

- DTA：未来可获得的税收利益；通常是“会计先确认费用，税法以后扣除”。
- DTL：未来额外税负；通常是“税法先扣除费用，会计以后确认”。

### 2. 有效税率（Effective Tax Rate）

$$
\text{ETR}=\frac{\text{Income Tax Expense}}{\text{Pretax Income}}
$$

分子是利润表所得税费用，不一定等于现金实缴税额。

### 3. DTA 估值备抵（Valuation Allowance）

$$
\text{Net DTA}=\text{Gross DTA}-\text{Valuation Allowance}
$$

US GAAP 下估值备抵增加通常减少 Net DTA，若相关变动计入损益则增加所得税费用。详情见 [[Deferred-Income-Taxes]]。

## 十、长期资产、债券和养老金

### 1. 无形资产 / 固定资产简化账面价值

$$
\text{Carrying Amount}=
\text{Cost}-\text{Accumulated Depreciation or Amortization}
-\text{Accumulated Impairment}
$$

成本模型下适用；重估模型有不同基准。

### 2. 债券实际利率法（Effective Interest Method）

$$
\text{Interest Expense}=
\text{Beginning Carrying Value}\times\text{Effective Interest Rate}
$$

$$
\text{Ending Carrying Value}=
\text{Beginning Carrying Value}
+\text{Interest Expense}-\text{Coupon Payment}
$$

适用于发行人债券负债按摊余成本核算的常见情形。见 [[07-Fixed-Income/Bond-Premium-and-Discount-Amortization]]。

### 3. 养老金净头寸（Net Pension Position）

$$
\text{Net Pension Position}=
\text{Defined Benefit Obligation (DBO)}
-\text{Fair Value of Plan Assets}
$$

正数为净设定受益负债；负数表示计划盈余，但确认净资产还受 Asset Ceiling（资产上限）限制。见 [[Defined-Benefit-Pension-Net-Position]]。

## 十一、FSA 公式做题通用检查

1. **分子分母单位统一**：百万元与千元不能混用。
2. **流量 / 存量分清**：利润、收入是期间数据；资产、权益是时点余额，ROE、ROA、周转率通常用平均余额。
3. **比例 / 倍数分清**：0.54 次可写成 54%，但应理解为周转效率，不是利润率。
4. **税率与口径核对**：DTA / DTL 按预计转回税率；ROA、债务比率等可能有题目指定口径。
5. **不用死记变形**：优先理解三因素杜邦恒等式，未知变量可用简单代数反推。
