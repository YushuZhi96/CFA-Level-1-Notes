---
subject: Financial Statement Analysis
topic: Common-Size Statements and Financial Ratios
status: "🟡 解析能懂，待独立验证"
created: 2026-11-02
last-reviewed:
tags: [CFA-L1, FSA, Common-Size, Financial-Ratios]
---

# 共同比财务报表与财务比率分析（Common-Size Statements & Financial Ratio Analysis）

## 一句话理解
**共同比财务报表（Common-Size Financial Statements）**把报表项目转换为统一基准的百分比，便于比较规模不同的企业或同一企业不同时期的结构变化；**财务比率分析（Financial Ratio Analysis）**则把相关财务项目建立比率关系，用于分析流动性、偿债能力、盈利能力和经营效率等。

> 术语提醒：Common-size 通常译为“共同比”或“百分比报表”，不要与“同比增长（year-over-year growth）”混淆。

## 一、共同比财务报表（Common-Size Financial Statements）

### 1. 共同比利润表（Common-Size Income Statement）

将利润表每一个项目表示为营业收入（Revenue / Sales）的百分比：

$$
Common\text{-}size\ percentage
=\frac{Income\ Statement\ Item}{Revenue}\times 100\%
$$

因此，Revenue = 100%。

例：Revenue = 500，COGS = 300，Net Income = 50：

- COGS / Revenue = 300 / 500 = 60%
- Net Income / Revenue = 50 / 500 = 10%

**分母不是 Net Income（净利润）**。本次题目选项 A 将分母写成 Net Income，因此错误。

### 2. 共同比资产负债表（Common-Size Balance Sheet）

将资产负债表各项目表示为总资产（Total Assets）的百分比：

$$
Common\text{-}size\ percentage
=\frac{Balance\ Sheet\ Item}{Total\ Assets}\times 100\%
$$

因此，Total Assets = 100%。

例：Inventory = 20，Total Assets = 200，则 Inventory / Total Assets = 10%。

### 3. 两种报表的基准对照

| 报表 | 共同基准 | 基准占比 |
|---|---|---:|
| Income Statement（利润表） | Revenue / Sales（营业收入） | 100% |
| Balance Sheet（资产负债表） | Total Assets（总资产） | 100% |

共同比分析属于纵向分析（Vertical Analysis）：关注每个项目在同一张报表中的构成比例。

## 二、共同比报表的两种比较用途

### 1. 时间序列分析（Time-Series Analysis）
比较**同一家企业在不同期间**的共同比数据，观察结构和趋势变化。

例：某公司 COGS / Revenue 从 55% 上升到 60%，再升至 65%。这提示成本占收入比例上升，可能挤压毛利率；仍需进一步调查原因。

记忆：Same company, different periods（同一公司，不同期间）。

### 2. 横截面分析（Cross-Sectional Analysis）
比较**不同企业在同一期间**的共同比数据。转换为百分比有助于减弱企业规模差异的影响。

例：同一年度 A、B 两家公司的 Net Income / Revenue 分别为 20% 和 10%，可比较其净利率表现。

记忆：Different companies, same period（不同公司，同一期间）。

### 3. 局限
共同比分析让比较更方便，但不能自动消除会计政策、业务模式、会计估计、季节性等差异。比较时仍要确认口径一致，并结合附注理解数据。

## 三、财务比率分析（Financial Ratio Analysis）

财务比率把报表中的项目联系起来，帮助回答不同问题。常见分类如下。

### 1. 流动性（Liquidity）
衡量企业偿还短期义务的能力。

**营运资本（Working Capital）**

$$
Working\ Capital = Current\ Assets - Current\ Liabilities
$$

**流动比率（Current Ratio）**

$$
Current\ Ratio = \frac{Current\ Assets}{Current\ Liabilities}
$$

**速动比率（Quick Ratio）**

$$
Quick\ Ratio =
\frac{Cash + Short\text{-}term\ Marketable\ Securities + Receivables}{Current\ Liabilities}
$$

也常按题目口径写作：

$$
Quick\ Ratio =
\frac{Current\ Assets - Inventory - Prepaids}{Current\ Liabilities}
$$

速动比率比流动比率更严格，通常剔除存货和预付费用等较难迅速用于偿债的项目。

### 2. 偿债能力 / 杠杆（Solvency / Leverage）
衡量企业长期偿债压力及资本结构。

**负债比率（Debt Ratio）**

$$
Debt\ Ratio = \frac{Total\ Liabilities}{Total\ Assets}
$$

**债务权益比（Debt-to-Equity Ratio）**

$$
Debt\text{-}to\text{-}Equity =
\frac{Total\ Debt}{Total\ Equity}
$$

**利息保障倍数（Interest Coverage）**

