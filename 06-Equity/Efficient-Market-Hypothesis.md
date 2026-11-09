---
subject: CFA Level I
topic: Market Efficiency
status: 持续更新
created: 2026-11-09
tags: [CFA-L1, Equity, Efficient-Market-Hypothesis, Market-Efficiency, Behavioral-Finance]
---

# Efficient Market Hypothesis (EMH)｜有效市场假说专题

[[06-Equity/INDEX|返回权益投资目录]] · [[06-Equity/Equity-Investments-Basics|权益投资基础概念]]

> **一句话核心**：在有效市场中，证券价格充分、迅速地反映相应范围内的可获得信息，因此投资者很难**仅凭这些已被反映的信息**持续获得经过风险调整后的异常收益（Abnormal Return）。
>
> 三种形式的顺序：**Weak Form（历史交易信息）→ Semi-Strong Form（全部公开信息）→ Strong Form（全部公开及私人信息）**。

**学习资料范围**：本专题以 CFA Institute 的 **2026 Level I Equity Investments — Market Efficiency** 官方公开课程摘要为基础，并补充便于做题的教学例子、逻辑说明和考点辨析；完整教材可在 CFA Learning Ecosystem 访问。
官方阅读：[CFA Institute — Market Efficiency (2026)](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/market-efficiency)。

## 1. Market Efficiency｜市场有效性是什么？

**信息有效性（Informational Efficiency）**：证券价格能够迅速、充分地反映市场可获得的相关信息。若某些信息尚未充分进入价格，善于搜集、分析信息的投资者理论上可能发掘利润机会。

- **Market Price / Market Value（市场价格／市场价值）**：证券当前可在市场成交的价格。
- **Intrinsic Value（内在价值）**：基于可获得信息，对资产未来现金流及其风险作出估计而得到的经济价值。它不是可以直接观察的绝对真值，现实估值有不确定性。
- **Efficient Market（有效市场）**：市场价格通常对相应信息作出及时反应；价格可能随新信息调整，仍可能波动、跌价甚至出现事后被证明不准确的预测。

**不代表**：
1. 证券价格永远不变或永远正确。
2. 所有投资者都理性、不会亏钱。
3. 没有投资收益：投资者仍可以获得风险承担所对应的预期回报。
4. 历史上有人战胜指数，就能直接证明市场无效。

### 市场价值 vs 内在价值

| 概念 | 英文 | 关注点 |
|---|---|---|
| Market Value | 市场价值 | 现在市场上能成交的价格是多少？ |
| Intrinsic Value | 内在价值 | 根据对未来现金流和风险的分析，合理估计价值是多少？ |

在高度有效的市场中，二者通常较为接近；若相关信息未被充分反映，可能出现明显偏离，但研究者也可能错估内在价值。

## 2. Three Forms of Market Efficiency｜三种市场有效形式

按价格已经反映的**信息集合（Information Set）**分类，而不是按市场涨跌幅、交易量大小或基金经理声誉分类。

| 形式 | 市场价格反映的信息 | CFA 最常见的应用 |
|---|---|---|
| Weak-Form Efficient（弱式有效） | 历史价格、成交量和其他历史交易信息 | Technical Analysis（技术分析） |
| Semi-Strong-Form Efficient（半强式有效） | **全部公开信息**，包括历史交易数据、公开财报与公告 | Fundamental Analysis（基于公开资料的基本面分析） |
| Strong-Form Efficient（强式有效） | **所有公开与非公开信息**，包括私人信息 | Private Information（私人／未公开信息） |

### 2.1 Weak-Form Efficiency｜弱式有效

- **涵盖信息**：Past Prices、Past Returns、Trading Volume 等历史市场交易信息。
- **含义**：仅靠技术图形、过去的价格模式、成交量等不能稳定取得风险调整后且扣除必要成本的异常收益。
- **不意味着**：研究公开财报一定没用，因为公开财报超出了最小的历史价格数据集合。
- **题干线索**：Technical Analysis、Historical Trading Data、Past Price Patterns。

