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

## 9. 复习清单

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
- [ ] 能说明何时不能直接用初末股价和计算收益率（除数调整）

**交叉科目**：[[07-Fixed-Income/Fixed-Income-Basics|固定收益基础概念]]（Securitization）；Derivatives（远期合约机制）。
