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

### Coupon Rate、Current Yield 与 Yield to Maturity｜三种收益率

**Coupon Rate（票面利率）**：按债券面值计算年度票息的比率。

\[
Coupon\ Rate=\frac{Annual\ Coupon}{Face\ Value}
\]

**Current Yield（当期收益率）**：年度票息除以当前债券市场价格；不考虑到期时面值与买入价格的差额，也不完整考虑货币时间价值。

\[
Current\ Yield=\frac{Annual\ Coupon}{Current\ Bond\ Price}
\]

**Yield to Maturity (YTM，到期收益率)**：使债券约定未来现金流现值等于当前市场价格的折现率。对于每年付息、到期按面值还本的普通债券：

\[
P=\sum_{t=1}^{N}\frac{C}{(1+YTM)^t}+\frac{FV}{(1+YTM)^N}
\]

其中 P 为当前价格、C 为每期票息（每年付息时为年度票息）、FV 为到期面值、N 为剩余期数。若付息频率不同，需相应调整每期收益率与期数。

### Premium / Par / Discount Bonds｜三种债券的收益率关系

| 债券类型 | 债券价格与面值 | 收益率关系 |
|---|---|---|
| Premium Bond（溢价债券） | Price > Par | **Coupon Rate > Current Yield > YTM** |
| Par Bond（平价债券） | Price = Par | **Coupon Rate = Current Yield = YTM** |
| Discount Bond（折价债券） | Price < Par | **Coupon Rate < Current Yield < YTM** |

上述严格不等式适用于有正票息、固定票息、到期按面值还本、无嵌入式期权的普通债券，并按一致年化口径比较；零息债等特殊情况需单独判断。

**原因与记忆**：
- **Premium**：买入价格高于到期偿还面值，持有至到期面临本金价差损失，因此 YTM < Current Yield；又因为市场价格高于面值，所以 Current Yield < Coupon Rate。
- **Par**：买入价格等于面值，因此三种收益率相等。
- **Discount**：买入价格低于到期偿还面值，持有至到期获得本金价差收益，因此 YTM > Current Yield；又因为市场价格低于面值，所以 Current Yield > Coupon Rate。

**例子**：面值 $100、票面利率 8%、当前价格 $110、剩余 5 年、每年付息一次。

- Annual Coupon = $8
- Coupon Rate = 8 / 100 = 8%
- Current Yield = 8 / 110 ≈ 7.27%
- YTM：由 110 = Σ[8 / (1+y)^t]（t=1至5）+ 100/(1+y)^5 求得，约 5.65%

故 **8% > 7.27% > 5.65%**，属于 Premium Bond。

**本题答案 B：Coupon Rate > Current Yield > YTM。**

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

### Non-Sovereign Government Debt｜非主权政府债务

- **定义**：由州、省、市等非中央政府层级的政府主体发行的债务。
- **发行主体**：State Government（州政府）、Provincial Government（省级政府）、Local Government（地方政府）、Municipality（市政政府）等。
- 在美国地方政府债券中，常见的两类是 **General Obligation Bond（一般责任债券）** 与 **Revenue Bond（收益债券）**。

#### Source of Repayment｜偿债来源

- **定义**：发行人用于支付债券利息（Interest）和偿还本金（Principal）的资金来源，回答“钱从哪里来”。
- **Credit Support（信用支持）**：指保障偿债的政府信用、征税权、抵押、担保或其他支持安排，回答“偿债能力有哪些保障”。
- **重要区别**：偿债来源不等于发行主体；地方政府发行的债券不一定由一般税收偿还，应核对具体 Bond Indenture（债券契约）。

#### General Obligation Bond (GO Bond)｜一般责任债券

- **定义**：通常由地方政府以其一般财政资源、整体信用及适用的征税能力支持偿还的债券。
- **典型偿债来源**：Tax Revenues（税收收入）及其他可用的一般财政收入。
- **Full Faith and Credit（全面信用支持）**：通常用于描述发行政府以整体信用及适用的征税权支持债务的承诺；具体范围与法律限制取决于发行条款。

#### Revenue Bond｜收益债券

