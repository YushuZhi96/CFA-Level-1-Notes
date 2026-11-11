---
subject: Portfolio Management
topic: Market Anomalies and Fama-French Three-Factor Model
status: "🟡 解析能懂，待独立验证"
created: 2026-11-11
last-reviewed: 2026-11-11
tags: [CFA-L1, Portfolio-Management, Market-Anomalies, Value-Effect, Multifactor-Models, CAPM, Fama-French]
---

# 市场异象与 Fama-French 三因子模型（Market Anomalies & Fama-French Three-Factor Model）

[[10-Portfolio-Management/INDEX|← 返回投资组合管理目录]]

## 一句话理解

**市场异象（Market Anomaly）**是指某种市场收益规律难以由现有资产定价模型或简单的市场有效性解释。**价值效应（Value Effect）**是常见例子：历史样本中，价值股（Value Stocks）往往表现出高于成长股（Growth Stocks）的平均收益。

**但“长期跑赢”本身只描述现象，并不能证明这种收益是市场错误定价，也不能证明它一定是合理的风险补偿。** 分析需要判断是否存在额外风险暴露、遗漏的定价因子或行为偏差。

## 一、三个层次：现象、解释、剩余异常收益

1. **观察到现象（Observed Return Pattern）**：某类股票的历史平均收益更高，例如价值股相对成长股的长期收益差异。
2. **尝试解释（Explanations）**：
   - 风险补偿（Risk-Based Explanation）：资产承担更多被市场定价的风险，因此要求更高回报；
   - 错误定价/行为解释（Mispricing / Behavioral Explanation）：投资者过度反应、预期偏差或市场摩擦导致价格与基本面偏离；
   - 模型遗漏因子（Omitted Factors）：原模型不够完整，无法解释系统性收益差异。
3. **考察风险调整后的剩余收益（Risk-Adjusted Alpha）**：加入合理因子后，原先显著的 Alpha 是否仍存在？

**判断原则：收益差异持续存在 ≠ 已经知道差异产生的原因。**

## 二、常见市场异象

| 中文 | 英文 | 典型现象或定义 |
|---|---|---|
| 价值效应 | Value Effect / Value Premium | 高账面市值比（Book-to-Market Ratio）的股票在某些历史样本中平均收益较高 |
| 规模效应 | Size Effect / Size Premium | 小市值股票在一些历史样本中平均收益高于大市值股票 |
| 动量效应 | Momentum Effect | 过去一段时期表现强势的证券在某些后续时期仍可能相对强势 |
| 异常收益 | Abnormal Return | 无法被指定基准资产定价模型解释的收益部分；定义依赖模型 |

**注意：**异象的统计表现会因样本、时期、市场和模型而变化；并不保证未来持续，更不保证扣除交易成本后可获利。

## 三、CAPM 为什么可能解释不够？

**资本资产定价模型（Capital Asset Pricing Model, CAPM）**：

$$
\boxed{E(R_i)=R_f+\beta_i[E(R_M)-R_f]}
$$

其中：
- $R_f$：无风险收益率（Risk-Free Rate）；
- $\beta_i$：对市场系统性风险的敏感度（Market Beta）；
- $E(R_M)-R_f$：市场风险溢价（Market Risk Premium）。

CAPM 用一个市场风险因子解释资产所需的收益率。如果某类股票在控制市场 Beta 后仍有系统性的超额收益，可能表现为**相对于 CAPM 的异常收益（CAPM Alpha）**。但这也可能只是单因子模型遗漏了额外的收益解释变量。

## 四、Fama-French 三因子模型（Fama-French Three-Factor Model）

Fama-French 三因子模型在市场因子之外，加入**规模因子 SMB**和**价值因子 HML**，以解释股票收益率的共同变动。

### 1. 因子回归的常见表达

$$
\boxed{R_{i,t}-R_{f,t}=\alpha_i+
\beta_{i,M}(R_{M,t}-R_{f,t})+
s_i SMB_t+
h_i HML_t+
\varepsilon_{i,t}}
$$

| 符号 | 英文 | 含义 |
|---|---|---|
| $R_{i,t}-R_{f,t}$ | Asset Excess Return | 资产的当期超额收益 |
| $R_{M,t}-R_{f,t}$ | Market Excess Return | 市场因子 |
| $SMB_t$ | Small Minus Big | 规模因子：小市值股票相对大市值股票的因子组合收益 |
| $HML_t$ | High Minus Low | 价值因子：高账面市值比股票相对低账面市值比股票的因子组合收益 |
| $\beta_{i,M}$ | Market Factor Loading | 资产对市场因子的暴露 |
| $s_i$ | Size Factor Loading | 对规模因子的敏感度 |
| $h_i$ | Value Factor Loading | 对价值因子的敏感度 |
| $\alpha_i$ | Intercept / Alpha | 回归截距，模型没有解释的平均收益部分 |
| $\varepsilon_{i,t}$ | Residual | 随机残差 |

**三因子不是“三种股票”：**Market、SMB、HML 是因子/因子组合收益；$\beta,s,h$ 是证券对这些因子的敏感度。

### 2. 对应的预期收益表达（模型应用）

以估计的平均因子溢价 $\lambda_M,\lambda_{SMB},\lambda_{HML}$ 表示：

