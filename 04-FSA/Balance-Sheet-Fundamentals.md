---
subject: Financial Statement Analysis
topic: Balance Sheet Fundamentals
status: "🟡 解析能懂，待独立验证"
created: 2026-11-02
last-reviewed:
tags: [CFA-L1, FSA, Balance-Sheet]
---

# 资产负债表（Balance Sheet）

## 一句话理解
资产负债表是在**某一个特定时点（at a specific point in time）**，展示企业控制的经济资源、承担的现时义务，以及归属于股东的剩余权益。

它回答三个问题：
1. 公司拥有什么资源？
2. 公司对外承担多少义务？
3. 扣除负债后，剩余多少权益归属于股东？

## 核心概念 / 定义

### 1. 会计恒等式（Accounting Equation）

$$
\boxed{Assets = Liabilities + Shareholders'\ Equity}
$$

即：

$$
资产 = 负债 + 股东权益
$$

- **Assets（资产）**：企业控制的、预期能够带来未来经济利益的资源。
- **Liabilities（负债）**：企业因过去事项形成的现时义务，清偿时通常需要转移经济资源。
- **Shareholders' Equity（股东权益）**：扣除全部负债后，归属于股东的剩余权益。

因此：

$$
Equity = Assets - Liabilities
$$

资产的资金来源可理解为两部分：债权人提供的资金（Liabilities）与股东提供并留存在企业的权益资金（Equity）。

### 2. 资产 Assets

常见项目：

| 项目 | 英文 | 含义 |
|---|---|---|
| 现金及现金等价物 | Cash and Cash Equivalents | 可立即使用或高度流动的资金 |
| 应收账款 | Accounts Receivable | 客户已欠付、企业有权收取的款项 |
| 存货 | Inventory | 待出售或用于生产的材料、在产品和商品 |
| 固定资产 | Property, Plant and Equipment (PP&E) | 用于经营的厂房、机器、设备等有形长期资产 |
| 无形资产 | Intangible Assets | 专利、商标、软件等可辨认或其他符合确认条件的无形资源 |
| 长期投资 | Long-term Investments | 预计长期持有的投资 |

### 3. 负债 Liabilities

常见项目：

| 项目 | 英文 | 含义 |
|---|---|---|
| 应付账款 | Accounts Payable | 企业因采购商品或服务而欠供应商的款项 |
| 短期借款 | Short-term Debt | 近期需要偿还的借款 |
| 应付工资 | Wages Payable | 已发生但尚未支付的工资 |
| 应付利息 | Interest Payable | 已发生但尚未支付的利息 |
| 长期借款 | Long-term Debt | 非流动的借款义务 |
| 租赁负债 | Lease Liabilities | 因租赁安排确认的付款义务 |

### 4. 股东权益 Shareholders' Equity

股东权益（Shareholders' Equity / Owners' Equity）是企业资产扣除全部负债后的**剩余权益（Residual Interest）**：

$$
Shareholders'\ Equity = Total\ Assets - Total\ Liabilities
$$

它不是“公司账户里剩余的现金”，也不等于公司股票的市场价值（Market Capitalization）。它是资产负债表上的会计账面权益（Book Equity）。

#### 4.1 股东权益的主要组成

不同国家、公司类型和会计准则下，报表列示名称可能不同。CFA 常见项目可按以下结构理解：

| 组成 | 英文 | 正常方向 | 核心含义 |
|---|---|---:|---|
| 普通股股本 | Common Stock / Ordinary Share Capital | 增加权益 | 按面值或法定 / 列报金额确认的已发行普通股资本 |
| 资本公积 / 额外实收资本 | Additional Paid-in Capital (APIC) / Share Premium | 增加权益 | 股东投入超过股票面值的部分及符合规定的其他资本投入 |
| 留存收益 | Retained Earnings | 可正可负 | 累计利润扣除股利及相关调整后的留存金额 |
| 累计其他综合收益 | Accumulated Other Comprehensive Income (AOCI) | 可正可负 | 以前期间和本期计入 OCI、累计留在权益中的金额 |
| 库存股 | Treasury Stock | **抵减权益** | 公司回购的自身股份，通常以负数列示 |

此外，报表还可能出现优先股（Preferred Stock）、股份支付储备（Share-based Payment Reserve）、重估盈余（Revaluation Surplus）等项目。合并财务报表还可能单独列示非控制性权益（Non-controlling Interest, NCI）。

#### 4.2 普通股股本与资本公积：股东投入的资本

**Common Stock（普通股股本）**
- 代表公司发行普通股所确认的股本金额，通常按股票面值（Par Value）或适用法律规定的列报金额记录。
- 它不是股票当前市场价格，也不等于公司收到的全部发行款。

**Additional Paid-in Capital, APIC（额外实收资本 / 资本公积）**
- 股东发行认购价超过股票面值的部分，通常计入 APIC；IFRS 报表常见名称为 Share Premium（股本溢价）。
- APIC 还可能包含其他符合准则的资本性投入或权益交易金额，具体看当地准则和报表列示。

例：公司发行 100,000 股普通股，每股面值 $1，发行价 $10：

$$
Cash\ Received=100,000\times10=\$1,000,000
$$

$$
Common\ Stock=100,000\times1=\$100,000
$$

$$
APIC=100,000\times(10-1)=\$900,000
$$

简化分录：

| 科目 | Debit 借方 | Credit 贷方 |
|---|---:|---:|
| Cash（现金） | $1,000,000 | |
| Common Stock（普通股股本） | | $100,000 |
| APIC（资本公积） | | $900,000 |

**考试重点：** 股东投入公司是权益融资（Equity Financing），不是营业收入（Revenue），因此不会因为发行股票而直接增加当期净利润（Net Income）。

#### 4.3 留存收益 Retained Earnings：公司赚取并留存的累计利润

留存收益是企业历年累计净利润中没有通过股利等方式分配出去、并经相关调整后的金额。

简化变动公式：

$$
Ending\ Retained\ Earnings
=Beginning\ Retained\ Earnings
+Net\ Income
-Dividends
$$

若当期发生净亏损（Net Loss），应以负数影响留存收益。实际报表还可能涉及前期差错更正、会计政策变更的追溯调整及其他准则规定的项目。

例：
- 期初留存收益：$200,000
- 本期净利润：$80,000
- 本期宣告股利：$30,000

$$
Ending\ RE=200,000+80,000-30,000=\$250,000
$$

注意：
- **Net Income（净利润）**先在利润表计算，期末结转后通常增加 Retained Earnings。
- **Dividends（股利）**是利润分配，不是利润表费用；宣告股利会减少留存收益并通常确认应付股利，支付时减少现金和应付股利。
- 留存收益不代表公司持有同等金额的现金；利润可能已用于购买设备、存货或偿还债务。

#### 4.4 累计其他综合收益 AOCI

**Other Comprehensive Income (OCI，其他综合收益)** 是按适用准则不直接计入当期净利润、而列入其他综合收益的特定收益和损失。

**Accumulated Other Comprehensive Income (AOCI，累计其他综合收益)** 是这些 OCI 项目在权益中累计形成的余额。

可能涉及的项目（取决于准则和具体分类）：
- 外币报表折算差额（Foreign Currency Translation Differences）；
- 某些金融资产的公允价值变动；
- 现金流量套期储备（Cash Flow Hedge Reserve）；
- 某些设定受益计划的重新计量（Remeasurements of Defined Benefit Plans）。

关系：

$$
Comprehensive\ Income=Net\ Income+OCI
$$

当期 OCI 会影响综合收益，并在适用情况下累计进入 AOCI；它不等于 Investment Income（投资收益），也不一定会在未来重分类进损益，具体取决于项目和会计准则。

#### 4.5 库存股 Treasury Stock：股东权益的抵减项

Treasury Stock 是公司已经回购、但尚未注销的自身股份。

- 通常作为股东权益的抵减项（Contra-equity），在权益部分以负数列示。
- 回购自身股份通常减少现金（Assets）和股东权益（Equity）。
- 库存股通常不享有股息分配权和表决权（具体法律安排除外）。
- 回购、再发行自身股份产生的差额通常作为权益内部项目处理，而不是确认普通经营收入或费用；应按适用准则判断。

例：公司用 $50,000 现金回购自身股份：

- Cash 减少 $50,000；
- Treasury Stock（抵减权益）增加 $50,000；
- 总股东权益减少 $50,000；
- 不因此确认经营费用。

#### 4.6 非控制性权益 NCI（合并报表补充）

**Non-controlling Interest (NCI，非控制性权益)** 是子公司权益中不归属于母公司股东的部分。

在合并资产负债表中，NCI 通常作为股东权益的一部分单独列示，但它不属于母公司股东应占权益（Equity Attributable to Owners of the Parent）。

#### 4.7 股东权益结构示例

假设某公司资产负债表列示：

| 项目 | 金额 |
|---|---:|
| Common Stock（普通股股本） | $100 |
| APIC（资本公积） | $400 |
| Retained Earnings（留存收益） | $250 |
| AOCI（累计其他综合收益） | $30 |
| Treasury Stock（库存股） | ($50) |
| **Total Shareholders' Equity（股东权益合计）** | **$730** |

计算：

$$
100+400+250+30-50=730
$$

这张表帮助记忆：股东投入、累计留存利润和累计 OCI 增加权益；库存股通常抵减权益。

#### 4.8 本题易错点：Investment Income 不等于 Equity Account

**Investment Income（投资收益）**通常是利润表（Income Statement）中的收益 / 利得项目，而不是资产负债表中直接列示的股东权益组成科目。

但它可能通过以下路径间接影响股东权益：

$$
Investment\ Income
\rightarrow Net\ Income
\rightarrow Retained\ Earnings
\rightarrow Shareholders'\ Equity
$$

因此：
- Paid-In Capital（投入资本）是股东权益组成；
- Retained Earnings（留存收益）是股东权益组成；
- Investment Income（投资收益）是利润表项目，确认后通过净利润结转影响留存收益。

**本题问“哪个科目最不可能属于 Owners' Equity”，正确答案是 B：Investment Income。**
## 资产与负债的分类

### 1. 流动资产 Current Assets
通常在正常营业周期内，或资产负债表日后 12 个月内，预期能够变现、出售或耗用的资产；现金及现金等价物等也按相关准则分类。

常见：Cash、Accounts Receivable、Inventory、Short-term Investments。

### 2. 非流动资产 Non-current Assets
不符合流动资产分类条件的长期资源。

常见：PP&E、Intangible Assets、Long-term Investments。

### 3. 流动负债 Current Liabilities
通常在正常营业周期内，或资产负债表日后 12 个月内需要清偿的义务；还需结合企业是否有权将清偿递延至少 12 个月等准则条件判断。

常见：Accounts Payable、Short-term Debt、Wages Payable。

### 4. 非流动负债 Non-current Liabilities
不符合流动负债分类条件的长期义务。

常见：Long-term Debt、Long-term Bonds、长期租赁负债。

> 注意：流动 / 非流动分类不能只机械看名称。应结合正常营业周期、报告日后 12 个月及适用会计准则判断；某些企业的正常营业周期可能超过 12 个月。

## 公式与变量

### 会计恒等式
$$
Assets = Liabilities + Equity
$$

### 营运资本（Working Capital）
$$
Working\ Capital = Current\ Assets - Current\ Liabilities
$$

### 流动比率（Current Ratio）
$$
Current\ Ratio = \frac{Current\ Assets}{Current\ Liabilities}
$$

衡量流动资产覆盖流动负债的程度。

### 速动比率（Quick Ratio）
常见定义之一：

$$
Quick\ Ratio = \frac{Cash + Short\text{-}term\ Marketable\ Securities + Receivables}{Current\ Liabilities}
$$

也可写为：

$$
Quick\ Ratio = \frac{Current\ Assets - Inventory - Prepaids}{Current\ Liabilities}
$$

具体口径应以题目给定定义为准。

### 负债比率（Debt Ratio）
$$
Debt\ Ratio = \frac{Total\ Liabilities}{Total\ Assets}
$$

衡量资产中由负债融资的比例。不要与 Debt-to-Equity Ratio（债务权益比）混淆。

## 直观理解 / 记忆方法

- **Balance Sheet = Snapshot（快照）**：展示某一个日期的财务状况。
- **Income Statement（利润表）= Period Performance（期间经营成果）**：展示一段期间的收入、费用和利润。
- **Cash Flow Statement（现金流量表）= Period Cash Movements（期间现金流动）**：展示一段期间现金及现金等价物的流入和流出。

例：公司在 2026 年 12 月 31 日的资产负债表，描述的是这一天的财务状况；2026 年全年利润则由 2026 年度利润表反映。

## 三大报表之间的联系（Linkages）

- 利润表的 **Net Income（净利润）** 通常会进入留存收益的变动计算。
- 现金流量表解释一段期间现金及现金等价物余额为什么发生变化。
- 资产负债表展示报告期末的 Cash、Receivables、Inventory、Debt、Equity 等余额。
- 三大报表需结合阅读，不能仅凭净利润判断现金状况，也不能仅凭资产总额判断偿债能力。

## 常见考试陷阱

1. **时点 vs 期间**：Balance Sheet 是某一时点（point in time）；Income Statement 和 Cash Flow Statement 是一段期间（over a period）。
2. **Accounts Receivable vs Accounts Payable**：应收账款是资产；应付账款是负债。
3. **Profitability vs Financial Position**：盈利能力主要通过利润表分析；资产负债表反映财务状况（financial position）。
4. **Equity 不等于 Market Value**：资产负债表中的股东权益是会计账面金额（book value），不等同于公司股票市值或股东权益市场价值。
5. **Current 不等于“只剩 12 个月”**：正常营业周期也会影响流动 / 非流动分类。
6. **流动资产多不必然代表偿债能力强**：还要检查存货能否出售、应收账款能否收回以及现金是否受限。

## 典型题型 / 判断路径

题目问 Balance Sheet 的功能：
- 出现 **specific point in time / financial position / assets / liabilities / equity**：通常属于资产负债表。
- 出现 **revenues / expenses / profitability / net income over a period**：通常属于利润表。
- 出现 **cash inflows / cash outflows / operating, investing, financing activities**：通常属于现金流量表。

## 易混知识点 / Obsidian 链接

- [[Income-Statement-Fundamentals|利润表基础概念]]
- [[Cash-Flow-Statement-Fundamentals|现金流量表基础概念]]
- [[Financial-Ratio-Analysis|财务比率分析]]


## 股东投入资本、债务融资与经营收入的区别

### 1. 发行普通股（Issuance of Common Stock）

股东认购公司新发行的普通股，向公司投入现金。这属于**权益融资（Equity Financing）**，不是公司通过经营活动赚取的收入。

简化会计分录（Journal Entry）：

```text
Dr. Cash（借：现金）                         200,000
    Cr. Common Stock / Additional Paid-in Capital
       （贷：普通股股本 / 资本公积）          200,000
```

影响：
- **Assets（资产）增加**：公司收到现金。
- **Shareholders' Equity（股东权益）增加**：股本及 / 或资本公积增加。
- **Liabilities（负债）不变**：没有产生偿债义务。
- **Income / Net Income（收益 / 净利润）不变**：股东投入资本不是营业收入，也不是利润。

在现金流量表（Cash Flow Statement）中，发行普通股收到的现金通常列入 **Financing Activities（筹资活动现金流入）**。

### 2. 发行债券或取得借款（Debt Financing）

公司发行债券或向银行借款，收到现金，同时承担偿还本金等合同义务。

简化分录：

```text
Dr. Cash（借：现金）             500,000
    Cr. Bonds Payable（贷：应付债券） 500,000
```

影响：
- Assets 增加；
- Liabilities 增加；
- Equity 和发行时的 Income 不因收到本金而直接增加；
- 收到债券或借款资金通常属于筹资活动现金流入。

后续 **Interest Expense（利息费用）** 通常计入利润表，减少税前利润；支付利息的现金流分类需根据适用会计准则及题目口径判断。

### 3. 经营收入（Revenue）与净利润（Net Income）

公司通过销售商品或提供服务赚取收入，才属于经营活动产生的 Revenue。收入扣除相关费用后影响 Net Income，净利润再通过留存收益（Retained Earnings）影响 Equity。

因此要区分：
- **Share issuance proceeds（发行股票收到的资金）**：权益融资，不是收入。
- **Bond proceeds（发行债券收到的资金）**：债务融资，不是收入。
- **Sales revenue（销售收入）**：经营活动收入，影响利润表。

### 4. 股息与利息不要混淆

- **Dividends（股息 / 股利）**：向股东分配利润，不属于利润表费用；宣告或支付股息会减少留存收益 / 股东权益。支付时现金减少。
- **Interest Expense（利息费用）**：债务融资成本，通常计入利润表费用，影响净利润。

### 5. 常见交易对报表项目的影响（简化）

| 交易 | Assets | Liabilities | Equity | Income |
|---|---:|---:|---:|---:|
| 发行普通股并收取现金 | ↑ | — | ↑ | — |
| 发行债券并收取现金 | ↑ | ↑ | — | — |
| 赊销商品并确认收入（暂不考虑成本） | ↑（应收账款） | — | 通过利润增加 | ↑（Revenue） |
| 宣告现金股息 | —（宣告时通常不变） | ↑（应付股息） | ↓ | — |
| 支付已宣告股息 | ↓（现金） | ↓（应付股息） | —（支付时不再重复减少） | — |
| 确认债券利息费用（尚未支付） | — | ↑（应付利息） | 通过净利润减少 | ↓（费用增加） |

注：表格为帮助理解的简化情形，未考虑税项、交易费用、存货成本、减值及其他复杂因素。股息在宣告与支付时点对报表的影响不同。

## 题目归档：新发行普通股收到的资金影响什么？

题意：公司发行新一轮普通股，股东投入资金，问这笔资金最不可能影响哪个项目。

**正确答案：Income（收益 / 收入）**。

判断路径：
1. 股东支付认购款 → 公司 Cash 增加 → Assets 增加。
2. 公司发行普通股 → Common Stock / Additional Paid-in Capital 增加 → Equity 增加。
3. 这是权益融资而非经营活动 → 不确认 Revenue，也不直接增加 Net Income。
4. 因此最不可能受影响的是 Income。

易错点：不要把“公司收到现金”直接等同于“公司赚到收入”。现金流入可能来自经营、投资或筹资活动，只有符合收入确认条件的经营成果才构成 Revenue。

关联概念：[[Income-Statement-Fundamentals|利润表基础概念]]、[[Cash-Flow-Statement-Fundamentals|现金流量表基础概念]]。

## 我的错因 / 验证记录

本次题目：问资产负债表**不具备**哪项功能。正确答案为“展示公司在某一期间的盈利能力”，因为盈利能力属于利润表的分析范围。

- [ ] 不看解析能独立解释资产、负债、股东权益及会计恒等式
- [ ] 能区分 Common Stock、APIC、Retained Earnings、AOCI 和 Treasury Stock
- [ ] 能解释 Investment Income 如何通过 Net Income 间接影响 Retained Earnings
- [ ] 能计算发行股票时 Common Stock 与 APIC 的金额
- [ ] 能解释 Treasury Stock 为什么是抵减权益项目
- [ ] 能区分流动 / 非流动资产与负债
- [ ] 能区分三大报表的时点与期间属性
- [ ] 能独立完成一道同类新题
- [ ] 能区分权益融资、债务融资与经营收入
- [ ] 能判断发行股票、发行债券、股息和利息对三大报表的影响