- **定义**：主要依靠特定项目、公共设施或业务产生的约定收入偿还本息的债券。
- **典型偿债来源**：Project Revenues（项目收入），例如 Toll Revenues（收费公路通行费）、机场收费、供水收费。
- **信用支持**：通常依靠指定收入而非政府一般税收及全面信用支持；实际也可能附有额外担保，应以合同为准。

#### GO Bond 与 Revenue Bond 对比

| 项目 | General Obligation Bond | Revenue Bond |
|---|---|---|
| 主要偿债来源 | 一般财政资源、税收及其他可用收入 | 指定项目或业务收入 |
| 典型信用支持 | 政府整体信用、适用征税权 | 约定的项目收入；可能另有担保 |
| 主要风险分析 | 财政收支、税基和征税能力 | 项目现金流、收费能力及运营成本 |
| 例子 | 地方政府一般责任债 | 收费公路收益债 |

**例子：地方政府建设收费公路。** GO Bond 依合同由政府一般财政资源支持偿债；Revenue Bond 通常主要用该公路的通行费偿债。发行主体相似，但偿债来源和信用支持不同。

**本题判断**：
- A：Local Governments 属于 Non-Sovereign Government Issuers，正确。
- B：GO Bonds 和 Revenue Bonds 是两种常见地方政府债券，正确。
- C：声称 Revenue Bonds 依靠地方政府 Full Faith and Credit 并由 Tax Revenues 偿还，混淆了 GO Bond 和 Revenue Bond 的典型特征，**错误（答案 C）**。

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

### High-Yield vs Investment-Grade｜高收益债与投资级债对比

- **Restrictive Covenants（限制性条款）**：债券契约限制发行人额外举债、分红、出售资产等行为。高收益债信用风险较高，通常设置更多或更严格的债权人保护条款。
- **Equity-like Cash Flows（类股权现金流特征）**：高收益债的实际现金流和投资表现受发行人经营、违约及重组影响较大，可能表现出类股票的高风险；债券仍有约定本息支付义务。
- **Credit Spread Contribution（信用利差贡献）**：高收益债信用利差通常更宽，在总收益率中占比通常更高。直观简化：债券收益率 ≈ 可比基准收益率 + 信用利差。

| 对比 | Investment-Grade | High-Yield |
|---|---|---|
| 信用风险 | 较低 | 较高 |
| 限制性条款 | 通常较少 | 通常更多 |
| 类股权风险特征 | 较弱 | 较强 |
| 信用利差 | 较窄 | 较宽 |
| 信用利差收益贡献 | 通常较小 | 通常较大 |

**本题 EXCEPT**：A 更严格的限制通常成立；B 类股权风险特征通常成立；C 声称高收益债信用利差贡献更低是错误的。答案 C。

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

#### Sovereign Bond Auctions｜主权债券拍卖

政府可通过竞争性投标（Competitive Bids）进行国债发行，按报价排序和发行规模确定中标者及配售数量。

**Single-Price Auction / Uniform-Price Auction（单一价格／统一价格拍卖）**
- 所有中标的竞争性投标按照相同的结算价格（或对应统一中标收益率）成交，通常依据边际中标报价确定。
- 并非所有投标都被接受，仍受发行数量和报价排序约束。

**Multiple-Price Auction / Discriminatory-Price Auction（多价格／差别价格拍卖）**
- 中标投资者按照各自中标报价（或相应收益率）成交。
- 与单一价格拍卖的关键差异是**中标后的结算机制**，并非是否对投标排序。

**Competitive Bid Ranking（竞争性投标排序）**
- 按价格（Bid Price）报价：通常**价格从高到低**排序，先接受高价格投标。
- 按收益率（Bid Yield）报价：通常**收益率从低到高**排序，先接受低收益率投标。
- 排序后依发行规模分配；边际报价处可能出现部分配售（Partial Allocation）。
- **Stop-Out Price / Stop-Out Yield（边际中标价格／收益率）**：最后获配的边际中标报价，通常影响统一价格拍卖的结算价格或收益率。
- **Cost of Funds（融资成本）**：发行人融资所承担的成本。单一价格拍卖不必然提高融资成本或缩小投资者范围；结果取决于竞争程度、市场状况及规则。

