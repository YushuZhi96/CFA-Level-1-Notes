---
subject: CFA Level I
topic: Equity Investments Fundamentals
status: 持续更新
tags: [CFA-L1, Equity, Fundamentals]
---

# Equity Investments Basics｜权益投资基础概念

本文件集中整理 CFA 一级权益投资（Equity Investments）章节中的基础概念、重要英文术语及做题判断方法。复杂模型与专项考点另建独立笔记。遇到涉及其他科目的知识点时，标明交叉关系，不按每道题重复建文件。

## 1. Market Participants and Trading Objectives｜市场参与者与交易目的

### Hedger｜套期保值者

- **定义**：已经面临某种价格、利率或汇率等风险的个人或机构，利用金融合约抵消或降低原有风险敞口（Risk Exposure）。
- **目的**：Risk Reduction（降低风险），而非单纯追求价格波动带来的盈利。
- **考试关键词**：Worried about price decrease / increase、Lock in a price、Reduce price risk、Protect against losses。
- **例子**：农民未来需要出售谷物，担心谷物跌价，今天卖出谷物远期合约锁定未来售价，属于 Hedger。
- **注意**：套期保值旨在降低特定风险，也可能放弃有利价格变动带来的额外收益；仍可能存在交易对手风险（Counterparty Risk）、数量或期限不匹配等风险。

### Speculator｜投机者

- **定义**：主动承担市场价格变动的风险，希望通过判断价格方向获得收益的交易者。
- **目的**：Profit from price movements（从价格波动中获利）。
- **例子**：交易者没有谷物现货或未来销售需求，只因预测谷物跌价而卖出谷物远期合约，通常属于 Speculator。
- **区别**：同为卖出远期合约，是否属于 Hedger，要看其是否在抵消**原有风险敞口**。

### Investor｜投资者

- **定义**：投入资金购买证券或其他资产，以获取收益、资本增值或满足投资目标的个人或机构。
- **目的**：Investment Return（投资回报），通常同时考虑风险与流动性。
- **注意**：Investor 与 Hedger 不一定在现实中互斥；投资者也可能进行套期保值。但在题目要求选择 **most appropriate label** 时，应根据案例最直接体现的交易目的选答案。

### Securitizer｜证券化者

- **定义**：参与将贷款、应收款等资产或其现金流汇集、重组，并以此为基础发行或安排发行证券的主体。
- **相关概念**：Securitization（资产证券化）、Asset-Backed Securities (ABS，资产支持证券)。
- **例子**：金融机构将一批住房抵押贷款汇集，形成可向投资者出售的证券。
- **不是套期保值**：证券化关注资产转化和融资结构；农民使用远期合约锁定未来售价不构成证券化。

### 四种角色对照

| 角色 | 英文 | 关键目的 | 判断线索 |
|---|---|---|---|
| 套期保值者 | Hedger | 降低已有风险 | 有现货或未来真实经营需求；锁定价格 |
| 投机者 | Speculator | 承担价格风险博取收益 | 主要根据行情判断建立风险头寸 |
| 投资者 | Investor | 获取投资回报 | 出资买入并持有资产或证券 |
| 证券化者 | Securitizer | 将资产现金流转化为证券 | 资产池、证券发行、现金流重组 |

## 2. Forward Contracts and Hedging｜远期合约与套期保值

### Forward Contract｜远期合约

- **定义**：双方约定在未来特定日期，以约定价格交易特定数量标的资产的合约；通常属于场外交易（Over-the-Counter, OTC）。
- **Forward Price / Delivery Price（远期约定价格）**：合约约定的未来交易价格；本题中是农民希望锁定的谷物售价。
- **Short Forward（卖出远期）**：承诺在未来按合约约定价格卖出标的。
- **Long Forward（买入远期）**：承诺在未来按合约约定价格买入标的。

### Short Hedge｜卖出套期保值

- **适用情形**：未来要卖出现货，担心现货价格下跌。
- **典型主体**：农民、商品生产商等。
- **操作**：卖出对应标的远期合约（Short Forward）以对冲未来现货销售收入下降的风险。

### Long Hedge｜买入套期保值

- **适用情形**：未来要采购标的，担心采购价格上涨。
- **典型主体**：未来需要购买燃油的航空公司。
- **操作**：买入对应标的远期合约（Long Forward）以对冲未来采购成本上升的风险。

| 经营需求 | 担心什么 | 典型操作 | 对冲方向 |
|---|---|---|---|
| 未来卖谷物 | 谷物跌价 | Sell Forward | Short Hedge |
| 未来买燃油 | 燃油涨价 | Buy Forward | Long Hedge |

### 例子：农民为什么属于 Hedger？

假设农民将在三个月后出售 1,000 吨谷物，并签订远期合约，约定每吨 2,000 元卖出。为便于理解，假设标的、数量、日期完全匹配，交易对手正常履约，不计成本。

| 三个月后的市场价 | 没有远期合约的销售收入 | 按远期约定的销售收入 |
|---|---:|---:|
| 1,500 元/吨 | 150 万元 | 200 万元 |
| 2,500 元/吨 | 250 万元 | 200 万元 |

- 价格下跌：远期合约保护农民免于按更低价格出售。
- 价格上涨：农民无法享受市场价上涨的额外收益。
- **核心**：农民为了稳定未来销售收入（减少价格风险），而不是单纯押注谷物价格下跌。

## 3. CFA Exam Traps｜考试陷阱与判断顺序

1. **先看原有风险敞口**：当事人是否已经持有现货，或有真实的未来买卖需求？
2. **再看交易目的**：为了 Lock in a price / Reduce risk，还是为了 Profit from price movements？
3. **最后看工具和方向**：Future sale + short forward；future purchase + long forward。
4. **不要把交易方向当作身份**：卖出远期不一定是投机，买入远期也不一定是投资。
5. **不要把证券化误认成套保**：Securitizer 涉及资产池与证券发行，不是简单的远期买卖。

**典型题识别**：A grain farmer worries about a fall in grain prices and enters a forward contract to sell grain at a predetermined price → **Hedger（套期保值者）**。

**一句话记忆**：Hedger reduces existing risk; Speculator takes risk for potential profit.

## 4. Margin Trading, Leverage and Annualized Return｜融资买入、杠杆与年化收益率

