---
subject: Portfolio Management
topic: Basics of Risk Management
status: "🟡 解析能懂，待独立验证"
created: 2026-11-11
last-reviewed: 2026-11-11
tags: [CFA-L1, Portfolio-Management, Risk-Management, Risk-Governance, Risk-Budgeting, Model-Risk, Tail-Risk]
---

# 风险管理基础（Basics of Risk Management）

[[10-Portfolio-Management/INDEX|← 返回投资组合管理目录]]

> 将当前复习中的风险预算、模型风险与尾部风险、有效风险治理知识统一整理。**只收录知识点、概念辨析及自拟例子，不保存完整题目和选项。** 内容以 CFA Institute 2026 年一级《Introduction to Risk Management》章节框架为主，另将近期题库采用的比较口径明确标注。

## 一、一句话理解

**风险管理（Risk Management）**不是消灭全部风险，而是结合组织目标，选择值得承担的风险，并**识别、衡量、监控、调整风险暴露**，使风险与组织可承受的水平相匹配。

可按以下逻辑梳理：

1. **Risk Governance（风险治理）**：谁来监督、批准风险承担方向和界限？
2. **Risk Appetite & Risk Tolerance（风险偏好与风险容忍度）**：愿意且可以承担哪些风险、多少风险？
3. **Risk Budgeting（风险预算）**：如何按照风险特征量化、配置风险额度或风险贡献？
4. **Risk Identification & Measurement（风险识别和测量）**：具体有哪些风险，如何测量？
5. **Risk Mitigation & Monitoring（风险缓释与监控）**：如何持续管理、调整并反馈？

这是帮助记忆的组织方式，**不是要求 ERM 必须按这些步骤串行运行**。

## 二、Risk Governance vs Risk Management Framework

### 1. Risk Governance（风险治理）

风险治理是风险管理的**顶层监督和责任体系**，强调风险决策的权限、责任和可接受的风险水平。

典型内容：
- 董事会（Board of Directors）对重大风险方向与风险容忍度进行监督；
- 风险委员会（Risk Committee）提供专门监督；
- 首席风险官（Chief Risk Officer, CRO）组织独立风险管理与报告；
- 明确组织允许承担和不可承担的风险，以及风险容忍度。

### 2. Risk Management Framework（风险管理框架）

风险管理框架的范围**大于**风险治理。按照 CFA Institute 2026 年一级阅读的概述，框架涉及：

- **Risk Governance**：风险治理；
- **Risk Identification and Measurement**：风险识别与测量；
- **Risk Infrastructure**：风险基础设施、系统与资源；
- **Risk Policies and Processes**：风险政策与流程；
- **Risk Mitigation and Management**：风险缓释及管理；
- **Communication**：风险信息沟通、报告与反馈；
- **Strategic Risk Analysis and Integration**：战略风险分析及整合。

### 3. Enterprise Risk Management（ERM，全面风险管理）

ERM 强调从**整个组织（Enterprise-wide）**视角综合识别和管理风险，而不是让市场、信用、流动性与操作风险各自孤立运作。

它是一种贯穿治理和实际管理全过程的综合视角，并非单纯位于风险预算之后的独立步骤。

### 4. 关于 Communication（沟通）的考试边界

近期题库在 **ERM / Risk Appetite / Communication** 三个选项之间，以 **Communication** 作为“最不可能属于核心 Risk Governance 要素”的答案。这一判断基于“**顶层治理核心要素**”的狭义比较口径。

但 CFA Institute 对更广义 **Risk Management Framework** 的总结中，**明确包含 Communication**：通过风险报告和反馈促进决策与管理改进。

**不能把题库结论误记为“风险管理不需要沟通”或“沟通不属于风险管理框架”。**

## 三、Risk Appetite、Risk Tolerance 与 Risk Budgeting

| 概念 | 英文 | 最重要的作用 | 判断关键词 |
|---|---|---|---|
| 风险偏好 | Risk Appetite | 组织为了目标**愿意**承担哪些风险及大致程度 | Willingness to take risk |
| 风险容忍度 | Risk Tolerance | 可接受与不可接受的风险及风险暴露**界限** | Acceptable / Unacceptable Risks, Limits |
| 风险预算 | Risk Budgeting | 按风险特征将投资或资产的**风险量化并分配** | Quantify / Allocate Risk |