$$
\boxed{E(R_i)-R_f\approx
\beta_{i,M}\lambda_M+s_i\lambda_{SMB}+h_i\lambda_{HML}}
$$

这是一种用于理解和估算模型解释收益的表达，并非宣称每个因子的未来溢价恒定或已被证明全由风险造成。

### 3. SMB 与 HML 的方向

- **SMB（Small Minus Big）**：Small（小市值）减 Big（大市值）。若因子收益为正，表示对应的小市值因子组合表现较强。
- **HML（High Minus Low）**：High **Book-to-Market（高账面市值比）**减 Low Book-to-Market（低账面市值比）。高账面市值比常用于代表价值股，低账面市值比常用于代表成长股。
- **HML 的 High/Low 指账面市值比，不是股价高低，也不是单纯的市盈率高低。**

## 五、为什么加入 HML 后，价值效应可能不再显得异常？

如果只使用 CAPM，价值股的收益中可能留有未解释部分，即 CAPM Alpha。

若进一步加入 HML，价值股相对较高的平均收益可能被其正向的价值因子暴露（$h_i$）所解释，**三因子模型下的 Alpha 可能减小甚至统计上不再显著**。

这表示：相对于**新的三因子基准**，原先不能解释的收益差异被模型吸收。

但必须区分：

- **统计解释（Statistical Explanation）**：因子模型拟合了历史收益关系；
- **经济解释（Economic Explanation）**：为什么因子会获得溢价，可能涉及风险、行为或市场摩擦。

**因子能解释收益，不等于已证明该因子溢价一定是额外风险的报酬，也不等于完全证明市场有效。**

### 一个简化的数字例子

以下全部为**假设的年化预期因子溢价**，用于理解公式：

| 项目 | 数值 |
|---|---:|
| 资产预期超额收益 $E(R_i)-R_f$ | 11% |
| 市场因子溢价 $\lambda_M$，资产市场暴露 $\beta=1$ | $6\%\times1=6\%$ |
| 规模因子溢价 $\lambda_{SMB}$，资产暴露 $s=0.5$ | $2\%\times0.5=1\%$ |
| 价值因子溢价 $\lambda_{HML}$，资产暴露 $h=1$ | $4\%\times1=4\%$ |

- 仅按市场因子解释：$11\%-6\%=5\%$，存在未解释的收益差异；
- 加入 SMB、HML 后：$6\%+1\%+4\%=11\%$，在这个假设例子中三因子解释了全部预期超额收益。

这里演示的是**模型解释力**，不能据此认定某个真实证券一定获得这些溢价。

## 六、价值股与成长股（Value vs Growth）

**价值股（Value Stocks）**：常被划分为估值比率较低或账面市值比较高的股票，例如相对于市值有较高账面权益。

**成长股（Growth Stocks）**：通常具有较高预期增长，部分估值倍数较高；在经典 HML 构造中更接近低账面市值比组。

价值股历史平均收益更高可能有多种解释：

1. **风险补偿（Risk Premium）**：某些价值公司可能面对财务困境、经营周期等风险；
2. **错误定价（Mispricing）**：投资者可能过度乐观看待成长股、过度悲观看待价值股；
3. **模型设定问题（Model Specification）**：单一市场 Beta 不足以捕捉跨股票的收益差异。

不应把“价值股长期跑赢”本身当作证明其风险更高、风险溢价合理，或者市场存在永久套利机会的证据。

## 七、与 CAPM、SML 的知识衔接

- [[CML-and-SML|资本市场线与证券市场线（CML & SML）]]：CAPM/SML 以市场 Beta 与市场风险溢价描述要求收益；三因子模型加入规模、价值暴露。
- [[Systematic-vs-Nonsystematic-Risk|系统性风险、非系统性风险与分散化]]：理解哪些风险可能被定价、哪些特有风险可以分散；因子模型中的额外暴露不等于每一种个股特有风险都应获补偿。
- [[Markowitz-Efficient-Frontier|马科维茨有效前沿]]：风险与收益的均值—方差分析为资产定价与组合选择提供基础。

## 八、CFA 考试速记与易错点

| 看到的表述 | 主要判断 |
|---|---|
| Value stocks outperform growth stocks over long periods | **观察现象**，不解释收益差异为何合理 |
| Additional risk exposure explains higher expected return | **风险补偿解释**的一种可能 |
| CAPM Alpha becomes insignificant under a three-factor model | 原异常收益可能来自**模型遗漏的因子** |
| HML = High Minus Low | **高/低账面市值比**，并不是股价或市盈率高/低 |
| SMB = Small Minus Big | **小市值减大市值**的因子组合 |
| Explaining the premium proves all value returns are risk compensation | **错误**：模型统计解释不等于经济机制已证实 |

- [ ] 能解释 Market Anomaly 与模型基准的关系
- [ ] 能区分“长期超额收益的事实”和“为何超额收益的解释”
- [ ] 能写出 CAPM 与 Fama-French 三因子模型的基本表达
- [ ] 能正确解释 SMB、HML、$\beta$、$s$、$h$ 和 Alpha
- [ ] 能说明模型解释力为何不等于证明纯粹风险补偿
