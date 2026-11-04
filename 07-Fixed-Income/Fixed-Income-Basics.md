---
subject: CFA Level I
topic: Fixed Income Fundamentals
status: 持续更新
tags: [CFA-L1, Fixed-Income, Fundamentals]
---

# Fixed Income Basics｜固定收益基础概念

本文件集中记录固定收益（Fixed Income）中的基础术语、定义与简单计算。复杂模型和专项考点另设独立笔记。

## 1. 债券期限相关概念

### Tenor｜剩余期限

- **定义**：从当前时点到债券到期日（Maturity Date）剩余的时间。
- **计算**：

\[
Tenor = Original\ Maturity - Elapsed\ Time
\]

- **例题**：一只10年期债券在3年前发行，则当前 Tenor 为：

\[
10-3=7\text{ years}
\]

### Original Maturity｜原始期限

- **定义**：债券发行日（Issue Date）至到期日之间的总期限。
- 本例中，Original Maturity = 10 years。

### Elapsed Time｜已过去时间

- **定义**：从债券发行日至当前时点已经经过的时间。
- 本例中，Elapsed Time = 3 years。

### Maturity Date｜到期日

- **定义**：债券合同约定偿还本金的日期。
- Tenor 衡量当前距离该日期还有多长时间。

### 易混淆点

| 概念 | 含义 | 本题数值 |
|---|---|---:|
| Original Maturity | 发行时确定的总期限 | 10年 |
| Elapsed Time | 已经过的时间 | 3年 |
| Tenor / Time to Maturity | 当前剩余期限 | 7年 |

## 2. 债券基本要素

### Par Value / Face Value｜面值

- **定义**：债券合同约定的本金金额，通常也是到期偿还的本金。
- 本例中 Par Value = $100。

### Coupon Rate｜票面利率

- **定义**：用于计算债券票息的年利率，通常以面值为计算基础。
- **年度票息公式**：

\[
Annual\ Coupon = Par\ Value \times Coupon\ Rate
\]

- 本例中年度票息为：

\[
100\times4\%=\$4
\]

- 注意：Coupon Rate 不等于 Yield（收益率）；票面利率以面值计算，而收益率反映债券价格与现金流之间的回报关系。

## 3. 债券发行主体分类

债券可根据发行主体（Issuer）进行分类。做题时首先识别是谁发行债券，而不是只看债券名称或是否有政府支持。

### Sovereign Bond｜主权债券

- **发行主体**：国家中央政府（National Government）。
- **含义**：由一个国家的主权政府发行的债券。
- **例子**：美国国债（U.S. Treasury Securities）、中国国债、日本国债。
- **识别关键词**：National Government / Central Government。

### Supranational Bond｜超国家机构债券

- **发行主体**：由多个国家共同建立或支持的国际机构（Supranational Organization）。
- **含义**：由跨国或超国家机构发行，而不是由某一个国家的中央政府直接发行。
- **例子**：世界银行（World Bank）、欧洲投资银行（European Investment Bank）。
- **识别关键词**：International Organization / Multiple Countries。

### Quasi-government Bond｜准政府债券

- **发行主体**：与政府有密切联系、具有政府支持背景的机构或政府关联实体（Government-related Entity）。
- **含义**：发行人并非国家中央政府本身，但与政府存在制度、所有权或支持关系。
- **例子**：美国政府支持企业（Government-Sponsored Enterprises, GSEs）发行的相关债券。
- **识别关键词**：Government-related Agency / Government-sponsored Entity。

### 三类债券对比

| 债券类型 | 发行主体 | 判断关键词 |
|---|---|---|
| Sovereign Bond | 国家中央政府 | National Government |
| Supranational Bond | 多国共同建立的国际机构 | International Organization |
| Quasi-government Bond | 政府关联机构或实体 | Government-related Entity |

**考试判断顺序：**
1. 国家中央政府直接发行 → Sovereign Bond。
2. 多国共同建立的国际机构发行 → Supranational Bond。
3. 政府关联机构发行，但发行人不是中央政府 → Quasi-government Bond。

### Corporate Bond｜公司债券

