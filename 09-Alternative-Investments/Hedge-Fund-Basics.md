---
subject: Alternative Investments
topic: Hedge Fund Basics
status: "🟢 FOF 优缺点单题独立答对；其余基础知识待验证"
created: 2026-11-14
last-reviewed: 2026-11-14
tags: [CFA-L1, Alternative-Investments, Hedge-Funds, Fund-of-Funds, Strategies, Due-Diligence]
---

# 对冲基金基础知识（Hedge Fund Basics）

[[09-Alternative-Investments/INDEX|返回另类投资目录]]

## 一句话理解

**Hedge Fund（对冲基金）**是以较灵活的投资策略争取投资目标的集合投资工具，通常依赖主动管理（Active Management），可能运用多空交易、衍生品和杠杆。**Fund of Hedge Funds (FoHF，对冲基金中的基金)**通过配置多只底层对冲基金，提供专业筛选和一定的分散化机会，但通常承担双层收费。

## AUM、NAV 与承诺资本（AUM, NAV and Committed Capital）

### AUM 是什么？

**Assets Under Management (AUM)｜管理资产规模**：投资管理机构或基金所管理资产的总价值，通常会随资产市场价值变化、投资者申购和赎回而变化。它是**所管理的资产**，不是基金经理的个人财富。

**重要口径限制**：AUM 的统计方法因管理机构、产品及披露口径而异，可能采用总资产或净资产等口径；**不能在没有题目或合同定义时，认定 AUM 一定等于总资产或 NAV**。

### AUM 与 NAV 的区别

- **Gross Assets｜总资产**：基金所持资产的价值。
- **Liabilities｜负债**：借款及其他应付款项。
- **Net Asset Value (NAV)｜资产净值**：总资产扣除负债后的净额。

$
NAV=\text{Gross Assets}-\text{Liabilities}
$

简化例子：资产总值为 150、负债为 50，则 NAV 为 100（同一货币单位）。若 AUM 采用总资产口径可为 150，采用净资产口径则可能为 100；**实际应以披露口径和题干为准**。

### AUM 与管理费（Management Fee）

若合同约定以某一时点的 AUM 作为计费基数：

$
\text{Management Fee}=\text{Specified AUM Base}\times m
$

其中 $m$ 为管理费率。常见计费基数包括：

- **Beginning AUM｜期初管理资产规模**
- **Year-end / Ending AUM｜期末管理资产规模**
- **Average AUM｜平均管理资产规模**

**考试陷阱**：不要看到 AUM 就固定使用期末值；需根据题干确定时点、口径和费用扣除前后状态。

### AUM 与 Committed Capital（承诺资本）

| 对比 | AUM | Committed Capital |
| --- | --- | --- |
| 中文 | 管理资产规模 | 承诺资本 |
| 本质 | 所管理资产的价值 | 投资者承诺未来投入的资本 |
| 典型应用 | 对冲基金管理费常按 AUM 计算 | 私募股权基金投资期管理费常按承诺资本计算 |
| 是否等于实缴金额 | 不一定 | 不一定 |

- **Called Capital｜已调用资本**：基金根据承诺向投资者要求缴纳的金额；实际已缴款金额须看题目定义。
- **Uncalled Capital｜未调用资本**：尚未调用的承诺资金。
- 简化情形下：$\text{Committed Capital}=\text{Called Capital}+\text{Uncalled Capital}$。
- 私募股权基金进入投资期后续阶段，管理费基数可能改为已投资资本或其他合同约定基数。

**记忆：AUM 看管理资产的价值；Committed Capital 看承诺投入的资金。**

## 对冲基金的主要特点

- **Active Management｜主动管理**：管理人主动选择证券、市场敞口或交易策略，通常寻求正的超额风险调整后收益（Positive Alpha），但不保证实现。
- **Investment Flexibility｜投资策略灵活性**：部分对冲基金可使用卖空（Short Selling）、杠杆（Leverage）和衍生品（Derivatives）；实际受到基金文件及监管限制。
- **Absolute Return Objective｜绝对收益目标**：一些对冲基金强调在不同市场环境中争取正回报，但不能把目标理解为保本或保证正收益。
- **Liquidity and Transparency｜流动性与透明度**：基金份额可能存在锁定期、赎回限制及较少公开披露；各基金差异很大。
- **Manager Dependence｜管理人依赖**：策略执行、风险管理和运营能力可能显著影响结果。

