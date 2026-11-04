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

## 5. 做题提醒

- 题目问 **Tenor** 或剩余到期时间时，先判断债券已经发行多久，再用原始期限减去已过去时间。
- 面值（Par Value）和票面利率（Coupon Rate）通常不是计算 Tenor 所必需的数据；若题目只问期限，不要被无关数据干扰。


## 6. Sinking Fund｜偿债基金

### Sinking Fund Arrangement（偿债基金安排）

发行人依据债券契约逐步偿还部分债券本金，或积累用于偿还债券的资金。偿债方式可能包括按计划赎回部分债券或在二级市场购回债券。

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