- **发行主体**：公司或其他商业企业（Corporation / Company）。
- **含义**：由企业为经营、投资或再融资等目的发行的债券。
- **例子**：Apple 公司发行的债券。
- **识别关键词**：Corporation / Company / Corporate Issuer。

### 按信用质量分类｜Credit Quality Classification

与按发行主体分类不同，信用质量分类关注发行人按时偿付本金和利息的能力，以及债券的违约风险。

#### Investment-Grade Bond｜投资级债券

- **含义**：信用评级达到投资级门槛的债券，通常被认为信用风险相对较低。
- **评级门槛**：
  - S&P：BBB− 及以上。
  - Moody's：Baa3 及以上。

#### Speculative-Grade Bond / Junk Bond｜投机级债券／垃圾债券

- **含义**：信用评级低于投资级门槛的债券，通常具有较高信用风险。
- **其他名称**：High-Yield Bond（高收益债券）。
- **注意**：高收益是对较高信用风险所要求的收益补偿，并不代表投资一定能获得更高的实际回报。
- **评级门槛**：
  - S&P：低于 BBB−。
  - Moody's：低于 Baa3。

### 两种分类维度不要混淆

| 分类依据 | 债券类别 | 判断问题 |
|---|---|---|
| 发行主体（Issuer） | Government Bond、Sovereign Bond、Supranational Bond、Quasi-government Bond、Corporate Bond | 谁发行了债券？ |
| 信用质量（Credit Quality） | Investment-Grade Bond、Speculative-Grade / Junk Bond | 发行人的偿债信用如何？ |

**同一只债券可以同时拥有不同维度的标签。** 例如，美国政府发行的债券属于 Government / Sovereign Bond（按发行主体分类），同时也可以被评为 Investment-Grade Bond（按信用质量分类）。

**考试识别：**
- Investment-Grade / Junk / High-Yield → 按信用质量分类。
- Government / Corporate / Municipal → 主要按发行主体分类。
- 题目问“哪一种不是根据信用质量命名”，Government Bond 是按发行主体命名。

## 4. 国际债券与市政债券

本节介绍 Foreign Bond、Eurobond 与 Municipal Bond。前两者主要按发行市场、发行人所在地及计价货币的关系分类；Municipal Bond 则主要按发行主体分类，二者不是完全相同的分类维度。

### Foreign Bond｜外国债券

- **定义**：外国发行人在某一国家的国内债券市场发行，并以该国本币计价的债券。
- **识别要素**：
  1. 发行人（Issuer）来自发行市场所在国以外。
  2. 在该国国内市场发行（Domestic Market）。
  3. 以该国本币（Local Currency）计价。
- **例子**：中国企业在美国国内市场发行美元债券。
- **典型名称**：
  - **Yankee Bond（扬基债券）**：外国发行人在美国发行的美元债券。
  - **Samurai Bond（武士债券）**：外国发行人在日本发行的日元债券。

### Eurobond｜欧洲债券／国际债券

- **定义**：以某种货币计价，但在该货币所属国以外的市场发行的债券。
- **识别要素**：发行市场位于计价货币所属国之外（Outside the Currency's Home Country）。
- **例子**：中国企业在伦敦发行美元债券；日本企业在伦敦发行日元债券。
- **注意**：
  - Eurobond 不要求在欧洲发行。
  - Eurobond 不要求以欧元（EUR）计价。
  - 名称中的 Euro 是历史形成的国际债券市场术语，不等同于 Euro Currency（欧元）。

### Municipal Bond｜市政债券

- **定义**：由地方政府（Local Government / Municipality）或符合相关市场定义的地方公共实体发行的债券。
- **常见用途**：道路、学校、医院、公共交通、供水及其他公共基础设施融资。
- **美国市场补充**：部分市政债券的利息可能享有联邦所得税优惠（Tax-Exempt Interest），但并非所有市政债券都免税，具体取决于债券类型及适用税法。
- **识别关键词**：Local Government、Municipality、Public Infrastructure。

### 三类概念对比