### Margin Trading / Buying on Margin｜融资买入

- **定义**：投资者使用自有资金（Investor's Equity）加上借款（Margin Loan）购买股票。
- **作用**：Leverage（杠杆）可以放大自有资金收益，也会放大自有资金亏损；实际交易还可能涉及融资利息、维持保证金及追加保证金要求（Margin Call）。
- **本题假设**：忽略交易成本、融资借款利息与股息；借款本金在卖出时偿还。

### Leverage Ratio｜杠杆比率

本题采用的杠杆比率为**持仓资产价值除以投入的自有资金**：

\[
Leverage\ Ratio=\frac{Total\ Position\ Value}{Investor's\ Equity}
\]

相应地：

\[
Investor's\ Equity=\frac{Total\ Position\ Value}{Leverage\ Ratio}
\]

- **Initial Margin（初始保证金比例/自有资金比例）** = Investor's Equity / Total Position Value = 1 / Leverage Ratio。
- 不要混淆 Leverage Ratio（倍数）与 Initial Margin（比例）。杠杆倍数 1.6 代表初始自有资金占总持仓的 \(1/1.6=62.5\%\)，其余 37.5% 由借款提供。

### Holding Period Return (HPR)｜持有期收益率

- **定义**：投资者在整个持有期内的累计回报率。
- 忽略分红时，股票价格本身的回报率为：

\[
R_{stock}=\frac{P_1-P_0}{P_0}
\]

- 对本题这种融资买入并持有到卖出的交易，忽略利息、股息与费用时：

\[
R_{equity}=Leverage\ Ratio\times R_{stock}
\]

- 此处的 \(R_{equity}\) 是**自有资金的持有期收益率**，不是股票本身的收益率，也不是年化收益率。
- 若考虑融资利息与费用，则需要从投资收益中扣除相应成本，不能直接套用上述简式。

### Annualized Return / Compound Annual Growth Rate (CAGR)｜年化收益率/复合年增长率

当题目给出持有期收益率 HPR 和持有年数 \(T\)，且期间没有额外投入或取出现金流时：

\[
R_{annual}=(1+HPR)^{1/T}-1
\]

- **复合年化（Geometric Annualization）**考虑收益复利效应。
- 不要直接用 \(HPR/T\) 来代替复合年化收益率；那是简单平均的口径。
- 要区分 **Holding Period Return（整个期间回报）** 与 **Annualized Return（折算年回报）**。

### 典型题：融资买入 500 股，两年后出售

**题目条件**：买入 500 股，买入价 $50，杠杆比率 1.6；两年后每股 $70 卖出。忽略交易成本、融资利息及股息。求年化收益率。

**方法一：快速计算**

1. 股票两年回报率：

\[
R_{stock}=\frac{70-50}{50}=40\%
\]

2. 融资交易的自有资金两年回报率：

\[
HPR=40\%\times1.6=64\%
\]

3. 将两年持有期回报复合年化：

\[
R_{annual}=(1.64)^{1/2}-1\approx28.06\%
\]

**正确答案：A. 28%。** B. 64% 只是两年 Holding Period Return，不是 Annualized Return。

**方法二：通过实际借款核算**

| 项目 | 计算 | 金额 |
|---|---|---:|
| 初始股票资产 | \(500\times\$50\) | $25,000 |
| 初始自有资金 | \(\$25,000/1.6\) | $15,625 |
| 融资借款本金 | \(\$25,000-\$15,625\) | $9,375 |
| 两年后卖出所得 | \(500\times\$70\) | $35,000 |
| 偿还借款后剩余 | \(\$35,000-\$9,375\) | $25,625 |
| 自有资金盈利 | \(\$25,625-\$15,625\) | $10,000 |

\[
HPR=\frac{25,625-15,625}{15,625}=64\%
\]

\[
R_{annual}=\sqrt{1+64\%}-1\approx28.06\%
\]

### 易错点与考场判断

1. **64% ≠ 28%**：64% 是两年的累计回报，28.06% 才是年化回报。
2. **64% ÷ 2 = 32% 不适用**：题目要求复合年化，而非算术平均年回报。
3. **1.6 倍杠杆 ≠ 1.6 倍收益率**：是用 1.6 乘股票价格回报率 40%，不是再乘最终年化率；结果须先计算 HPR，再年化。
4. **杠杆双向放大**：若股票跌价，忽略融资成本时，初始杠杆也放大自有资金亏损。
5. **无需单独使用 500 股**：快捷法里数量会约掉；逐项核算法能帮助验证自有资金、借款和卖出所得。

**考试速记**：Stock HPR × Initial Leverage → Equity HPR → CAGR。

## 5. Primary Market, Secondary Market and Instrument Types｜一级、二级市场与金融工具分类

### Primary Market｜一级市场／发行市场

- **定义**：新证券首次发行或新金融合约被创建的市场环节，重点在于**新的金融工具或合约产生**。
- **典型情形**：企业 IPO（Initial Public Offering，首次公开募股）、新债券发行（New Bond Issue）。
- **本题用法**：题干为 *issue new stock index futures*，按题目设定将新的期货合约创建归为 **Primary Market**。
- **提醒**：这是考试对市场分类的简化表述。现实交易所一般负责**上市、提供交易及规则体系**，并非像上市公司那样发行股票募集资本；期货新持仓的建立也不同于公司 IPO，不应机械理解为“投资者把发行款交给交易所”。

### Secondary Market｜二级市场／流通市场

- **定义**：已发行证券在投资者间买卖的市场，主要用于交易和流动性提供。
- **典型情形**：投资者之间买卖已经上市的股票或流通债券。
- **考试关键词**：Trading of existing securities、Resale、Between investors。
- **注意**：金融交易中“买卖股票”不自动等于 Primary Market，需要看是否是**新证券发行**。

### Derivative Contract｜衍生品合约

- **定义**：价值由某种标的资产、价格或指数（Underlying Asset / Underlying）衍生的金融合约。
- **典型品种**：Forwards（远期）、Futures（期货）、Options（期权）、Swaps（互换）。
- **Stock Index Futures（股票指数期货）**：以股票指数为标的的期货合约，属于衍生品，不是持有指数成分股票所有权的 Equity Security（股票类证券）。
- **本题关键词**：Futures → Derivative Contracts。

### Equity Securities｜股票类证券／权益证券

- **定义**：通常代表发行人剩余权益或所有权请求权的证券，如 Common Shares（普通股）、Preferred Shares（优先股）。
- **与股票指数期货区别**：买入股票通常取得股份权益；持有股票指数期货获得的是基于指数变动的合同权利和义务，并不因此直接持有指数成分股。

### Pooled Investment Vehicles｜集合投资工具

- **定义**：将多个投资者资金汇集后，按共同投资目标或策略统一投资和管理的工具。
- **例子**：Mutual Funds（共同基金／开放式基金）、ETFs（交易型开放式指数基金）等。
- **本题易错点**：股票指数期货（Stock Index Futures）是一种衍生品，并非因为标的是整个指数，就成为 Pooled Investment Vehicle。指数本身也不是资金池。

### 两个独立的分类维度

| 分类维度 | 选项举例 | 判断问题 |
|---|---|---|
| 市场类型 | Primary / Secondary Market | 是否为新证券发行或新合约形成，还是既有证券流通？ |
| 金融工具类型 | Equity Securities / Derivatives / Pooled Investment Vehicles | 是股份权益、衍生合约，还是共同投资资金池？ |

### 典型题：Toronto Stock Exchange 推出新的股票指数期货

> The Toronto Stock Exchange plans to issue new stock index futures to the investors. This trading is most likely known as:

- A. Equity securities in primary market：**错误**，Stock Index Futures 不属于 Equity Securities。
- B. Pooled investment vehicles in secondary market：**错误**，Stock Index Futures 不是 Pooled Investment Vehicles，且题目强调 *new*。
- C. Derivative contracts in primary market：**按本题标准答案正确**；Futures = Derivative Contracts，且 *new* 表示新合约。
- **做题顺序**：先看金融工具类型（Futures），再看发行／交易环节（New）。

**谨慎表述**：这道题将期货新合约“发行”视为一级市场，是为选择题分类服务的简化；现实中期货通常由交易所挂牌并通过清算机制建立合约头寸，不完全沿用股票发行/二级转让的概念框架，不能由本题推导出“交易所像上市公司一样募集发行资金”。

**考试速记**：Futures = Derivatives；New issue = Primary；Existing security trading = Secondary；Pooled fund ≠ Index future。

## 6. IPO, Underwriting and Private Placement｜首次公开募股、承销与私募

### Initial Public Offering (IPO)｜首次公开募股

- **定义**：一家企业首次向公众投资者公开发售股份（First Public Offering of Shares），通常是股票进入公开市场的重要环节。
- **关键词**：First、Public、Offering（首次、公众、发售）。
- **考试易错点**：题干若说仅向一小组 Qualified Investors（合格投资者）销售证券，通常描述 **Private Placement（私募发行）**，而不是 IPO。
- **补充**：IPO 发行可能涉及新股，也可能包含现有股东出售的股份，具体取决于发行安排；不能简单认定所有 IPO 销售所得都进入公司。

### Private Placement｜私募发行

- **定义**：证券不面向一般公众公开发售，而是向有限数量的机构或其他符合资格的投资者进行非公开发行／出售。
- **识别关键词**：Small Group、Qualified Investors、Selected Investors、Not Offered to the General Public。
- **区别**：IPO 强调首次向公众发售股票；Private Placement 强调非公开方式及特定投资者范围。

### Investment Bank / Underwriter｜投资银行／承销商

- **定义**：协助发行人设计发行方案、定价、销售和分销证券的金融中介机构。承销商是否承担未售出证券的风险，取决于承销协议。
- **本题考点**：Firm Commitment（坚定承诺／包销）与 Best Efforts（尽力承销／代销）的**未售出证券风险归属**不同。

### Firm Commitment Underwriting / Underwritten Offering｜坚定承诺承销／包销

- **定义**：在典型 Firm Commitment 承销中，投资银行按约定条件向发行人购入整批证券，再向投资者分销。
- **风险承担者**：投资银行（Investment Bank / Underwriter）承担无法按预期价格或数量转售、留下未售出证券的风险。
- **识别关键词**：Underwriter purchases the issue、Assumes the risk、Unsold Securities、Firm Commitment。
- **注意**：题目中的 *underwritten offering* 按标准答案采用承销商承担发行销售风险的口径；具体合同风险仍应以是否为 firm commitment 为准。

### Best Efforts Offering｜尽力承销／代销

- **定义**：投资银行尽合理／约定努力帮助发行人推销证券，但通常不承诺买下未售出的证券。
- **风险承担者**：发行人（Issuer）通常承担无法完成全部销售的风险。
- **识别关键词**：Best Efforts、No Obligation to Buy Unsold Securities、No Guarantee of Full Sale。
- **注意**：Best Efforts 不等于投资银行可以不履行勤勉销售义务，而是其通常不承担包销剩余证券的购买义务。

### Firm Commitment vs Best Efforts｜核心对比

| 比较项目 | Firm Commitment Underwriting | Best Efforts Offering |
|---|---|---|
| 中文 | 坚定承诺承销／包销 | 尽力承销／代销 |
| 承销商买下整批证券？ | 按约定承诺购买 | 通常不需要 |
| 未售出证券风险主要由谁承担？ | 投资银行／承销商 | 发行人 |
| 是否保证全部售出给最终投资者？ | 不保证最终售出，但承销商承担库存／转售风险 | 不保证 |
| CFA 判断关键词 | Takes the risk; Purchases issue | Best efforts; No obligation to purchase unsold |

### 例子：发行 100 万股

假设公司打算发行 100 万股，最终投资者只认购 80 万股：

- **Firm Commitment**：投资银行按承销承诺购买发行证券，再对外销售；剩余 20 万股的风险通常由承销商承担。
- **Best Efforts**：投资银行仅按约定尽力销售；对于剩余 20 万股通常没有强制购入义务，发行人承受募集不足风险。

### 典型题：With respect to IPO, which statement is most correct?

- **A 错误**：*Sell securities to a small group of qualified investors* 描述 Private Placement（私募），而非 IPO 公开发售。
- **B 正确**：*Investment bank takes the risk that the entire issue will not be sold under an underwritten offering*。按 Firm Commitment Underwriting 理解，承销商承担销售不足的风险。
- **C 错误**：截图中的 *Under a best effort offering, the investment bank is obligated to buy the unsold ...* 与 Best Efforts 不承诺买入未售出证券的机制相反。原题选项末尾在截图中被截断，不补写缺失英文原文。

**做题顺序**：
1. Small group of qualified investors → Private Placement，不是 IPO。
2. Takes the risk of unsold issue → Firm Commitment / Underwritten Offering。
3. Best Efforts + Obligated to buy unsold → 错误。

**一句话速记**：Firm Commitment = Bank bears unsold issue risk；Best Efforts = Issuer bears shortfall risk。

## 7. Shelf Registration and Staged Equity Offerings｜储架注册与分批发行股票

### Shelf Registration｜储架注册／储架发行

- **定义**：发行人在适用证券监管规则允许的前提下，提前办理覆盖一定证券数量或规模的发行注册，并在有效期内根据融资需要分次发行证券；英文可称 **Shelf Registration**，分批实际发售称 **Shelf Offering / Takedown**。
- **核心特征**：**One Registration + Multiple Offerings（一次注册、分批发行）**。
- **适用范围**：除了债券，也可以用于符合相关规定的股票等证券发行。本章与 [[07-Fixed-Income/Fixed-Income-Basics|固定收益基础概念]] 中的 Shelf Registration 为同一个跨科目术语。
- **优点**：发行时间更灵活（Flexibility），能与经营资金需求和市场条件匹配；可以避免每次都从头重复完成整套注册流程。
- **法规提醒**：招股说明书（Prospectus）与注册申请文件（Registration Statement）不能在法律上简单视为一回事。储架发行并非后续每次发售都无需披露，具体还可能需要招股说明书补充文件（Prospectus Supplement）及满足有效期、资格条件和其他监管要求。

### Prospectus｜招股说明书／发行说明书

- **定义**：为潜在投资者说明证券发行条件、公司或发行人信息、主要风险及其他重要信息的披露文件。
- **考试关键词**：Published a prospectus、Plans to offer new shares、Public Offering。
- **注意**：题干说六月公布发行计划，不等于 3 亿股在六月已经全部发行。

### Dividend Reinvestment Plan (DRIP)｜股息再投资计划

- **定义**：股东选择将收到的现金股息（Cash Dividends）自动用于购买更多公司股票，而不是直接领取现金。
- **核心关键词**：Reinvest Dividends / Buy Additional Shares。
- **与 Shelf Registration 区别**：DRIP 关注“已有股东如何再投资分红”，而不是公司按资金需求分批向公众发行股票。

### Private Placement｜私募发行（与储架注册辨析）

- **定义**：向特定投资者或有限范围的符合资格投资者非公开发行证券。
- **关键词**：Selected Investors、Qualified Investors、Not the General Public。
- **与本题区别**：本题明确写了 **to the public（向公众出售）**，不属于所描述的私募情形。更重要的是，私募／公开是发行对象和方式的维度，储架注册是注册与发行时间安排的维度，两者不能混为同一分类标准。

### 本题时间线：Golden Company 的分批股票发行

题干：

> Golden Company published a prospectus of 300,000,000 new shares offering in June. Since the company plans to launch new products in 4 months, it tends to sell 60,000,000 shares in October and 100,000,000 shares at the end of the year to the public.

| 时间 | 发行安排 | 拟发售股票数 |
|---|---|---:|
| 六月（June） | 公布拟发行 3 亿股的说明文件 | 总计划 300,000,000 股 |
| 十月（October） | 面向公众发售第一批 | 60,000,000 股 |
| 年底（End of year） | 面向公众发售第二批 | 100,000,000 股 |
| 未来 | 未明确后续出售时间 | 140,000,000 股（按计划计算的余额） |

**判断**：同一总体发行计划下，根据资金需求分批公开发售新股 → **B. Shelf Registration（储架注册）**。

### 三选项对比与易错点

| 选项 | 关键词 | 是否符合题意 |
|---|---|---|
| A. Dividend Reinvestment Plan | 股东将股息再购买股票 | 否：题干没有股息再投资 |
| B. Shelf Registration | 总体发行计划 + 后续多批发行 | **是：正确答案** |
| C. Private Placement | 面向特定投资者非公开发行 | 否：题干是 to the public |

- 不能仅因为出现 **Prospectus** 就选 Shelf Registration；必须结合**同一发行计划分多次落实**。
- **300,000,000 − 60,000,000 − 100,000,000 = 140,000,000**，只是剩余的拟发行额度，不表示已经上市或必定在某天发行。
- 私募（Private Placement）与储架（Shelf Registration）不是完全互斥的通用法规概念；本题三选一时按照最能体现交易安排的选项来选。

**考试速记**：One registration, several takedowns = Shelf Registration；Dividends reinvested = DRIP；Selected investors = Private Placement。

## 8. Price-Weighted Index and Price Return｜价格加权指数与价格收益率

### Price-Weighted Index｜价格加权指数

- **定义**：根据指数成分证券的每股价格（Share Price）确定权重的股票指数。价格较高的股票在指数中的权重通常更大，与公司规模或市值高低不是同一概念。
- **基本计算**：

\[
Index\ Level=\frac{\sum_{i=1}^{N}P_i}{D}
\]

其中 \(P_i\) 为第 \(i\) 只成分股的价格，\(D\) 为指数除数（Index Divisor）。最初无特殊调整的简化情形常取 \(D=N\)（成分股数量），即**价格算术平均值**。
- **为什么需要 Index Divisor（指数除数）？** 当出现拆股（Stock Split）、成分股调整等不应单凭机械价格变动就令指数跳变的事项时，指数编制者可能调整除数以维持连续性。
- **权重理解**：在同一计算时点、常规价格加权结构下，股票 \(i\) 的相对权重为 \(w_i=P_i/\sum P_i\)。它不是 Equal-Weighted（等权重）或 Market-Capitalization-Weighted（市值加权）。

### Market-Capitalization-Weighted Index｜市值加权指数

- **定义**：按每只成分股的市值（Market Capitalization / Market Value）大小分配指数权重；市值越大，在其他条件相同时对指数收益率的影响越大。
- **Market Capitalization（股票总市值）** = Share Price（每股价格） × Shares Outstanding（流通在外的股份总数）。
- **注意**：Shares Outstanding 是已发行且在外流通的股份总数，不一定等于实际可自由交易的 Free Float Shares（自由流通股份）。

**完全市值加权指数（Full Market-Capitalization-Weighted Index）的权重公式**：

\[
\boxed{w_i=\frac{P_iQ_i}{\sum_{j=1}^{N}P_jQ_j}}
\]

其中 \(P_i\) 为第 \(i\) 只股票价格，\(Q_i\) 为其流通在外股份数，\(w_i\) 为指数权重。权重求和为 100%。

**指数收益率**（固定成分、无额外公司行动和权重重构的简单情形）：

\[
R_{index}=\sum_{i=1}^{N}w_{i,0}\times R_i
\]

其中 \(w_{i,0}\) 是期初指数权重，\(R_i\) 是对应成分股在这一期间的收益率。

- **影响大小的重要限定**：*The largest market value* 表示**最大权重**，但实际的指数收益贡献还取决于该股票涨跌幅 \(R_i\)；只有比较相同涨跌幅时，最大市值对应最大绝对贡献。若小市值股票涨跌特别大，实际贡献也可能更大。本题问的是加权方法的主要决定因素。
- **Float-Adjusted Market-Capitalization Weighting（自由流通市值加权）**：某些指数只考虑自由流通股份计算权重，须按题干规定的市值口径判断。

#### 直观例子：市值权重而非单看股价或股份数

| 股票 | 每股价格 | Shares Outstanding | 股票市值 | 指数权重 |
|---|---:|---:|---:|---:|
| A | 100 元 | 100 万股 | 1 亿元 | 10% |
| B | 20 元 | 1,000 万股 | 2 亿元 | 20% |
| C | 50 元 | 1,400 万股 | 7 亿元 | 70% |
| 合计 | — | — | 10 亿元 | 100% |

- **A** 股价最高，但权重仅 10%。
- **C** 股价不是最高，却因总市值最大而具有 70% 的权重。
- 若三只股票各上涨 10%，对指数上涨贡献依次为 1、2、7 个百分点；C 贡献最大。

#### 与 Price-Weighted Index 对比

| 加权方法 | 权重主要由什么决定？ | 高影响力的成分股 |
|---|---|---|
| Price-Weighted Index（价格加权） | 单只股票每股价格 \(P_i\) | 每股价格高者权重更高 |
| Market-Capitalization-Weighted Index（市值加权） | 每股价格 × 股份数量 \(P_iQ_i\) | 市值高者权重更高 |
| Equal-Weighted Index（等权重） | 各股票初始权重相同 | 同样涨幅时贡献相同 |

#### 本题：Which factor has the largest impact on the index return based on the market-capitalization weighted method?

- **A. The lowest stock price — 错误。** 仅价格低无法判断市值，更无法判断市值权重。
- **B. The largest numbers of shares outstanding — 错误。** 股份数量最多不代表总市值最高，还要看价格。
- **C. The largest market value — 正确。** 市值最高的成分股对应最大指数权重；在相同回报率下影响最大。

**考试速记**：Price-Weighted 看 Price；Market-Cap-Weighted 看 Price × Shares；Equal-Weighted 看 Equal Weight。指数实际回报贡献还取决于个股涨跌幅。

### Price Return｜价格收益率

- **定义**：只反映证券或指数价格变动形成的收益率，**不计股息（Dividends）**。
- **Price Return Index（价格收益指数）**：只追踪成分证券价格变化，不把现金分红再投资计入指数收益。

\[
R_{price}=\frac{Index_{end}}{Index_{begin}}-1
\]

**本题无成分调整、拆股及除数变化的简化条件下**，初末指数使用同一除数，消去后：

\[
\boxed{R_{price}=\frac{\sum P_{end}-\sum P_{begin}}{\sum P_{begin}}}
\]

- 若计算期内除数因拆股或成分变化而调整，不能直接用**初末简单股价和**套用上式；须按调整后的指数水平和编制规则计算。

### Total Return｜总收益率

- **定义**：既考虑价格变化，也考虑股息等现金分配带来的收益，指数总回报的计算遵循相关分红再投资规则。
- **Total Return Index（总收益指数）**：在价格变化之外，按指定方法将股息再投资纳入指数表现。
- **判断原则**：题目明确问 **Price Return** 时，即使数据表提供 Total Dividends，也不要把股息加进分子。

### 本题：三只股票的价格加权指数

题干：Doug Greyson is measuring the performance of the market based on the price-weighted index. The price return of the index is:

| 股票 | Beginning of Period Price (RMB) | End of Period Price (RMB) | Total Dividends (RMB) |
|---|---:|---:|---:|
| A | 50 | 54 | 2 |
| B | 35 | 50 | 3 |
| C | 30 | 32 | 2 |
| **合计** | **115** | **136** | **7** |

**计算方法一：股价和直接计算**

\[
R_{price}=\frac{136-115}{115}=\frac{21}{115}=18.260869\%\approx18.26\%
\]

**答案：C. 18.26%。** 本题没有需要调整除数的说明，因此可以直接使用简化计算。股息合计 7 元不纳入 Price Return。

**计算方法二：先算指数水平**

- 期初指数水平：\((50+35+30)/3=38.3333\)。
- 期末指数水平：\((54+50+32)/3=45.3333\)。

\[
R_{price}=\frac{45.3333-38.3333}{38.3333}\approx18.26\%
\]

**方法三：理解价格加权权重**

| 股票 | 期初价格权重 \(w_i=P_{0,i}/115\) | 个股价格收益率 |
|---|---:|---:|
| A | 43.48% | \(4/50=8.00\%\) |
| B | 30.43% | \(15/35=42.86\%\) |
| C | 26.09% | \(2/30=6.67\%\) |

按照期初权重加权各股价格收益率，也得到约 18.26%。这说明 **Price-Weighted ≠ 简单平均三只股票的百分比收益率**。

### 易错点

1. **Price Return ≠ Total Return**：表格给了 Total Dividends，并不表示一定要使用；本题明确只问价格收益率。
2. **Price-Weighted ≠ Equal-Weighted**：不能把三只股票的 8%、42.86%、6.67% 直接取算术平均。
3. **Price-Weighted ≠ Market-Cap-Weighted**：题中没有股数、总市值，不需要计算市值权重。
4. **除数可调整**：若题目出现 Stock Split、指数调整等事件，必须检查 Index Divisor 是否变化，不能机械套用初末股价和公式。
5. **与此前学过的 CAGR 区分**：本题问一个 Period 的价格收益率，不是多年度的复合年化收益率。

**考试速记**：Price-Weighted → Sum of Share Prices / Divisor；Price Return → Price Changes Only，Ignore Dividends。

## 9. Fixed-Income vs Equity Index Constituents｜债券指数与股票指数成分证券的差异

### 核心区别：债券需要更多分类维度

- **Equity Index（股票指数）**：由股票等权益证券作为成分证券（Constituent Securities），可按行业（Sector）、公司市值（Market Capitalization）、国家和投资风格（Investment Style）等维度分类。
- **Fixed-Income Index / Bond Index（固定收益指数／债券指数）**：由符合规则的债券等固定收益证券组成。除了发行主体不同，同一发行主体也可能发行大量具有不同到期日、信用质量和合同条款的债券。
- **CFA 判断**：相较于股票指数，固定收益指数的成分证券通常 **Classified Along More Dimensions（按更多维度分类）**。

| 债券分类维度（Classification Dimension） | 英文 | 常见差别 |
|---|---|---|
| 发行人类型 | Issuer Type | 主权政府、地方政府、公司等 |
| 到期期限 | Maturity / Time to Maturity | 短期、中期、长期 |
| 信用评级／信用质量 | Credit Rating / Credit Quality | 投资级、投机级及具体评级 |
| 票息结构 | Coupon Structure | 固定利率、浮动利率、零息等 |
| 计价货币 | Currency | 美元、人民币、欧元等 |
| 偿付优先级 | Seniority | 优先、次级等 |
| 税务特征（视市场而定） | Tax Status | 某些债券可能享有特定税务待遇 |

**直观例子**：同一家企业发行 3 年期固定利率债券和 10 年期浮动利率债券，即使发行人相同，两只债券的风险和现金流特征也不同。这会影响它们被纳入哪一类债券指数。

### Price Transparency｜价格透明度

- **股票**：大型上市股票通常在集中交易所活跃交易，交易价格和报价较为频繁、透明。
- **债券**：很多单只债券在 Over-the-Counter (OTC，场外市场) 交易，成交频率可能较低，某些债券缺少连续成交价，需要依赖报价或估值。
- **CFA 判断**：相比股票，固定收益指数的成分证券通常**并非**具有更频繁、更透明的价格数据（Frequent and Transparent Price Data）。
- **限制**：这是典型市场比较；活跃国债可能很透明，也存在不活跃股票，不能绝对化。

### Investment Horizon vs Maturity｜投资期限与到期期限

- **Investment Horizon（投资期限）**：投资者计划持有某项资产的时间。
- **Maturity（债券到期期限）**：债券合同约定的本金偿还日期／剩余期限。
- **区别**：多数普通债券有到期日，普通股通常没有固定到期日；不能推断债券指数的成分证券普遍具有比股票更长的 Investment Horizon。

### 与固定收益模块已整理知识点的联系

参见：[[07-Fixed-Income/Fixed-Income-Basics|Fixed Income Basics]] 中的 **Bond Indexes and Equity Indexes｜债券指数与股票指数**。

广泛债券指数（Broad Bond Index）与广泛股票指数（Broad Equity Index）比较时，债券指数往往：
- **More Constituents（成分数量更多）**：单个发行人可能发行多个债券品种。
- **Higher Turnover（成分周转率较高）**：债券到期、新发行及信用评级变化等影响纳入资格。
- **Harder Full Replication（完全复制更难）**：成分多、流动性差异和场外交易提高复制难度。
- **More Classification Dimensions（分类维度更多）**：债券具体合约特征较丰富。

### 典型题：Compared to equity indexes ...

> Compared to equity indexes, the constituent securities of fixed-income indexes are most likely:

- **A. With longer investment horizon — 错误**：投资者持有期限与证券约定到期期限不同，不能概括债券的持有期限更长。
- **B. With frequent and transparent price data — 错误**：许多债券在 OTC 市场交易、成交不频繁，价格数据通常不如活跃股票透明。
- **C. Classified along more dimensions — 正确**：债券按发行人、期限、信用评级、票息、币种、偿付优先级等更多维度分类。


### 典型题：In contrast with equity index, bond index has the following characteristics EXCEPT

> In contrast with equity index, bond index has the following characteristics except that:

- **A. Bond index has a broad universe — 属于典型特征（不选）**。**Broad Universe（广泛的可选债券集合）**意味着市场中有大量不同发行人、期限、信用质量与条款的债券。同一发行人也可能有多只债券存续，广泛债券指数通常面对比股票指数更庞大的可选证券范围。
- **B. Bond index has less turnover — 不符合典型特征（正确答案）**。债券有固定 Maturity（到期日）；到期退指、新发行债券入指、评级变化或剩余期限不符合指数规则，都会令成分变动。故广泛债券指数通常有 **Higher Index Turnover（更高的成分周转率）**，而不是 Less Turnover。这里的 Index Turnover 是**指数成分调整频率**，不是日常成交量 Trading Volume。
- **C. Bond index providers rely on dealers for prices — 属于典型特征（不选）**。许多债券通过 OTC 场外市场交易，缺乏连续交易所成交价；指数编制机构（Index Providers）可能参考 Dealer Quotes（交易商报价）、成交数据及第三方估值形成指数价格。这里的 rely on dealers 不代表全部债券价格只能来自单一交易商。

**本题陷阱：EXCEPT = 选出不符合描述的一项**。A（范围广）和 C（依赖交易商报价）通常正确，B（较低成分周转率）错误，因此选择 **B**。

**两题串联：**上一题正确特点是 More Classification Dimensions；本题错误特点是 Less Turnover。联合记忆：**Bond Index = Broad Universe + More Dimensions + Higher Turnover + Dealer/OTC Pricing + Harder Replication**。

**考试速记**：Bond Index → More Dimensions + Less Transparent Pricing + Higher Turnover + Harder Replication。

## 10. Alternative Investment Indices｜另类投资指数基础概念

### Alternative Investment Indices｜另类投资指数

- **定义**：跟踪传统股票和债券以外的特定投资类别表现的指数。本题重点包括 **Commodity Indices（商品指数）**、**Hedge Fund Indices（对冲基金指数）** 和 **Real Estate Indices（房地产指数）**。
- **考法**：分别识别商品期货指数的收益来源、对冲基金指数的样本偏差，以及房地产指数的常见类型。

### Commodity Index｜商品指数

- **定义**：按指数规则选取和配置一种或多种商品相关资产或期货合约，以衡量相关商品投资表现的指数。
- **典型投资型商品指数**：常由 Commodity Futures Contracts（商品期货合约）构成，而不是直接持有黄金、原油、农产品等实物商品（Physical Commodities）。
- **Underlying Commodity（标的商品）**：期货合约所依据的实物商品或其价格；其现货价格（Spot Price）表现不一定等于商品期货指数收益。
- **为什么指数与标的商品回报可能不同**：
  1. 期货到期前必须按照规则展期（Rolling），不同期货期限的价格结构会影响收益。
  2. 不同商品指数的成分选择、权重（Weighting Method）及展期方法（Roll Method）可能不同。
  3. 全收益指数（Total Return Index）可能计入支持期货头寸的现金抵押品收益，而现货价格指数不计入。

### Spot Return, Roll Return, Collateral Return｜商品期货收益的三个常见来源

在**完全现金抵押的商品期货投资（Fully Collateralized Commodity Futures Investment）**、使用标准的收益分解口径时：

\[
R_{total}\approx R_{spot}+R_{roll}+R_{collateral}
\]

- **Spot Return（现货价格收益）**：标的商品现货价格变化形成的收益贡献。
- **Roll Return / Roll Yield（展期收益）**：期货合约到期前，按策略卖出原合约、买入后续合约所产生的收益影响，受到期货期限结构（Term Structure）的影响。
- **Collateral Return / Collateral Yield（抵押品收益）**：现金抵押品或与之类似的短期安全资产产生的回报。
- **重要限制**：并非每一种商品指数都包含相同收益项目。有 Price / Spot、Excess Return、Total Return 等不同指数口径；题干仅说 *could be different*，不意味着每种商品指数都一定不同于现货表现。
- **示例（教学假设）**：现货上涨 10%，展期收益 −4%，现金抵押品收益 +2%，总收益约 8%。说明期货指数收益不必与标的商品现货涨幅一致。

**参考**：[CFA Institute — Introduction to Commodities and Commodity Derivatives](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/introduction-commodities-commodity-derivatives)。

### Hedge Fund Index｜对冲基金指数

- **定义**：依据纳入的对冲基金（Hedge Funds）报告的业绩，综合衡量某类或某组基金的表现。
- **关键问题**：对冲基金的业绩披露可能是自愿的，样本并非一定能代表全部基金。

#### Survivorship Bias｜幸存者偏差

- **定义**：已关闭、业绩较差或停止报告的基金可能被指数数据库剔除，留下的基金业绩较好，使指数结果偏高。
- **例子**：五只等权基金收益分别为 +20%、+15%、+10%、−30%、−40%。若只保留前三只“幸存基金”，平均收益为 +15%；全部纳入的平均收益为 −5%。该假设仅用来说明样本筛选对报告结果的影响。
- **考试陷阱**：*Hedge fund indices do not suffer from survivorship bias* → **错误**。对冲基金指数恰恰常被提醒存在此类偏差。

#### Backfill Bias｜回填偏差／历史业绩回填偏差

- **定义**：基金开始向指数数据库报告时，可能选择将此前表现良好的历史业绩一起补录，使历史指数回报出现向上偏差。
- **区别**：Survivorship Bias 是**表现差的基金退出数据库**；Backfill Bias 是**后来加入者可能选择性提交较好的历史业绩**。两者都可能高估业绩。

### Real Estate Index｜房地产指数

本题常见的三类：

| 类别 | 英文 | 数据基础与特点 |
|---|---|---|
| 评估价值指数 | Appraisal-Based Index | 定期专业评估地产价值；估值可能滞后、平滑波动 |
| 重复销售指数 | Repeat-Sales Index | 使用同一房产不同时间的重复成交价格衡量变化 |
| 房地产投资信托基金指数 | REIT Index | 跟踪上市或符合指数标准的 REITs 证券市场表现 |

- **REIT (Real Estate Investment Trust，房地产投资信托基金)**：以房地产资产、相关权益或抵押贷款等为主要投资对象的投资工具；符合规则的上市 REIT 证券可纳入 REIT Index。
- **C 选项为什么错**：*Real estate indices can only be classified into appraisal indices and repeat sales indices* 忽略了 REIT Index（房地产投资信托基金指数）。**Only** 是绝对化关键词。

### 本题：Regarding the various alternative investment indices ...

> Regarding the various alternative investment indices, which of the following is most accurate?

- **A. The performance of commodity indices could be different from the underlying commodities'. — 正确。** 商品期货指数可因期货展期、权重和抵押品收益而不同于标的商品现货表现。
- **B. Hedge fund indices do not suffer from survivorship bias. — 错误。** 对冲基金指数可能存在幸存者偏差，表现较差或关闭的基金不再计入数据库会高估历史业绩。
- **C. Real estate indices can only be classified into appraisal indices and repeat sales indices. — 错误。** 还存在 REIT Index；“only” 过于绝对。

**考试速记**：
1. **Commodity Index ≠ Spot Commodity Return**（商品期货指数收益不等于商品现货涨幅）。
2. **Hedge Fund Index → Survivorship & Backfill Bias**（对冲基金指数留意样本偏差）。
3. **Real Estate Index → Appraisal + Repeat Sales + REIT**（房地产指数三种常见类型）。

**相关科目**：[[09-Alternative-Investments/INDEX|另类投资（Alternative Investments）]]。本题出现在 Equity Investments 中的 Security Market Indices 主题，与另类投资模块存在交叉。

## 11. Behavioral Finance and Investor Biases｜行为金融学与投资者偏差

### Behavioral Finance｜行为金融学

- **定义**：研究心理因素、认知方式和社会互动如何影响投资者决策及金融市场表现。
- **本题关注**：投资者对自身的信息处理和解释能力过度确信，属于 Overconfidence（过度自信）。
- **Cognitive Bias（认知偏差）**：信息处理、推理或判断过程中的系统性偏差；与情绪偏差（Emotional Bias）可做概念区分。

### Overconfidence / Overconfidence Bias｜过度自信／过度自信偏差

- **定义**：投资者高估自己的知识、分析能力、预测准确度或对结果的控制程度，对自身判断过分确信。
- **识别关键词**：Always、Can Process and Interpret Information Precisely、Overestimate Own Ability、Too Certain of Their Judgment。
- **直观例子**：投资者阅读一家公司的财报后，确信自己能完全理解所有信息，并认为预测几乎不会出错，忽视不确定性和可能的反面证据。
- **可能后果**：Excessive Trading（过度交易）、Underdiversification（分散投资不足）、过度集中头寸或低估风险。
- **本题关键**：题干说投资者 *believe they can always*（主观认为自己始终能够做到），而不是证明其信息处理实际上一直准确。因此主要考查的是**对自身能力的过高信心**。
- **交叉内容**：投资组合管理（Portfolio Management）也会学习行为偏差；词汇表已在 Ethics 部分收录 Overconfidence 的基础释义，此处增加投资情境。

### Loss Aversion｜损失厌恶

- **定义**：在其他条件相似的情况下，同等金额损失带来的心理痛苦通常强于同等金额收益带来的愉悦。
- **识别关键词**：Dislike Losses More Than Equivalent Gains、Reluctant to Realize Losses。
- **例子**：亏损 1,000 元产生的痛苦，可能超过赚取 1,000 元带来的快乐。
- **常见延伸**：可能不愿卖出亏损头寸、过早兑现盈利；但这些行为并非所有损失厌恶者都会出现，不能当作严格定义。
- **与本题区别**：题干谈的是**信息处理能力的自我评价**，没有描述对收益与损失的不对称心理反应。

### Information Cascades｜信息瀑布效应／信息级联

- **定义**：一个人观察到前面其他人的行动后，可能推断他们掌握了更有价值的信息，从而忽视自己的私人信息（Private Information）并跟随他人做出决定；后续参与者继续模仿，形成连锁决策。
- **识别关键词**：Follow Earlier Investors' Actions、Ignore Own Information、Copy Others' Choices。
- **例子**：前面多位投资者买入某只股票，后来者尽管自己的分析并不支持买入，仍认为前面的人“肯定知道些什么”，于是跟随买入。
- **与本题区别**：题干说的是相信**自己**的分析总准确，未提到观察并追随**他人**行动，因此不选 Information Cascades。
- **与 Herding（羊群行为）的关系**：信息瀑布可以推动羊群式决策，但强调的是从前面参与者的行动推断信息并忽略私人信号，不只是简单地“大家都在买，所以跟着买”。

### 三种偏差对比

| 类型 | 英文 | 主要心理机制 | 典型线索 |
|---|---|---|---|
| 过度自信 | Overconfidence | 高估自己的判断能力 | I am always right |
| 损失厌恶 | Loss Aversion | 同等损失的痛苦大于收益快乐 | Losses hurt more |
| 信息瀑布 | Information Cascades | 从他人行动推断信息并跟随 | Follow others despite private signal |

### 本题：If investors believe they can always process and interpret information precisely ...

> If investors believe they can always process and interpret information precisely, they most likely exhibit:

- **A. Loss aversion — 错误**。题目没有提到对损失的厌恶程度，或收益与损失的不对称反应。
- **B. Overconfidence — 正确**。投资者认为自己始终能准确处理、理解信息，体现对自身认知和分析能力的过度确信。
- **C. Information cascades — 错误**。题目没有提到观察他人行动、追随其他交易者或放弃个人信息。

**考试判断顺序**：
1. 自己的分析判断总准确？→ **Overconfidence**。
2. 同样金额更怕亏损？→ **Loss Aversion**。
3. 看别人行动并忽略自己掌握的信息？→ **Information Cascades**。

**考试速记**：Overconfidence = Trust Myself Too Much；Loss Aversion = Fear Losses More；Information Cascades = Follow Others' Actions。

## 12. 复习清单

- [ ] 能解释 Hedger、Speculator、Investor、Securitizer 的区别
- [ ] 能识别农民卖出远期与航空公司买入远期分别在对冲什么风险
- [ ] 知道同一种交易工具可以用于 Hedging，也可以用于 Speculation
- [ ] 能解释套期保值为何可能放弃有利行情带来的额外收益
- [ ] 能区分 Leverage Ratio、Initial Margin 和 Margin Loan
- [ ] 能区分 HPR 与 Annualized Return，并将杠杆收益复合年化
- [ ] 能区分一级市场与二级市场
- [ ] 能区分 Equity Securities、Pooled Investment Vehicles 与 Derivatives
- [ ] 能区分 IPO 和 Private Placement
- [ ] 能解释 Firm Commitment 与 Best Efforts 的未售出证券风险由谁承担
- [ ] 能区分 Shelf Registration、Dividend Reinvestment Plan 与 Private Placement
- [ ] 能计算 Price-Weighted Index 的 Price Return，并明确忽略 Dividends
- [ ] 能写出市值加权公式、说明市值与指数权重的关系，区分价格加权和市值加权
- [ ] 能说明何时不能直接用初末股价和计算收益率（除数调整）
- [ ] 能解释债券指数为什么有更多分类维度，以及债券价格为何通常不如活跃股票透明
- [ ] 能解释 Broad Universe、Higher Index Turnover、Dealer Quotes，并识别 EXCEPT 题目
- [ ] 能解释商品指数为何可能与商品现货价格表现不同（期货展期、权重、抵押品收益）
- [ ] 能区分 Survivorship Bias 与 Backfill Bias，并列出房地产指数的三种常见类型
- [ ] 能区分 Overconfidence、Loss Aversion 与 Information Cascades，掌握关键词和例子

**交叉科目**：[[07-Fixed-Income/Fixed-Income-Basics|固定收益基础概念]]（Securitization）；Derivatives（远期合约机制）。