| 对比 | Single-Price Auction | Multiple-Price Auction |
|---|---|---|
| 中文 | 统一价格拍卖 | 差别价格拍卖 |
| 中标者结算价格 | 统一结算 | 按各自中标报价 |
| 是否排序竞争性报价 | 是 | 是 |
| 是否接受全部竞争性投标 | 否 | 否 |

**示例**：按每100面值报价，发行量300单位，每笔申请100单位，A报102、B报101、C报100、D报99。中标A、B、C；D未中标。若以100为边际结算价，单一价格拍卖三家均支付100；多价格拍卖分别支付102、101、100。

**本题（Most likely correct）**：C 正确——价格报价通常从高到低排序。A 不成立——单一价格拍卖不必然导致更高融资成本、更窄投资者分布。B 错误——竞争性投标不是全部获配。

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


## 11. Repo Transactions｜回购交易基础

### Repo / Repurchase Agreement｜回购协议

- **定义**：一方出售证券并约定在未来某一日期按约定价格买回相同或等同证券的交易。
- **经济实质**：通常是一种以证券作抵押的短期融资安排（Secured Financing）。
- **借款方（Borrower）**：现在出售证券并取得现金，未来支付回购价格买回证券。
- **贷款方（Lender）**：现在支付现金并取得证券作为抵押，未来收回现金及约定收益。
- 从证券出售方角度看是 Repo；从现金提供方角度看是 Reverse Repo（逆回购）。

### Repo Participants｜回购交易参与方

- **Borrower（借款方）**：出售证券、取得现金的一方；承担未来回购证券的义务。
- **Lender（贷款方）**：提供现金、取得抵押品的一方。
- **Counterparty（交易对手）**：交易中的另一方，具体角色取决于观察视角。

### Collateral｜抵押品

- **定义**：为担保融资偿还而提供的资产。
- Repo 中通常由借款方交付证券作为抵押品。
- **Collateral Value（抵押品价值）**：用于计算抵押品覆盖程度的市场价值。
- **Cash Borrowed（借入现金）**：借款方通过 Repo 实际取得的现金金额。

### Haircut｜抵押品折扣率

- **定义**：抵押品市场价值超过实际借出现金金额的比例，用于为贷款方提供价格波动缓冲。
- **公式**：

\[
Haircut=\frac{Collateral\ Value-Cash\ Borrowed}{Collateral\ Value}
\]

- Haircut 越高，表示相对于抵押品价值，借款方能够取得的现金越少，贷款方通常获得的缓冲越大。
- **本题例子**：T-bonds 市场价值 3.2 million，借入现金 3.0 million：

\[
Haircut=\frac{3.2-3.0}{3.2}=0.0625=6.25\%
\]

- 注意：分母是抵押品价值，不是借入现金金额，也不是回购价格。

### Repo Price and Repo Interest｜回购价格与回购利息

- **Sale Price（初始出售价格）**：借款方在交易开始时收到的现金。
- **Repurchase Price（回购价格）**：借款方在约定日期买回证券时支付的金额。
- **Repo Interest（回购利息）**：回购价格与初始出售价格之间的差额。

\[
Repo\ Interest=Repurchase\ Price-Sale\ Price
\]

- **本题例子**：初始出售价格为 3.0 million，三个月后回购价格为 3.1 million：

\[
Repo\ Interest=3.1-3.0=0.1\text{ million}
\]

即 100,000 美元。

### Haircut 与 Repo Interest 的区别

| 项目 | Haircut | Repo Interest |
|---|---|---|
| 中文 | 抵押品折扣率 | 回购利息 |
| 衡量内容 | 抵押品价值相对融资金额的缓冲 | 初始融资金额对应的融资成本 |
| 计算 | (Collateral Value − Cash Borrowed) / Collateral Value | Repurchase Price − Sale Price |
| 本题结果 | 6.25% | $100,000 |

### 本题考点与做题步骤

1. 识别抵押品市场价值：3.2 million。
2. 识别实际借入现金（初始出售价格）：3.0 million。
3. 用两者差额除以抵押品价值，得到 Haircut = 6.25%。
4. 若题目问 Repo Interest，则用回购价格减初始出售价格，得到 100,000 美元。