| 概念 | 主要分类依据 | 发行人 | 发行地点与货币关系 |
|---|---|---|---|
| Foreign Bond | 外国发行人进入当地国内债券市场 | 发行市场所在国以外的发行人 | 在当地市场发行，并以当地本币计价 |
| Eurobond | 发行市场与计价货币所属国的关系 | 可以来自不同国家或机构 | 在计价货币所属国以外的市场发行 |
| Municipal Bond | 发行主体 | 地方政府或地方公共实体 | 不由发行地点与货币关系定义 |

**重要区别**：Foreign Bond 与 Eurobond 是跨境债券发行安排的分类；Municipal Bond 是按发行主体分类。因此，Municipal Bond 与前两者并非严格互斥的类别。

### 考试识别方法

- Foreign issuer + domestic market + local currency → **Foreign Bond**。
- Issued outside the home country of the currency → **Eurobond**。
- Local government / municipality / public infrastructure → **Municipal Bond**。

## 5. Principal Repayment Structures｜债券本金偿还方式

本节按照债券本金（Principal）在存续期间及到期日的偿还安排，区分 Bullet Bond、Partially Amortizing Bond 与 Fully Amortizing Bond。

### Bullet Bond｜到期一次还本债券

- **定义**：债券存续期间不分期偿还本金，全部本金在到期日（Maturity Date）一次性偿还。
- **识别特征**：No principal repayment before maturity；full principal repaid at maturity。
- **例子**：本金为 1,000,000 美元，存续期间不偿还本金，到期日一次偿还 1,000,000 美元。

### Partially Amortizing Bond｜部分摊还债券

- **定义**：债券存续期间分期偿还部分本金，到期日仍有未偿还本金，需要支付剩余本金。
- **识别特征**：部分本金在存续期间偿还，剩余本金在到期日偿还。
- **Balloon Payment（气球式付款／到期大额尾款）**：到期时集中偿还的剩余本金。
- **例子**：本金为 1,000,000 美元，存续期间偿还 600,000 美元，到期日偿还剩余 400,000 美元。

### Fully Amortizing Bond｜完全摊还债券

- **定义**：本金通过存续期间的定期付款逐步全部偿还；到期时本金余额为零。
- **识别特征**：Scheduled payments fully amortize the principal by maturity。
- **例子**：本金为 1,000,000 美元，通过多期还款逐步偿还全部本金，到期时不再有剩余本金。

### 三种债券对比

| 债券类型 | 存续期间本金偿还 | 到期日偿还 | 到期时本金余额 |
|---|---|---|---|
| Bullet Bond | 不分期偿还本金 | 一次偿还全部本金 | 到期前保持全部本金 |
| Partially Amortizing Bond | 偿还部分本金 | 偿还剩余本金（Balloon Payment） | 大于 0 |
| Fully Amortizing Bond | 分期偿还全部本金 | 如有最后一期付款则结清 | 0 |

### 本题考点

题干给出面值（Par Value）为 10,000,000 美元，其中 60% 的本金在到期日偿还。按题目所考查的部分摊还结构理解，剩余 40% 已在债券存续期间偿还：

\[
Principal\ repaid\ at\ maturity=10,000,000\times60\%=6,000,000
\]

\[
Principal\ amortized\ before\ maturity=10,000,000\times40\%=4,000,000
\]

因此，到期日仍有本金需要偿还，但并非全部本金都留到到期日，也不是全部本金都已摊还完毕，属于 **Partially Amortizing Bond**。

**考试速记：**
- 全部本金到期一次偿还 → Bullet Bond。
- 部分本金提前摊还，剩余本金到期偿还 → Partially Amortizing Bond。
- 全部本金在到期前／到期时通过分期付款摊还完毕 → Fully Amortizing Bond。

## 6. 做题提醒

- 题目问 **Tenor** 或剩余到期时间时，先判断债券已经发行多久，再用原始期限减去已过去时间。
- 面值（Par Value）和票面利率（Coupon Rate）通常不是计算 Tenor 所必需的数据；若题目只问期限，不要被无关数据干扰。


## 7. Sinking Fund｜偿债基金