## 常见投资策略（Hedge Fund Strategies）

| 策略 | 英文 | 核心思路 |
| --- | --- | --- |
| 多空策略 | Long/Short | 买入预期表现较好的资产，同时卖空预期表现较差的资产；不代表一定市场中性 |
| 事件驱动 | Event-Driven | 围绕并购、重组、破产等企业事件寻找机会 |
| 套利策略 | Arbitrage | 利用相关资产之间的相对定价差异，仍可能承担基差、流动性和执行风险 |

**边界**：这是一份入门速记，不代表完整的 CFA 对冲基金策略分类；后续遇到专门策略题再补充。

### 事件驱动与基本面价值策略（Event-Driven vs. Fundamental Value）

本题题库将 **Distressed Securities（困境证券）** 与 **Merger Arbitrage（并购套利）** 归入 **Event-Driven（事件驱动）**，而将 **Fundamental Value（基本面价值）** 归入 **Equity Hedge（权益对冲）**。关键在于投资机会主要由**特定企业事件**还是**基本面估值差异**驱动。

| 子策略 | 所属典型类别 | 核心收益驱动 |
| --- | --- | --- |
| Distressed Securities（困境证券） | Event-Driven（事件驱动） | 企业破产、债务重组及证券回收价值变化 |
| Merger Arbitrage（并购套利） | Event-Driven（事件驱动） | 并购完成概率、收购价格与当前证券价格的差异 |
| Fundamental Value（基本面价值） | Equity Hedge（权益对冲） | 盈利、现金流、资产质量与估计内在价值的偏离 |

**Distressed Securities｜困境证券策略**：关注陷入财务困难（Financial Distress）、可能违约或进行债务重组（Debt Restructuring）的企业证券。投资结果受重组结果、清偿顺序、回收率（Recovery Rate）等影响；低价买入不保证盈利。

**Merger Arbitrage｜并购套利**：关注并购公告后交易标的价格与约定收购条件之间的差异。现金收购中，目标公司股票可能低于收购价，价差反映时间、融资、监管审批与交易失败风险（Deal Risk）等；**并购套利不是无风险套利**。

**Fundamental Value｜基本面价值策略**：分析财务报表、盈利、现金流和内在价值（Intrinsic Value），寻找估值偏差；并不必须等待并购、破产等特定企业事件，因此在本题分类中不属于 Event-Driven。

#### CFA 判断口诀

- **Bankruptcy / Restructuring → Distressed Securities → Event-Driven**
- **Merger / Acquisition → Merger Arbitrage → Event-Driven**
- **Earnings / Cash Flow / Intrinsic Value → Fundamental Value → Equity Hedge**

**分类边界**：实际基金可能同时采用多种策略，且不同数据提供商的分类略有差异；本小节保留题库的分类框架，不把策略标签理解为互斥的法律定义。

**复习记录**：本次能够独立判断 Fundamental Value 不属于典型 Event-Driven 策略，🟢 单题独立答对，待变式验证。

## Fund of Hedge Funds（FoHF）是什么？

- **Single Hedge Fund｜单只对冲基金**：投资者直接持有单只基金权益，回报与该基金的策略和管理人相关。
- **Fund of Hedge Funds｜对冲基金中的基金**：上层基金募集投资者资金，并将其配置到多个底层对冲基金（Underlying Funds）。
- 通过 FOF，投资者可以获得多基金投资敞口，但实际分散化效果取决于底层策略是否具有不同风险来源。

## Master-Feeder Structure（主从基金结构）

### 一句话理解

**Master-Feeder Structure｜主从基金结构**：不同类别或不同司法管辖区的投资者通过各自的从基金（Feeder Fund）投入资金，再汇集到同一个主基金（Master Fund），由主基金统一执行投资策略。典型优势是**汇集资金、形成规模经济，以及针对不同投资者安排适当的法律、税务和运营结构**；它**不保证投资者免税**。

### 核心概念与资金流向

- **Master Fund｜主基金**：汇集各 Feeder Fund 的资金，统一管理和投资。
- **Feeder Fund｜从基金 / 联接基金**：为不同投资者群体募集资金，并将其投入主基金。
- **Onshore Feeder｜在岸从基金**：面向某一司法管辖区内的投资者或按当地法律设立的从基金。
- **Offshore Feeder｜离岸从基金**：在境外司法管辖区设立的从基金。
- **Pooling Funds｜资金汇集**：多个 Feeder 将资金汇总至 Master，由同一投资组合管理。