### 1. Risk Appetite（风险偏好）

强调总体意愿。例如机构愿意承担适度股票市场风险，但不愿采用高杠杆策略。

风险偏好不是一个必须完全等同于最大亏损限额的概念；在实践中常由董事会批准或监督。

### 2. Risk Tolerance（风险容忍度）

强调可接受边界。按 CFA 本章口径，风险容忍度界定哪些风险可接受、哪些不可接受，以及组织整体可以暴露于多少风险。

例如：某策略的市场波动或损失风险不应超过预定限额。

### 3. Risk Budgeting（风险预算）

风险预算是一种**按照风险特征配置投资、风险额度或风险贡献**的方法，可以考虑资产波动、相关性、Beta、VaR 等风险度量。

若题目出现 **Quantify and Allocate Tolerable Risk（量化并分配可容忍风险）**，应优先识别为 **Risk Budgeting**，不是仅仅确认可承受风险界限的 Risk Tolerance。

### 4. 自拟例子：风险额度分配

假设一家投资机构给各策略制定内部风险额度：
- 股票策略：50 单位；
- 债券策略：30 单位；
- 其他策略：20 单位。

三部分**内部风险预算额度**相加为 100 单位，体现“分配”这一动作。

**注意：这里使用的是人为设定的可加总预算单位，不是说实际组合的 VaR 或标准差天然可以直接相加。** 真实组合风险还会受到相关性及风险贡献的影响。

## 四、风险来源（Sources of Risk）

### 1. Financial Risks（金融风险）

CFA 一级本章特别列出的金融风险包括：

| 英文 | 中文 | 含义 |
|---|---|---|
| Market Risk | 市场风险 | 股价、利率、汇率及商品价格等变动引起的风险 |
| Credit Risk | 信用风险 | 债务人或交易对手未按约履行付款义务 |
| Liquidity Risk | 流动性风险 | 因交易者缺乏或市场状况恶化，无法迅速以合理价格卖出资产 |

### 2. Non-financial Risks（非金融风险）

本章列举了多种非金融风险，包括：
- **Operational Risk（操作风险）**：人员、流程、系统故障或外部事件影响运营；
- **Legal / Regulatory Risk（法律 / 监管风险）**；
- **Accounting / Tax Risk（会计 / 税务风险）**；
- **Settlement Risk（结算风险）**；
- **Model Risk（模型风险）**；
- **Tail Risk（尾部风险）**。

**分类说明：**这里遵循 CFA 本章对风险来源的教学整理；模型风险和尾部风险也可能与金融市场损失交叉，并非表示“尾部风险与市场价格无关”。

### 3. 风险可以相互影响（Risk Interactions）

市场大幅波动可能引发保证金要求提高、资产折价卖出、流动性恶化，进一步放大市场损失。**风险并非彼此独立**，压力时期相关关系和影响可能非线性变化。

## 五、Model Risk 与 Tail Risk

### 1. Model Risk（模型风险）

**定义：**模型的假设、结构、输入数据、估计或使用方法存在问题，导致估值、风险测量或投资决策发生偏差。

常见成因：
- 使用了不符合现实的概率分布（Distribution Assumption）；
- 历史数据不充分，或者忽略市场状态切换；
- 相关系数、波动率估计偏差；
- 模型实施、验证与使用不当。

### 2. Tail Risk（尾部风险）

**定义：**收益或损失分布尾端的极端结果风险；风险管理尤其关注**左尾（Left Tail）的大额损失**。

典型例子：资产在平常时期表现稳定，但极端市场事件出现时可能发生非常大的损失。

### 3. 二者为什么关系密切？

例如模型假设每日收益服从正态分布（Normal Distribution），实际收益却具有较厚的尾部（Fat Tails）：

$$
\text{Unrealistic Model Assumption}
\longrightarrow
\text{Underestimated Extreme Losses}
$$

错误的模型可能**低估尾部事件的概率与损失规模**。