### Sinking Fund Arrangement（偿债基金安排）

发行人依据债券契约逐步偿还部分债券本金，或积累用于偿还债券的资金。偿债方式可能包括按计划赎回部分债券或在二级市场购回债券。

### Sinking Fund 对信用风险的影响

- 偿债基金安排使发行人在债券到期前逐步偿还或购回部分债券，因此 **Outstanding Principal（未偿还本金）** 会下降。
- 未偿还债务规模下降，债权人的本金风险敞口（Exposure）通常随之下降，也减轻发行人到期集中偿债的压力。
- 需要区分：这并不必然意味着发行人发生违约的概率（Probability of Default）下降；更准确地说，是未偿本金及潜在损失敞口降低。
- 投资者可能因此面临提前收回本金后的再投资风险（Reinvestment Risk）。


- **Default Risk（违约风险）**：逐步偿债通常减轻最终到期时集中偿还本金的压力。
- **Reinvestment Risk（再投资风险）**：若债券持有人提前收回本金，而市场利率已经下降，可能只能以较低收益率重新投资。
- 利率下降不意味着每位持有人的本金一定提前返还，具体由偿债基金条款决定。

### Callable Bond 与 Sinking Fund Bond 对比

| 项目 | Callable Bond | Sinking Fund Bond |
|---|---|---|
| 机制 | 发行人按赎回条款可提前赎回 | 按合同安排逐步偿还／购回 |
| 主要目的 | 发行人提前赎回的灵活性 | 分散集中偿债压力 |
| 对投资者 | 提前收回本金可能增加再投资风险 | 提前收回本金同样可能增加再投资风险 |

### 本题考点

市场利率下降时，设有 Sinking Fund 的债券持有人可能面临更高的 **Reinvestment Risk**，因为本金若被提前偿还，就可能需要以更低利率再投资。

**Prefer their bonds to be repaid**：更希望所持债券被偿还。
- **prefer + 名词 + to be + 过去分词**：希望某物被……。
- **repay**：偿还；**be repaid**：被偿还。
- 利率下降时，投资者一般更希望继续持有高票息债券，而不是提前收回本金。


## 8. Securitization and Tranche Structure｜证券化与分层结构

### Securitization｜资产证券化

- **定义**：将贷款、应收款等资产汇集并以其产生的现金流为基础发行证券的融资安排。
- 资产证券化产品可能根据不同的偿付优先级和风险承担顺序划分为多个分层（Tranches）。

### Tranche｜分层

- **定义**：资产证券化交易中，按照现金流分配顺序、损失承担顺序及风险特征划分的证券层级。
- 不同 Tranche 对底层资产现金流和信用损失承担的优先级不同。

### Waterfall Structure｜现金流瀑布结构

- **定义**：按照合同约定的优先顺序分配底层资产产生的现金流，并按约定顺序分配损失。
- **现金流分配（Payment Priority）**：通常先支付 Senior Tranche，再支付 Mezzanine Tranche，最后支付 Junior / Equity Tranche。
- **损失承担（Loss Allocation）**：通常先由 Junior / Equity Tranche 承担损失，再依次影响 Mezzanine，最后才影响 Senior。
- 具体分配和损失顺序以证券化交易文件为准。

### 三种常见 Tranche

| Tranche | 中文 | 现金流偿付优先级 | 通常信用风险 |
|---|---|---|---|
| Senior Tranche | 优先级分层 | 最高 | 最低 |
| Mezzanine Tranche | 夹层 | 中间 | 中等 |
| Junior / Equity Tranche | 劣后级／权益级 | 最低 | 最高 |

### 本题考点

- **Statement 1：正确。** Sinking Fund Arrangement 在到期前逐步减少 Outstanding Principal，降低未偿债务规模及债权人的本金风险敞口，并缓解到期集中偿债压力。
- **Statement 2：错误。** Higher-ranked tranche（较高优先级分层）通常拥有更高的现金流偿付优先级，并在损失分配中受到更多保护，因此其信用风险通常较低，而不是较高。
- **考试速记**：
  - Senior：先收现金流、后承担损失 → 风险较低。
  - Junior：后收现金流、先承担损失 → 风险较高。
  - Waterfall：现金流从 Senior 向 Junior 分配；损失通常从 Junior 向 Senior 传递。