**考试速记：**
- Haircut 看抵押品价值与实际融资金额。
- Repo Interest 看回购价格与初始出售价格。
- Repo 是借款方视角；Reverse Repo 是现金提供方视角。


### Types of Repo｜回购协议分类

回购交易可以从**到期期限、交易方向、抵押品要求**三个不同维度分类。以下名称并非完全互斥。

#### Term Repo｜固定期限回购

- **定义**：交易开始时约定明确的回购到期日（Fixed Maturity Date）。
- **判断关键词**：Specified Maturity / Fixed Term。
- **例子**：今天借款，约定30天后回购证券。

#### Open Repo｜开放式回购

- **定义**：没有预先约定固定的最终到期日，通常可依协议条款由任一方通知终止。
- **判断关键词**：No Fixed Maturity / Terminable on Notice。

#### Reverse Repo｜逆回购

- **定义**：从提供现金、取得证券的一方（Cash Lender）的视角看待同一回购交易。
- **区分**：Repo 一方借入现金并提供证券；Reverse Repo 的交易对手方提供现金并取得证券。
- **判断关键词**：Lends Cash / Acquires Securities。

#### General Collateral Repo｜一般抵押品回购

- **定义**：允许在某一类或一组合格证券中选择抵押品，而非必须交付某一只指定证券。
- **合格抵押品（Eligible Collateral）**：按协议满足期限标准（Maturity Criteria）、信用标准（Credit Criteria）等条件的证券。
- **特点**：融资方通常可从合格抵押品池中选择证券，交易主要关注融资而非某一特定证券。
- **判断关键词**：Group of Eligible Securities / Maturity and Credit Criteria。

#### Special Collateral Repo｜特定抵押品回购

- **定义**：交易要求交付某一只特定证券（Specific Security），交易的一项关键需求可能是取得该证券。
- **判断关键词**：Specific Security / Particular Bond。

### 五种概念对比

| 类型 | 分类依据 | 核心识别条件 |
|---|---|---|
| Term Repo | 期限 | 约定固定到期日 |
| Open Repo | 期限 | 无预先固定到期日 |
| Repo / Reverse Repo | 交易方向 | 借入现金 / 提供现金的视角 |
| General Collateral Repo | 抵押品要求 | 一组合格证券可供选择 |
| Special Collateral Repo | 抵押品要求 | 要求特定证券 |

**重要**：同一笔交易既可以是 Term Repo，也可以是 General Collateral Repo，因为期限与抵押品选择是不同的分类维度。

### 本题考点：General Collateral Repo

一家 Money Market Fund（货币市场基金）通过回购协议借入 $10,000,000，协议允许使用满足特定 **Maturity Criteria（期限标准）** 和 **Credit Criteria（信用标准）** 的一组证券作为抵押品。

- 题目强调的是**符合条件的一组证券**，而非某一只指定债券。
- 因此正确答案是 **C. General Collateral Repo**。
- **Term Repo** 侧重期限，但题干未给出固定到期日。
- **Reverse Repo** 是现金提供方的视角，而题中基金是借入现金的一方。

**考试速记**：Group of Eligible Securities → General Collateral；Specific Security → Special Collateral。


## 12. Short-Term Funding Markets｜银行短期融资市场

### Interbank Funds Market｜银行间资金市场

- **定义**：银行之间进行短期贷款与存款交易的市场。
- **主要用途**：调剂短期资金余缺、管理流动性（Liquidity）。
- **例子**：银行 A 短期缺少 500 万美元，向资金盈余的银行 B 借入该金额。
- **本题 Statement 1**：The market of loans and deposits between banks。正确。

### Central Bank Funds Market｜央行准备金资金市场

- **定义**：合格存款机构之间借贷其在中央银行持有的准备金余额的市场（在具体制度下可能有其他合格参与机构）。
- **主要用途**：满足准备金需求并管理短期流动性。
- **重要区别**：市场名称涉及中央银行准备金，不代表一定是中央银行直接向商业银行放款。
- **本题 Statement 2**：准备金不足的银行可以向准备金充裕的其他银行借款。正确。

### Required Reserves｜法定准备金