**关键区别：**
- **Tail Risk** 是需要面对的真实极端损失风险；
- **Model Risk** 是模型不能准确识别、衡量或预测有关风险所产生的错误风险；
- 两者会交叉，但**不是同一种风险，也并非所有模型风险都只涉及极端事件**。

按近期题库的三项比较（Tail Risk、Operational Risk、Liquidity Risk），其教学意图是优先选择 **Tail Risk** 作为与模型风险最直接的联系；不能由此推出模型风险与其他两种风险没有关联。

## 六、风险测量与管理手段（Risk Measures & Risk Responses）

### 1. 常见测量指标

- **Standard Deviation / Volatility（标准差 / 波动率）**：衡量收益总体波动；
- **Beta（贝塔系数）**：衡量相对市场的系统性风险；
- **Duration（久期）**：衡量利率变化对债券价格的敏感度；
- **Value at Risk, VaR（风险价值）**：在给定模型、时间范围和置信水平下的损失分位数；
- **Conditional VaR / Expected Shortfall（条件风险价值 / 预期尾部损失）**：关注超过 VaR 阈值的尾部损失；
- **Stress Testing / Scenario Analysis（压力测试 / 情景分析）**：考察极端或假设情境下可能的损失。

**易错点：VaR 并非最坏情况下的最大损失，也不自动表示超出 VaR 后损失有多大。**

### 2. 固定收益与衍生品的敏感性指标（Sensitivity Measures）

风险管理中要先辨别**受什么因素影响**，再选择适当的敏感性指标（Sensitivity Measure）。不能看到“价格变动”就把债券久期与期权希腊字母混用。

| 衡量指标 | 英文 | 衡量什么变化 | 常见应用 |
|---|---|---|---|
| **久期** | Duration | 债券价格对收益率变化的敏感度；其中**修正久期**直接近似价格百分比变化 | 固定收益（Fixed Income）利率风险 |
| **凸性** | Convexity | 债券价格—收益率关系的二阶曲率，补充久期的一阶近似 | 固定收益利率风险 |
| **德尔塔** | Delta ($\Delta$) | 期权价值对标的价格变化的一阶敏感度 | 期权（Options） |
| **伽马** | Gamma ($\Gamma$) | 期权 Delta 随标的价格变化的速度（二阶敏感度） | 期权 |
| **Rho** | Rho ($\rho$) | 期权价值对利率变化的敏感度（在常见希腊字母定义下） | 期权的利率敏感度 |

**修正久期（Modified Duration）**近似公式：

$
\boxed{\frac{\Delta P}{P}\approx-D_{\mathrm{mod}}\Delta y}
$

- $\Delta P/P$：债券价格的相对变动；
- $D_{\mathrm{mod}}$：修正久期（Modified Duration）；
- $\Delta y$：债券到期收益率的变化，使用**小数**表示，例如 100 bps = 0.01；
- **负号**反映普通固定利率债券价格与收益率通常反向变动。
- 例如 $D_{\mathrm{mod}}=5$、$\Delta y=+0.01$，则债券价格约下降 $5\%$。此为**一阶近似**，假设其他条件不变。

**加入凸性（Convexity）时**，在使用一致定义的凸性指标 $C$ 下：

$
\boxed{\frac{\Delta P}{P}\approx-D_{\mathrm{mod}}\Delta y+\frac12 C(\Delta y)^2}
$

**Delta 与 Gamma** 则主要针对期权价值 $V$ 对**标的资产价格** $S$ 的敏感性：

$
\Delta=\frac{\partial V}{\partial S},
\qquad
\Gamma=\frac{\partial^2 V}{\partial S^2}
$

**关键边界：**如果题干只问“固定收益证券对利率变化的敏感性”（Interest Rate Sensitivity of a Fixed-Income Instrument），在常规债券情境下应优先选 **Duration**，而不是 Delta 和 Gamma。利率衍生品也可能使用不同的风险希腊字母或 DV01 等指标，但不改变此基础题的判断。