## 9. Distressed Debt｜困境债务

### Distressed Debt（困境债务）

- **定义**：由陷入严重财务困境、违约或面临较高违约风险的发行人所发行或尚未偿还的债务工具，通常以显著折价交易。
- **投资方式**：投资者（包括 Hedge Fund，对冲基金）可能低价购入困境债务，期待企业经营恢复、债务重组（Debt Restructuring）或债权回收价值提升。
- **Equity-like Return（类股权收益）**：由于买入价格很低且结果高度不确定，债券价格可能产生大幅涨跌，收益风险特征可能类似股权；这**不表示困境债务本身就是股票**。
- **Priority of Claims（清偿顺序）**：债权通常在普通股之前受偿，但具体回收金额取决于担保、债权优先级、破产程序与资产价值。
- **风险**：违约、重组失败和本金大幅损失均可能发生。低价不等于便宜或安全。

### 考试识别

题目：Hedge fund seeks equity-like returns from a deeply distressed company.

- CFA 此类语境中重点识别 **Distressed Debt（困境债务）**：对冲基金可能以很低价格购买高风险债权，追求重组或恢复带来的高回报。
- 困境公司的股票也可能交易并有波动，但题目考查的典型策略是购买困境债务，而不是仅因出现 equity-like 就选择 Stocks。
- **速记：Distressed Debt = Debt Instrument + Potential Equity-like Return + High Risk。**


## 10. Bond Issuance Methods｜债券发行方式

### Shelf Registration｜储架注册

- **定义**：发行人一次办理符合适用法规的发行注册／披露安排，在允许的期限与额度内，根据融资需要分次发行证券。
- **核心特征**：Single Registration / Single Offering Circular（一次注册／统一发行说明资料） + Multiple Issues（分批发行）。
- **优势**：发行时间安排更灵活（Flexibility）、可以配合融资需求与市场环境、减少重复注册成本。
- **注意**：分批发行不代表后续每期完全不需要补充披露；具体以适用监管规则为准。

### Syndicated Offering｜承销团发行

- **定义**：多家承销商（Underwriters）组成承销团（Underwriting Syndicate），共同协助发行人承销和分销债券。
- **核心关键词**：Multiple Underwriters（多个承销商）。
- 主要描述**承销组织方式**，不是注册批次。

### Auction｜拍卖发行

- **定义**：投资者通过提交竞价（Bids）参与债券发行，按拍卖规则确定价格／收益率与配售。
- **核心关键词**：Bidding / Competitive Auction（竞价）。
- 主要描述**定价与配售方式**。

### 对比与考试识别

| 发行方式 | 主要关注点 | 题目关键词 |
|---|---|---|
| Shelf Registration | 一次注册，按需要分批发行 | Single Circular + Series of Bonds |
| Syndicated Offering | 多家承销商合作 | Underwriting Syndicate |
| Auction | 通过竞价确定发行条件 | Bids / Auction |

三者不一定互斥：注册安排、承销组织方式、定价配售方式属于不同维度。

**本题**：Golden Finance 使用一份统一的发行说明资料，随后按需分批发行债券。正确答案为 **A. Shelf Registration**。


## 9. Bond Indexes and Equity Indexes｜债券指数与股票指数

### Equity Index｜股票指数

- **定义**：按照一套既定规则选取一组股票作为成分证券（Constituents），并通过特定计算方法衡量这组股票或某一股票市场表现的指标。
- **作用**：反映特定市场、市场板块或股票组合的整体表现，也可作为投资组合业绩比较基准（Benchmark）。
- **例子**：S&P 500、NASDAQ Composite、沪深300指数。

### Broad Equity Index｜广泛股票指数／宽基股票指数

- **定义**：覆盖范围较广、代表较广泛股票市场或市场主要部分的股票指数，而不是只跟踪单一行业或主题。
- **与 Sector Index 的区别**：Sector Index（行业指数）集中于特定行业；Broad Equity Index 的覆盖范围通常更广。
- **例子**：S&P 500、沪深300指数。