### 2.2 Semi-Strong-Form Efficiency｜半强式有效

- **涵盖信息**：所有公开可得信息（Publicly Available Information）——包括过去的交易数据、上市公司公告、财务报表、宏观经济新闻。
- **含义**：纯粹利用已公开信息的技术分析或基本面分析，不能持续取得风险调整后的异常收益。
- **题干线索**：Public Announcements、Earnings Releases、Financial Statements。
- **重点**：Semi-Strong 包含 Weak；若历史交易信息尚能被系统性套利，市场也不能是半强式有效。

### 2.3 Strong-Form Efficiency｜强式有效

- **涵盖信息**：公开信息与私人／非公开信息（Public and Private Information）。
- **含义**：即使掌握私人信息，也不能持续利用它取得异常收益。
- **与现实区别**：这是最严格的理论假设；CFA Institute 的公开课程总结认为实证证据不支持强式有效。利用重大非公开信息交易也可能违反法律，不应据此推导任何交易建议。
- **题干线索**：Inside Information、Private Information、Nonpublic Information。

### 2.4 包含关系及逻辑判断

\[
Strong\text{-}Form\ Efficient\Rightarrow Semi\text{-}Strong\text{-}Form\ Efficient\Rightarrow Weak\text{-}Form\ Efficient
\]

**逆向不成立**：市场若是弱式有效，并不能自动推断它也是半强式有效；市场若不能满足弱式有效，就不可能满足半强式或强式有效。

**口诀**：**弱式看历史，半强看公开，强式看全部。**

## 3. Technical vs Fundamental Analysis｜技术分析与基本面分析

| 分析方式 | 典型输入 | 对应的有效市场形式 |
|---|---|---|
| Technical Analysis（技术分析） | 历史股价、交易量、图表形态 | 检验弱式有效 |
| Fundamental Analysis（基本面分析） | 财报、公告、行业、宏观数据、估值 | 检验半强式有效（当信息全部是公开的） |
| Analysis Using Private Information（使用私人信息） | 非公开信息 | 与强式有效的严格检验有关 |

**不要背错**：
- 不是“弱式有效只允许基本面分析赚钱”，而是弱式有效**没有否定**从公开基本面信息中取得优势的可能性。
- 不是“只要技术分析模型复杂，就说明能打败市场”。题目的重点是信息类型和持续盈利的证据，不是模型复杂程度。
- 对某一特定信息集合而言，信息已经反映在价格中时，就不能指望仅靠重复处理该信息稳定取得额外回报。

## 4. Factors Affecting Market Efficiency｜影响市场有效性的因素

CFA 课程特别关注**市场参与者的数量和竞争、分析师覆盖、信息可获得性、交易限制**。

| 因素 | 通常有利于有效性 | 通常损害有效性 |
|---|---|---|
| Market Participation（市场参与） | 足够多的活跃参与者与分析竞争 | 资金、资格或地域限制使部分投资者无法参与 |
| Information Availability（信息可获得性） | 相关信息及时公开、成本合理 | 信息匮乏、披露滞后、取得成本高 |
| Analyst Coverage（分析师覆盖） | 更多独立分析与信息处理 | 研究覆盖不足，难以及时发现定价偏差 |
| Trading / Arbitrage Constraints（交易／套利限制） | 可以低成本交易和纠正错误定价 | 卖空限制、交易费用、流动性差或交易障碍 |

### 已做题：Capital Restrictions

> Capital restrictions prevent some investors from participating in the market. Effect on market efficiency?

**答案：C. Impeding Market Efficiency（阻碍市场有效性）。**

**机制**：投资者参与受限 → 信息竞争减少、部分错误定价难以被纠正 → Price Discovery（价格发现）受阻 → Informational Efficiency 可能下降。

**限定**：不能直接等同“成交量少 = 必然无效”；题目考的是参与壁垒可能削弱纠正定价偏差的机制。不同监管限制也可能有其他政策目标。

## 5. Active vs Passive Investing｜主动管理与被动管理