详细推导与单位注意事项请查看：[[07-Fixed-Income/Modified-Duration|修正久期（Modified Duration）]]、[[07-Fixed-Income/Macaulay-Duration|麦考利久期（Macaulay Duration）]]。

### 3. 风险管理手段

- **Risk Avoidance / Prevention（风险规避与预防）**：不承担某项风险或降低事件发生可能性；
- **Risk Transfer（风险转移）**：例如保险；
- **Risk Shifting / Hedging（风险转移暴露 / 对冲）**：例如使用衍生品调整风险敞口；
- **Diversification（分散化）**：降低可分散的特有风险；
- **Monitoring and Limits（风险监控及限额）**：持续检测风险暴露是否超出允许范围。

选择方法时应比较其潜在效益、成本及最终整体风险状况，并与治理目标保持一致。

## 七、三组核心区别一页速查

| 概念组 | 更精准的区别 |
|---|---|
| Risk Governance vs Risk Management Framework | **治理是顶层监督；框架还包括沟通、识别、度量、实施和反馈** |
| Risk Appetite vs Risk Tolerance vs Risk Budgeting | **愿意承担 → 可接受边界 → 按风险特征配置额度**（记忆逻辑，非强制线性顺序） |
| Model Risk vs Tail Risk | **模型出错或失效的风险 → 极端损失本身的风险**；可能相互关联但不相同 |

### 关键词快速识别

- **Enterprise-wide / Integrated Risk** → Enterprise Risk Management。
- **Risk oversight / Board / CRO / Committee** → Risk Governance。
- **Communication / Reporting / Feedback Loops** → Risk Management Framework 的沟通环节。
- **Willingness to take risk** → Risk Appetite。
- **Acceptable risk / Risk limits** → Risk Tolerance。
- **Quantify and allocate risk** → Risk Budgeting。
- **Incorrect assumptions / Faulty models** → Model Risk。
- **Fat tails / Extreme losses** → Tail Risk。

## 八、与既有 CFA 笔记的联系

- [[Portfolio-Management-Process|投资组合管理流程]]：风险目标与治理要求影响 Planning；风险监控影响 Feedback。
- [[Investment-Policy-Statement|投资政策声明（IPS）]]：Risk Objectives、Constraints、Risk Tolerance 的投资者层面应用。
- [[Systematic-vs-Nonsystematic-Risk|系统性风险、非系统性风险与分散化]]：与风险来源分类互补，但系统性/非系统性是**风险能否被分散**的维度。
- [[CML-and-SML|资本市场线与证券市场线]]：标准差与 Beta 衡量不同维度的投资风险。
- [[07-Fixed-Income/Modified-Duration|修正久期（Modified Duration）]]：固定收益证券对收益率变动的价格敏感性公式与单位。

## 九、复习检查

- [ ] 能区分 Risk Governance 与 Risk Management Framework，并解释 Communication 的角色
- [ ] 能解释 ERM 为什么是企业整体视角
- [ ] 能区分 Risk Appetite、Risk Tolerance、Risk Budgeting 的英文触发词
- [ ] 能列出 Market、Credit、Liquidity、Operational、Model、Tail Risks 的中文含义
- [ ] 能说明模型为何可能低估尾部风险，以及二者并不等同
- [ ] 能说明 VaR 为什么不是“最大可能损失”
- [ ] 能区分 Duration、Convexity 与期权的 Delta、Gamma、Rho，并正确使用修正久期公式
- [ ] 能描述风险规避、转移、对冲和分散化的基本作用

## 来源与适用范围

- CFA Institute, **2026 Level I Portfolio Management — Introduction to Risk Management**，公开学习摘要（本笔记对风险治理、风险管理框架、风险预算、风险来源和应对方式的划分依据）：https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/introduction-risk-management
- CFA Institute, **2026 Level II Portfolio Management — Measuring and Managing Market Risk**（补充理解压力测试、VaR 与模型局限；不作为一级考试题量或要求的依据）：https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/measuring-managing-market-risk

> 本文件保留一级学习层次；增加少量必要的模型风险与风险预算说明，旨在避免错误记忆。题库中“最符合/最不符合”的判断，须结合明确的比较范围，不应误记为不附条件的通用定义。