### Bond Index｜债券指数

- **定义**：按照既定规则选取一组债券作为成分证券，并衡量其价格、收益或总回报表现的指数。
- **作用**：衡量债券市场或特定债券市场细分领域的表现，也可作为债券投资组合的业绩基准。

### Broad Bond Index｜广泛债券指数

- **定义**：覆盖较广泛债券市场或多个债券类别的债券指数，而非只追踪单一债券类别或期限区间。
- **特点**：通常包含大量不同发行人、期限、票息和信用特征的债券。

### Index Constituents｜指数成分证券

- **定义**：按照指数编制规则被纳入指数的证券。
- 股票指数的 Constituents 是股票；债券指数的 Constituents 是债券。
- 指数成分数量（Number of Constituents）本身不能说明指数更容易复制；成分数量更多通常意味着需要处理更多证券，但复制难度还取决于流动性、可交易性、证券特征及指数规则。

### Index Turnover｜指数换手率／成分周转

- **定义**：衡量指数成分证券在一定期间内被替换或调整的程度。
- **债券指数的换手率通常高于广泛股票指数**，主要原因包括：
  1. **Maturity（到期）**：债券到期后不再是存续证券，通常需要从指数中移除。
  2. **New Issuance（新发行）**：符合纳入规则的新债券可能进入指数。
  3. **Credit Rating Changes（信用评级变化）**：评级变化可能导致债券不再符合特定指数的资格要求。
  4. 其他指数纳入、剔除及再平衡规则也会引起成分变化。
- 股票指数也会因公司行动、退市及定期调整而换手，但股票本身没有固定到期日。

### Index Replication｜指数复制

- **定义**：通过持有指数中的全部或部分成分证券，或采用其他复制方法，使投资组合尽可能跟踪指数表现。
- **债券指数通常比广泛股票指数更难进行完整复制（Full Replication）**，原因包括：
  1. **Large Number of Constituents（成分数量庞大）**：广泛债券指数可能包含大量债券。
  2. **Lower Liquidity（流动性较低）**：部分债券交易不活跃，可能难以买入或卖出。
  3. **Heterogeneity（异质性）**：债券在期限、票息、信用评级、偿付优先级等方面存在差异。
  4. **OTC Trading（场外交易）**：债券大量通过场外市场交易，报价和交易可得性可能不如集中交易的股票透明、连续。
- **重要辨析**：债券指数成分数量更多，不代表更容易复制；大量成分证券和较低流动性通常会增加完整复制的复杂度。

### Over-the-Counter (OTC)｜场外交易

- **定义**：交易双方通过交易商网络或其他场外安排直接协商成交，而不是在集中交易所内撮合交易。
- **债券市场特征**：许多债券在 OTC 市场交易，单只债券的交易活跃度可能不同，价格信息和交易可得性也可能存在差异。
- **对指数复制的影响**：可能增加交易成本、搜寻证券和维持指数权重的难度。

### Bond Index 与 Equity Index 对比

| 对比维度 | Broad Bond Index | Broad Equity Index |
|---|---|---|
| 成分证券 | 债券 | 股票 |
| 成分数量 | 通常更多 | 通常相对较少 |
| 成分换手率 | 通常较高 | 通常较低 |
| 固定到期日 | 多数债券有 | 股票没有固定到期日 |
| 交易方式 | 大量通过 OTC 市场 | 通常在交易所集中交易 |
| 完整复制难度 | 通常较高 | 通常较低 |

### 本题考点

- **Statement 1：正确。** Broad Bond Index 通常比 Broad Equity Index 有更高的 turnover，债券到期、新债发行及评级变化等都会推动指数成分调整。
- **Statement 2：错误。** 债券指数通常更难复制。成分数量多并不会使复制更容易；债券数量庞大、流动性较低、证券异质性及 OTC 交易等因素会增加复制难度。
- **考试速记**：
  - Bond Index：通常 turnover 更高。
  - Bond Index：通常 replication 更难。