- **Active Management（主动管理）**：主动选择证券、择时或调整仓位，试图获得相对基准的额外回报。
- **Passive Management（被动管理）**：按一定指数或市场组合规则进行投资，通常减少主动择股和择时成本。
- **高有效性市场的含义**：依赖市场已充分反映的信息寻找稳定超额收益更难，**低成本被动投资**通常更有吸引力。
- **有效性较低的市场**：研究或交易技巧可能更有价值，但也必须考虑成本、流动性和风险，不能推论“主动管理必定赚钱”。
- **市场有效不代表所有投资者都必须被动管理**：风险偏好、税务需求、负债匹配和个人约束等仍会影响投资组合选择。

## 6. Testing Market Efficiency｜检验市场是否有效

### 6.1 风险调整后的超额收益与 Alpha

实际投资组合收益高于指数收益，不必然证明投资经理有能力；高收益可能只是在承担更多市场或其他系统性风险。

一种示意性定义：

\[
Active\ Return=Portfolio\ Return-Benchmark\ Return
\]

更严格检验异常收益还需要考虑风险模型、交易成本、样本时段和统计显著性。

**例子**：投资经理过去每年都获得比市场基准多 6% 的收益；但如果组合风险显著高于基准、成本高，或业绩只有很短的样本，仍不足以确定存在可复制的异常收益。

### 6.2 Event Study｜事件研究

观察财报、重大公告等**新公开信息**公布前后，证券价格如何以及多快调整。
- 市场若能迅速把公开信息反映进价格，符合半强式有效的典型预期。
- 公告后的持续异常价格漂移可能作为检验市场有效性的线索，但需控制风险、模型和其他信息变化。

### 6.3 Joint-Hypothesis Problem｜联合假设问题

检验“异常收益”时，需要先选定什么收益是对所承担风险的合理补偿。
- 若策略表现似乎异常，究竟是市场不够有效，还是**用于衡量应得收益的风险模型不准确**？
- 因此单独一个策略的过往成功，不足以严格证明 EMH 不成立。

### 6.4 Random Walk｜随机游走

“随机游走”可辅助理解：新信息带来难以事先预测的价格变化，因此单凭过去价格难以稳定预测未来异常收益。

**注意**：弱式有效不必要求所有收益在统计上完全独立、所有波动模式消失；二者不是完全等价的严格命题。

## 7. Market Anomalies and Behavioral Finance｜市场异象与行为金融

### Market Anomalies｜市场异象

历史上识别的一些收益模式可能与简单有效市场假设存在张力，例如：
- **Size Anomaly（规模异象）**：某些历史时期小市值股票表现有异常差异。
- **January Effect（1月效应）**：历史上某些股票在一月份表现较突出；年末税损出售（Tax-Loss Selling）是一种解释。
- **Momentum / Winners–Losers Anomalies（动量／赢家—输家异象）**：历史赢家或输家可能呈现某种延续或反转模式。

**考点**：观察到 Anomaly 不等于它一定会重复，也不等于扣除费用、承担风险后能盈利。可能与数据挖掘、样本选择或风险补偿有关。

### Behavioral Finance｜行为金融学

研究投资者的认知与情绪偏差，如：
- Overconfidence（过度自信）：高估自己的判断和信息处理能力；
- Loss Aversion（损失厌恶）：同等损失的痛苦强于收益快乐；
- Herding / Information Cascades（羊群行为／信息瀑布效应）：受到他人行动影响。

**CFA 特别提醒**：即使个体投资者存在不理性行为，市场依然**可能**有效，因为其他投资者可能利用价格偏差进行交易。行为偏差不等于市场必然无效。

## 8. Two Typical CFA Questions｜已做典型题

### Question A：技术分析模型连续获利

> Dheeraj makes investment decisions using a complex technical analysis model and earned approximately 6% excess return every year in the past. The market is most likely:

A. Weak-form efficient  
B. Semi-strong-form efficient  
C. Weak-form inefficient

**考试答案：C. Weak-Form Inefficient。**