$$
Interest\ Coverage = \frac{EBIT}{Interest\ Expense}
$$

注意 Debt Ratio 与 Debt-to-Equity Ratio 的分母不同，不要混淆。

### 3. 盈利能力（Profitability）
衡量企业赚取利润的能力。

**毛利率（Gross Profit Margin）**

$$
Gross\ Profit\ Margin = \frac{Gross\ Profit}{Revenue}
$$

**营业利润率（Operating Profit Margin）**

$$
Operating\ Profit\ Margin = \frac{Operating\ Income}{Revenue}
$$

**净利率（Net Profit Margin）**

$$
Net\ Profit\ Margin = \frac{Net\ Income}{Revenue}
$$

**资产回报率（Return on Assets, ROA）**

$$
ROA = \frac{Net\ Income}{Average\ Total\ Assets}
$$

**股东权益回报率（Return on Equity, ROE）**

$$
ROE = \frac{Net\ Income}{Average\ Shareholders'\ Equity}
$$

### 4. 经营效率 / 活动能力（Activity / Efficiency）
衡量企业使用资产创造收入或管理营运资本的效率。

**存货周转率（Inventory Turnover）**

$$
Inventory\ Turnover = \frac{COGS}{Average\ Inventory}
$$

**应收账款周转率（Receivables Turnover）**

$$
Receivables\ Turnover =
\frac{Net\ Credit\ Sales}{Average\ Receivables}
$$

若题目未提供赊销额，可能按题目给定口径使用 Revenue。

**总资产周转率（Total Asset Turnover）**

$$
Total\ Asset\ Turnover =
\frac{Revenue}{Average\ Total\ Assets}
$$

周转率通常是“期间流量 ÷ 平均时点余额”。因此在可获得数据时，常使用平均资产、平均存货或平均应收账款，而不是只取期末余额。

## 四、共同比分析与比率分析的区别

| 对比 | Common-Size Analysis | Ratio Analysis |
|---|---|---|
| 核心方法 | 每个项目 ÷ 统一基准 | 两个或多个财务项目建立比率 |
| 主要目的 | 看报表结构、构成比例 | 看流动性、盈利能力、杠杆、效率 |
| 例子 | COGS / Revenue | Current Assets / Current Liabilities |
| 常见用途 | 时间序列、横截面比较 | 企业诊断、同业比较、趋势分析 |

两者可以结合使用：先通过共同比报表发现成本结构或资产结构异常，再用具体财务比率深入分析。

## 五、常见考试陷阱

1. 共同比利润表的基准是 **Revenue（营业收入）**，不是 Net Income（净利润）。
2. 共同比资产负债表的基准是 **Total Assets（总资产）**。
3. Time-series = 同一公司、不同时期；Cross-sectional = 不同公司、同一时期。
4. Common-size 不等于同比增长率（Year-over-Year Growth）。
5. 共同比分析减弱规模差异，但不能消除会计政策和业务模式差异。
6. 流动比率分子为 Current Assets；速动比率通常剔除 Inventory 和 Prepaids。
7. Debt Ratio = Total Liabilities / Total Assets；Debt-to-Equity = Total Debt / Total Equity，口径不同。
8. 周转率及 ROA、ROE 常使用平均余额，因为分子是期间数据、分母是时点数据。

## 六、本次题目记录

题目问哪项表述最不准确。正确答案 A。错误点：将共同比利润表的基准误写成 Net Income；正确基准应为 Revenue。

- [x] 能说出共同比利润表和资产负债表各自的分母
- [x] 能区分 Time-Series 与 Cross-Sectional Analysis
- [ ] 能独立计算常见流动性、偿债能力和盈利能力比率
- [ ] 能解释平均余额在周转率及回报率计算中的作用
- [ ] 能独立完成一道同类新题


## 七、共同比现金流量表（Common-Size Cash Flow Statement）

与共同比利润表（Revenue 为基准）和共同比资产负债表（Total Assets 为基准）相比，现金流量表可根据分析目的使用两种常见标准化方法。

### 方法一：各现金流项目除以营业收入（Revenue）

$$
Common\text{-}Size\ Cash\ Flow\ Percentage
=\frac{Cash\ Flow\ Item}{Revenue}\times100\%
$$

例如 Revenue = 1,000，CFO = 200，则 CFO / Revenue = 20%。这种方法适合跨期或跨公司衡量现金流相对于收入的规模。

### 方法二：现金流入和流出分别以各自总额为基准

现金流入项目：

$$
Cash\ Inflow\ Percentage
=\frac{Individual\ Cash\ Inflow}{Total\ Cash\ Inflows}\times100\%
$$

现金流出项目：

$$
Cash\ Outflow\ Percentage
=\frac{Individual\ Cash\ Outflow}{Total\ Cash\ Outflows}\times100\%
$$

例：客户收款 600、债务融资流入 400，则现金流入总额 1,000，客户收款占 60%；支付供应商 500、购买设备 300，则现金流出总额 800，供应商付款占 62.5%。

### 必须区分三个概念

| 英文 | 中文 | 含义 |
|---|---|---|
| Total Cash / Cash Balance | 现金余额 | 某一时点持有的现金存量 |
| Total Cash Inflows | 现金流入总额 | 一段期间所有现金流入之和 |
| Total Cash Outflows | 现金流出总额 | 一段期间所有现金流出金额之和 |
| Net Cash Flow | 现金净流量 | 现金流入减现金流出 |

**本题易错点：**“Divide each item by total cash”并非通常的共同比现金流量表编制方法，因为期末现金余额是时点存量，与当期总现金流入不同。现金净流量也不宜机械作为统一分母，可能为零或极小。

**判断要点：**
- 按 Revenue 标准化：合理。
- 流入除以 Total Cash Inflows、流出除以 Total Cash Outflows：合理。
- 所有项目统一除以 Total Cash Balance：不是本题所指的常规共同比分析方法。

特殊现金比率分析也可能采用现金余额作为分母，但这不等于标准的共同比现金流量表。


## 八、三项核心财务比率：Quick Ratio、EBIT Margin、Current Ratio

### 1. Quick Ratio（速动比率）

$$
\boxed{Quick\ Ratio=\frac{Quick\ Assets}{Current\ Liabilities}}
$$

常见展开式：

$$
Quick\ Ratio=\frac{Cash+Marketable\ Securities+Receivables}{Current\ Liabilities}
$$

或按题目给定科目口径：

$$
Quick\ Ratio=\frac{Current\ Assets-Inventory-Prepaid\ Expenses}{Current\ Liabilities}
$$

- **Quick Assets（速动资产）**：通常包括现金、短期有价证券、应收款等。
- **Current Liabilities（流动负债）**：通常需在营业周期内或短期内清偿的负债。
- **作用**：衡量不依赖出售存货等流动性较弱资产的短期偿债能力。
- **关键**：Inventory（存货）不计入速动比率分子。

### 2. EBIT Margin（息税前利润率）

$$
\boxed{EBIT\ Margin=\frac{EBIT}{Revenue}\times100\%}
$$

$$
EBIT=Earnings\ Before\ Interest\ and\ Taxes
$$

简化经营情形：

$$
EBIT=Revenue-COGS-Other\ Operating\ Expenses
$$

- **Revenue（营业收入）**：公司销售商品或提供服务产生的收入。
- **COGS（销售成本）**：已销售商品计入当期的成本。
- **作用**：衡量每单位收入对应多少息税前利润。
- **关键**：在收入与其他费用不变时，COGS 下降会使 EBIT 及 EBIT Margin 上升。

### 3. Current Ratio（流动比率）

$$
\boxed{Current\ Ratio=\frac{Current\ Assets}{Current\ Liabilities}}
$$

- **Current Assets（流动资产）**：包括现金、应收账款、存货、预付费用等。
- **作用**：衡量流动资产覆盖流动负债的程度。
- **关键**：与 Quick Ratio 不同，Current Ratio 的分子**包含 Inventory**。

### 三个指标的比较

| 指标 | 分子 | 分母 | 是否直接包含存货 |
|---|---|---|---|
| Quick Ratio | Quick Assets | Current Liabilities | 否 |
| EBIT Margin | EBIT | Revenue | 存货计价通过 COGS 间接影响 EBIT |
| Current Ratio | Current Assets | Current Liabilities | 是 |

### 与 FIFO/LIFO 的联系（简化情形）

如果使用 FIFO 相比 LIFO 使期末存货账面价值增加：
- **Current Ratio**：通常提高，因为 Inventory 计入流动资产。
- **Quick Ratio**：不会因为 Inventory 增加而直接提高；若考虑历史上已实际支付的额外所得税，现金可能减少，从而使速动比率下降。
- **EBIT Margin**：若 FIFO 使当期 COGS 降低，EBIT Margin 提高。

注意：涉及税额、现金或递延所得税负债时，须区分“实际使用 FIFO 所产生的现金税影响”和“分析师将 LIFO 报表重列为 FIFO 的非现金调整”，不可无条件认为 Cash 必然下降。

关联：[[Inventory-Cost-Flow-Methods|FIFO、LIFO 与 WAC 存货计价方法]]。

### 自测
- [ ] 能默写三个比率公式
- [ ] 能说出 Quick Ratio 与 Current Ratio 在 Inventory 上的区别
- [ ] 能说明 COGS 对 EBIT Margin 的作用