简化结构：

\`\`\`text
Onshore Investors         Offshore Investors
        |                         |
  Onshore Feeder            Offshore Feeder
        \                         /
         \                       /
                 Master Fund
                     |
             Investment Portfolio
\`\`\`

### 典型优势与边界

1. **Economies of Scale｜规模经济**：在岸和离岸投资者资金汇集后，主基金可集中交易、风控和投资管理，可能减少重复工作；但结构本身也会产生法律、审计和行政费用。
2. **Tax / Operational Structuring｜税务与运营安排灵活性**：不同 Feeder 可以针对不同投资者资格、税务及运营需要设计结构；**税务效率不等于完全免税**。
3. **Regulatory Structuring｜监管架构安排**：题库将“可以避免部分地区性监管限制”视为典型优势。更准确的表述是，合法架构可能帮助投资者在适用规则下获得投资机会、减少不必要的结构障碍，但**不能免除适用法律或违法规避监管**。

### 典型考试陷阱

- **Without Any Tax Liability｜完全没有纳税义务**：绝对化表述；主从基金结构不能保证投资者在其税务居民地或其他相关司法管辖区免税。
- **Taxable Jurisdiction｜应税司法管辖区**：投资者的税收责任仍取决于税法、居民身份、收入性质和基金结构。
- **Do Not Include｜不包括**：反向提问，选择不属于真实或可保证优势的陈述。
- **Onshore vs. Offshore**：描述基金所在或适用的司法管辖区，并非“在岸一定缴税、离岸一定免税”。

### Master-Feeder 与 Fund of Hedge Funds（FoHF）比较

| 维度 | Master-Feeder Structure | Fund of Hedge Funds（FoHF） |
| --- | --- | --- |
| 资金结构 | 多个 Feeder → 同一个 Master | 一个 FoHF → 多只底层基金 |
| 主要目的 | 集中投资管理，适配不同投资者 | 专业尽调、策略配置和分散化 |
| 投资执行 | 通常由 Master 统一执行 | 底层基金可能分别采用不同策略 |
| 费用与风险 | 依具体法律和收费安排而定 | 典型存在双层收费，底层策略可能相关 |

**记忆：Master-Feeder = 多对一；FoHF = 一对多。** 两者都是基金结构，但服务于不同的主要目的。

### 我的错因 / 验证记录

- 本次误选“地区监管要求”相关陈述，未识别 **without any tax liability** 这一绝对化错误。
- 题库判定：资金汇集产生规模经济是优势；通过合适结构适配不同地区监管也是可能优势；**完全免税不是可保证优势**。
- 复习状态：🟡 曾答错，待独立验证。

### 复习检查清单

- [ ] 能画出 Onshore / Offshore Feeder → Master Fund 的资金流向。
- [ ] 能解释 Economies of Scale 的来源及结构成本。
- [ ] 能区分税务效率与完全免税。
- [ ] 能区分合法监管架构安排与违法规避监管。
- [ ] 能说明 Master-Feeder 与 FoHF 的结构区别。

## FoHF 的典型优势（Benefits）

1. **Access for Smaller Investors｜较小投资者的可参与性**：FOF 汇集投资者资金，可能降低单个投资者获得多基金配置所需的最低投资额（Minimum Investment Requirement）；仍受投资者资格和基金条款限制。
2. **Professional Due Diligence｜专业尽职调查**：FOF 管理人对底层基金进行选择、评估及持续监督。
   - **Investment Due Diligence｜投资尽调**：评估策略、历史业绩来源、风险敞口及投资流程。
   - **Operational Due Diligence｜运营尽调**：评估内部控制、估值、托管及运营安排。
3. **Diversification Benefits｜分散化效益**：多管理人、多策略可能降低单一基金特有风险；若底层基金高度同向，则分散效果有限。

## FoHF 的典型缺点（Drawbacks）

- **Double-Layered Fees｜双层收费**：底层基金收取管理费和可能的业绩报酬，上层 FOF 也可能收取相应费用，投资者通常承担更高的总费用。
- **Look-Through Complexity｜穿透分析复杂性**：需要了解底层基金的实际持仓、风险敞口及相关性，透明度可能受限制。
- **Liquidity Mismatch｜流动性错配**：上层基金赎回安排可能与底层基金的锁定期或赎回期限不同。
- **Manager Selection Risk｜管理人选择风险**：即使有尽调，也可能选错基金或低估共同风险。

**核心比较**：相对单只对冲基金，FOF 可能更容易让较小投资者参与，并提供专业尽调和多基金配置；但**Lower Fees（更低费用）不是典型优势**。

## 对冲基金的主要风险（Principal Risks）

- **Leverage Risk｜杠杆风险**：借款或衍生品敞口可能放大损失。
- **Liquidity Risk｜流动性风险**：锁定期、赎回限制或底层资产难以出售。
- **Manager Risk｜管理人风险**：业绩依赖策略判断、执行与风控。
- **Concentration Risk｜集中度风险**：单一策略、资产或共同市场风险可能集中。
- **Valuation and Operational Risks｜估值与运营风险**：部分资产难以定价，运营和内部控制也可能出现问题。

## 对冲基金与私募股权基金的结构比较（Hedge Funds vs. Private Equity Funds）

| 维度 | Hedge Fund | Private Equity Fund |
| --- | --- | --- |
| 法律结构 | 可采用 Partnership（合伙企业） | 也可采用 Partnership（合伙企业） |
| 管理费常见基数 | AUM | 投资期常为 Committed Capital |
| 资金安排 | 通常认购时投入基金 | 通常先承诺，后按 Capital Call 缴款 |
| 常见业绩保护安排 | High-Water Mark（高水位线） | Clawback Provision（收益追回条款） |

- **Partnership｜合伙企业**：两类基金均**可以**采用合伙结构，但并非必须。
- **Clawback Provision｜收益追回条款**：私募股权基金中常见，可能要求 GP 返还此前多分配的 Carried Interest（业绩分成），以符合基金最终利润分配安排。
- **High-Water Mark｜高水位线**：对冲基金常见机制，通常要求净值先超过约定的历史高点，才能再次计提业绩报酬。
- Clawback 并非仅限 PE，HWM 也不是所有对冲基金必备；这是典型对比，而非排他性法律规定。

### 本次易错点

- 曾将 **Hedge Fund Management Fees** 错认为按 **Committed Capital** 计算。
- 修正：对冲基金通常以 **AUM** 为基数；PE 投资期通常以 **Committed Capital** 为基数。**两类基金都可能采用 Partnership 结构**。
- 复习状态：🟡 该跨基金对比题曾答错，待独立验证。

## 与收费专题的分工

- 本笔记解释 **FOF 为什么有优势与缺点**，以及对冲基金的基本概念和策略。
- [[Hedge-Fund-Fee-Structures|对冲基金费用结构]] 专门解释 Management Fee、Incentive Fee、Hard/Soft Hurdle、High-Water Mark，以及 FOF 双层收费的计算顺序。
- [[Leverage-and-Leveraged-Returns|杠杆与杠杆收益率]] 专门解释借款成本和杠杆后的权益收益率公式。
- [[Alternative-Investments-Basics|另类投资基础]] 解释对冲基金与其他另类投资类别的关系。

## 高频英文与考试陷阱

- **Relative to**：相对于，用于比较两类投资。
- **Least Likely**：最不可能，找不符合典型特征的选项。
- **Characterized by**：以……为特征。
- **Accessible**：可参与的；不等于任何投资者都可无条件投资。
- **Conduct Due Diligence**：开展尽职调查；不等于保证盈利。
- **Lower Fees**：对 FOF 来说通常不是相对单只基金的优势。
- **Diversification ≠ No Risk**：多基金分散化不能消除市场共同风险。
- **Hedge Fund ≠ Always Hedged**：名字包含 hedge，不意味着所有风险均已对冲。

## 我的错因 / 验证记录

- FOF 的参与门槛、尽调与费用比较：**已独立答对一次**，能识别双层收费通常导致更高费用。
- 对冲基金策略、其他风险概念：目前主要为基础知识整理，尚未完成独立变式验证。
- 复习状态：🟢 FOF 优缺点单题独立答对；其余基础知识待验证。

## 复习检查清单

- [x] 已独立答对一次 FOF 优缺点判断题。
- [ ] 能不看笔记说明对冲基金的主要策略与风险。
- [ ] 能区分单只对冲基金和 FoHF。
- [ ] 能解释 FoHF 的专业尽调、投资门槛与分散化优势。
- [ ] 能解释为什么 FoHF 通常费用更高。
- [ ] 能区分本笔记与收费专题的内容范围。