理由：Technical Analysis 主要使用过去价格、成交量等历史交易信息；若仅凭这些数据可以持续得到风险调整后的超额收益，不符合弱式有效的基本预期。既然不能满足弱式要求，也不能归为半强式有效。

**现实中的谨慎判断**：历史收益还需要经过风险调整、成本、统计显著性及样本外检验。

### Question B：资本限制阻止投资者参与

> Capital restrictions prevent some investors from participating in the financial market. This most likely:

A. Does not affect market efficiency  
B. Enhances market efficiency  
C. Impedes market efficiency

**考试答案：C. Impedes Market Efficiency。**

限制有效参与可能弱化竞争、信息传播和错误定价修正。

## 9. Common Exam Traps｜易错点归纳

1. **半强式有效包含弱式有效**：不能因为某技术策略能持续获利就选择“半强式有效”。
2. **Weak-Form 只否定历史交易信息的独立优势**：不代表基本面分析在所有情形下都无效。
3. **Strong-Form 不仅是公开财报**：还要包括 Private / Nonpublic Information。
4. **Positive Return ≠ Abnormal Return**：赚钱不等于战胜适当风险基准。
5. **Outperformance in the Past ≠ Proven Inefficiency**：历史表现可能来自风险、成本口径、运气或模型问题。
6. **Efficient ≠ Price Never Changes**：价格会根据新信息迅速调整。
7. **Anomaly ≠ Guaranteed Profit**：市场异象可能不稳定或无法交易获利。
8. **Behavioral Bias ≠ Market Must Be Inefficient**：行为偏差可能被其他市场参与者的交易抵消。

## 10. Self-Test｜自测题

**Q1**：投资者利用历史价格和成交量持续获得风险调整后的异常收益。最直接与哪种有效性冲突？  
**A1**：Weak-Form Efficiency（弱式有效）。

**Q2**：公司发布公开财报，部分投资者能够在公告后很长时间仅靠该公开信息系统性盈利。最直接与哪种有效性冲突？  
**A2**：Semi-Strong-Form Efficiency（半强式有效）。

**Q3**：若 Strong-Form Efficiency 成立，Semi-Strong-Form Efficiency 是否必然成立？  
**A3**：是。信息集合具有包含关系。

**Q4**：投资经理过去连续三年战胜市场，是否足以证明市场无效？  
**A4**：不足以。需要风险调整、成本、统计显著性及样本外检验。

**Q5**：限制部分投资者进入市场，对市场有效性通常有什么影响？  
**A5**：可能阻碍 Price Discovery，从而 Impede Market Efficiency。

## 11. One-Page Revision｜考前速查

| 关键词 | 应想到的答案 |
|---|---|
| Historical Prices / Technical Analysis | Weak-Form |
| Public Financial Statements / Earnings Announcement | Semi-Strong-Form |
| Private / Inside Information | Strong-Form |
| Persistent Risk-Adjusted Technical Alpha | Weak-Form Inefficient |
| Capital Restrictions / Barriers to Entry | Impeded Market Efficiency |
| Price vs Estimated Fundamental Value | Market Value vs Intrinsic Value |
| Passive vs Active | Efficient Market → Active Alpha Harder |
| January / Size / Winners–Losers | Market Anomalies |
| Overconfidence / Herding | Behavioral Finance |

**最终口诀：弱式看历史，半强看公开，强式看全部；能稳定从旧信息里获利，就要质疑相应有效性。**

## Sources｜学习依据

1. CFA Institute (2026), [Market Efficiency, CFA Level I Equity Investments](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/market-efficiency)（官方公开课程摘要与 LOS）。
2. CFA Institute (2026), [Equity Valuation: Concepts and Basic Tools](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/equity-valuation-concepts-basic-tools)（技术分析与基本面分析的差别）。
3. CFA Institute Research Foundation, [Identifying Skilled Active Managers](https://rpc.cfainstitute.org/sites/default/files/-/media/documents/book/rf-publication/2013/rf-v2013-n4-1-pdf.pdf)（有效性分类与区分偶然收益和技能的背景）。