- **定义**：在适用制度存在法定准备金要求时，银行必须按监管规定持有的准备金。
- **注意**：各经济体的准备金制度不同，并非所有国家在任何时期都有正的法定准备金比例。

### Excess Reserves｜超额准备金

- **定义**：银行持有的准备金超过适用的最低准备金要求的部分。
- **例子**：若应持有 1000 万美元而实际持有 1500 万美元，超额部分为 500 万美元。

### Federal Funds Market｜美国联邦基金市场

- **定义**：美国合格存款机构等参与者借贷其在联邦储备体系持有的余额的市场，交易常见为隔夜期限。
- **Federal Funds Rate（联邦基金利率）**：该市场联邦基金交易的利率；常用的有效联邦基金利率为 Effective Federal Funds Rate（EFFR）。
- **与 Discount Window（贴现窗口）区别**：联邦基金交易通常发生在市场参与机构之间；贴现窗口是合格机构直接向美联储借款的机制。

### 两种资金市场对比

| 维度 | Interbank Funds Market | Central Bank Funds Market |
|---|---|---|
| 中文 | 银行间资金市场 | 央行准备金资金市场 |
| 交易对象 | 银行间短期资金借贷及存款 | 中央银行准备金余额 |
| 主要用途 | 流动性管理 | 准备金及短期流动性管理 |
| 两者关系 | 较广义 | 与银行间交易存在交集 |

### 本题速记

- Statement 1：银行间资金市场是银行之间的贷款和存款市场，**正确**。
- Statement 2：准备金不足的银行可向资金充裕的银行借款，**正确**。
- **答案 C：Both statements are correct**。


## 13. Matrix Pricing｜矩阵定价法

### Matrix Pricing｜矩阵定价法

- **定义**：当债券交易不活跃、缺少可靠的当前市场报价时，利用期限、信用质量等特征相近且具有可观察交易数据的债券，估计该债券的必要收益率（Required Yield）、利差（Required Yield Spread）或价格。
- **适用场景**：Inactively Traded Bonds（交易不活跃债券），不以经常交易且具有可靠报价的债券为典型应用对象。

### Comparable Bonds｜可比债券

- **定义**：用于估值参照、具有相似信用风险及现金流特征的债券。
- **选择要点**：相近的 Time to Maturity（剩余期限）、Credit Quality（信用质量），并考虑 Coupon Rate（票面利率）、流动性及其他条款。
- 对期限存在小幅差异的可比债券，可以根据适当假设进行 Linear Interpolation（线性插值）；信用质量差异较大时不可不加调整地直接比较。

### Benchmark Yield + Required Spread｜必要收益率简化分解

\[
Required\ Yield\approx Benchmark\ Yield+Required\ Yield\ Spread
\]

- **Benchmark Yield（基准收益率）**：同期限或可比条件下的参考收益率。
- **Required Yield Spread（必要收益率利差）**：相对基准收益率要求的额外补偿，可能反映信用、流动性及其他风险。
- **简化示例**：5年期基准收益率为3%，可比债券显示需要2%的利差，则估计必要收益率约为5%。

### 基本步骤

1. Identify Comparable Bonds：寻找信用质量、期限及其他特征相近的可比债券。
2. Estimate Yield or Spread：从可比债券数据估计必要收益率或相对基准的利差。
3. Discount Cash Flows：以估计的收益率折现目标债券未来现金流，获得估计价格。

### Linear Interpolation｜线性插值法（简化示例）

假设两只 AA 级可比债券：4年期收益率4%，6年期收益率5%。若5年期待估债券其他特征相近，则：

\[
Y_{5}=4\%+\frac{5-4}{6-4}(5\%-4\%)=4.5\%
\]

此例仅用来说明期限插值的计算方式，不代表市场收益率曲线一定线性。

### 本题考点

- A 错误：Matrix Pricing 主要应用于交易不活跃、缺少可观察报价的债券。
- B 错误：估值需要参考特征相近的可比债券，不能直接忽略期限和信用质量差异。
- C 正确：可用 Matrix Pricing 为交易不活跃债券估计相对 Benchmark 的 Required Yield Spread。
- **答案 C**。

**速记：交易不活跃 → 找相似债券 → 估计收益率或利差 → 折现估值。**
