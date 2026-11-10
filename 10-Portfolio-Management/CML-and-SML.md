---
subject: Portfolio Management
topic: Capital Market Line (CML) and Security Market Line (SML)
status: "🟡 解析能懂，待独立验证"
created: 2026-11-10
last-reviewed: 2026-11-10
tags: [CFA-L1, Portfolio-Management, CAPM, CML, SML, Alpha, Beta]
---

# 资本市场线与证券市场线（Capital Market Line, CML & Security Market Line, SML）

[[10-Portfolio-Management/INDEX|← 返回投资组合管理目录]]

## 一句话理解

- **CML（Capital Market Line，资本市场线）**：描述无风险资产与市场组合的不同配置所形成的**有效投资组合**的预期收益率与**总风险**之间的关系。
- **SML（Security Market Line，证券市场线）**：根据 CAPM 描述证券或投资组合的**系统性风险**（Beta）与其**理论要求收益率**之间的关系。

记忆：**CML 看总风险 $\sigma$ 和有效组合；SML 看系统性风险 $\beta$ 和 CAPM 定价。**

## 一、CML：资本市场线（Capital Market Line）

### 1. 定义与经济含义

在 CAPM 的均衡框架下，投资者可以将无风险资产（Risk-Free Asset）与市场组合（Market Portfolio）按不同比例组合，形成有效投资组合。所有这些有效组合的风险—收益关系落在 CML 上。

- **Risk-Free Asset（无风险资产）**：模型中收益确定，标准差为零。
- **Market Portfolio（市场组合）**：理论上包含市场中所有风险资产，并按市场价值加权；在 CAPM 均衡中是风险资产有效前沿的切点组合。
- **Efficient Portfolio（有效投资组合）**：在给定风险下预期收益最高，或给定预期收益下风险最低的组合。
- 投资者可按风险偏好选择不同位置：较保守者配置更多无风险资产；风险承受较高者增加市场组合权重；若允许按无风险利率借款，市场组合权重可超过 100%。

### 2. CML 公式

$$
\boxed{E(R_p)=R_f+
\frac{E(R_M)-R_f}{\sigma_M}\sigma_p}
$$

| 符号 | 英文 | 含义 |
|---|---|---|
| $E(R_p)$ | Expected Portfolio Return | 有效投资组合预期收益率 |
| $R_f$ | Risk-Free Rate | 无风险收益率 |
| $E(R_M)$ | Expected Market Return | 市场组合预期收益率 |
| $\sigma_p$ | Portfolio Standard Deviation | 投资组合标准差 |
| $\sigma_M$ | Market Portfolio Standard Deviation | 市场组合标准差 |

**斜率（Slope）：**

$$
\boxed{\frac{E(R_M)-R_f}{\sigma_M}}
$$

这是市场组合的**夏普比率（Sharpe Ratio）**，表示每承担一单位总风险所获得的市场风险溢价。

### 3. CML 的图形与适用范围

- 纵轴：预期收益率 $E(R_p)$；
- 横轴：总风险（Total Risk），用标准差 $\sigma_p$ 衡量；
- 纵轴截距：无风险收益率 $R_f$；
- 市场组合 $M$：CML 与风险资产有效前沿相切的位置；
- CML 上的组合是无风险资产与市场组合的有效组合；
- **不在 CML 上的风险组合通常是无效组合**，即存在其他组合能在相同风险下提供更高预期收益。

**考试关键词：CML = Total Risk = Standard Deviation = Efficient Portfolios。**

## 二、SML：证券市场线（Security Market Line）

### 1. 定义与经济含义

**SML（Security Market Line，证券市场线）**是 CAPM 的图形表达，描述资产或投资组合的 Beta 与 CAPM 理论要求收益率之间的线性关系。

它关注资产承担的**系统性风险（Systematic Risk）**，而不是全部波动。

- **Systematic Risk（系统性风险）**：由市场整体因素引起，无法通过持有更多不同证券完全分散掉的风险。
- **Unsystematic Risk（非系统性风险）**：公司或个别资产特有的风险，可通过充分分散化降低。
- **Beta（$\beta$，贝塔系数）**：衡量资产收益率对市场收益率变动的敏感度，反映系统性风险。

### 2. SML / CAPM 公式

$$
\boxed{E(R_i)=R_f+\beta_i[E(R_M)-R_f]}
$$

| 符号 | 英文 | 含义 |
|---|---|---|
| $E(R_i)$ | Expected Return | CAPM 下资产 $i$ 的理论要求收益率 |
| $R_f$ | Risk-Free Rate | 无风险收益率 |
| $\beta_i$ | Beta | 资产的系统性风险指标 |
| $E(R_M)$ | Expected Market Return | 市场组合预期收益率 |
| $E(R_M)-R_f$ | Market Risk Premium | 市场风险溢价 |

**斜率（Slope）：**

$$
\boxed{E(R_M)-R_f}
$$

即市场风险溢价（Market Risk Premium）：市场组合相对于无风险资产所要求的额外预期收益。

### 3. Beta 如何理解？

- $\beta=1$：资产的系统性风险与市场组合相当；
- $\beta>1$：资产对市场变动更敏感，系统性风险高于市场；
- $0<\beta<1$：资产对市场变动的敏感度较低；
- $\beta=0$：与市场收益率没有线性协动关系；
- $\beta<0$：与市场收益率呈负向协动。

Beta 不是“股票每天一定跟着市场涨跌多少”的保证，而是基于收益率关系估计出的敏感度。

### 4. SML 上方、线上、下方：Alpha 与定价

将资产的预期收益与 CAPM 要求收益比较：

$$
\alpha_i=E(R_i)_{\mathrm{forecast}}-
\left[R_f+\beta_i(E(R_M)-R_f)\right]
$$

- **SML 线上（On the SML）**：$\alpha=0$，预期收益等于 CAPM 要求收益；在模型意义上属于合理定价（Fairly Priced）。
- **SML 上方（Above the SML）**：$\alpha>0$，预期收益高于 CAPM 要求收益；在其他条件不变的估值解释下，通常意味着低估（Undervalued）。
- **SML 下方（Below the SML）**：$\alpha<0$，预期收益低于 CAPM 要求收益；通常意味着高估（Overvalued）。

注意：低估/高估是相对于 CAPM 基准及估值假设而言，并不保证价格一定会按预期调整。

### 5. SML 的适用范围：理论与现实要分清

- 在**CAPM 均衡且资产按模型合理定价**时，证券和投资组合的模型预期收益应满足 SML 关系。
- SML 是所有证券和投资组合的**定价基准**，并不意味着现实中每一项资产的预测收益都必然恰好落在线上。
- 若实际预测收益与 CAPM 要求收益不同，就会出现正或负 Alpha，资产点位可能在 SML 上方或下方。

**考试措辞陷阱：**“All securities and portfolios will lie on the SML”若没有“fairly priced / in CAPM equilibrium”等限定，不能不加区分地理解为现实中所有证券都必然在线上。只有满足 CAPM 合理定价关系的点才位于线上。

## 三、CML 与 SML 对比表

| 比较维度 | CML | SML |
|---|---|---|
| 全称 | Capital Market Line | Security Market Line |
| 中文 | 资本市场线 | 证券市场线 |
| 横轴风险指标 | 标准差 $\sigma$ | Beta $\beta$ |
| 风险类型 | 总风险（Total Risk） | 系统性风险（Systematic Risk） |
| 纵轴 | 预期收益率 | CAPM 理论要求收益率 / 预期收益率 |
| 适用对象 | 有效投资组合 | 证券及投资组合的 CAPM 定价关系 |
| 斜率 | 市场组合 Sharpe Ratio | 市场风险溢价 |
| 截距 | 无风险收益率 $R_f$ | Beta 为 0 时的无风险收益率 $R_f$ |
| 核心问题 | 有效组合的风险—收益关系 | 承担某一 Beta 应要求多少收益 |

**特别提醒：**SML 的适用对象比 CML 广。单只股票通常不位于 CML，因为它不是由无风险资产和市场组合构成的有效组合；但单只股票可以用 Beta 放在 SML 上进行 CAPM 定价比较。

## 四、典型 CFA 题：CML 与 SML 两个陈述

题目：

*With respect to the capital market line (CML) and security market line (SML), which of the following statements is/are correct?*

- Statement 1: *Only efficient portfolios will lie on the CML.*
- Statement 2: *All securities and portfolios of securities will lie on the SML.*

**题库答案：A — Only Statement 1 is correct.**

### Statement 1：正确

CML 表示无风险资产与市场组合构成的有效组合。位于 CML 上的组合属于有效组合；无效组合不在 CML 上。

### Statement 2：按本题题库口径判错

题库解析强调：**所有被合理定价（Fairly Priced）的证券和组合才落在 SML 上**。题干直接说“All securities and portfolios”全部必然位于 SML，遗漏了合理定价 / CAPM 均衡的限定，因此表述过宽。

如果资产存在非零 Alpha，预测收益就可能偏离 CAPM 要求收益，点位在 SML 上方或下方。

**本题正确选项：A。**

## 五、计算例题

### 例 1：CML 上有效组合的预期收益

假设：
- $R_f=3\%$；
- $E(R_M)=9\%$；
- $\sigma_M=20\%$；
- 某有效组合 $\sigma_p=10\%$。

$$
E(R_p)=3\%+\frac{9\%-3\%}{20\%}\times10\%
$$

$$
=\boxed{6\%}
$$

市场组合 Sharpe Ratio：

$$
\frac{9\%-3\%}{20\%}=0.30
$$

### 例 2：SML / CAPM 要求收益率

假设：
- $R_f=3\%$；
- $E(R_M)=9\%$；
- 股票 Beta $=1.5$。

$$
E(R_i)=3\%+1.5(9\%-3\%)
$$

$$
=\boxed{12\%}
$$

若该股票分析师预测收益率为 $15\%$：

$$
\alpha=15\%-12\%=\boxed{+3\%}
$$

正 Alpha，点位在 SML 上方；按 CAPM 基准解释为相对低估。

## 六、与已学知识的关系

- **Markowitz Efficient Frontier（马科维茨有效前沿）**：先根据风险资产的收益、方差和协方差建立有效集合。
- **CML（资本市场线）**：在 CAPM 框架下加入无风险资产与市场组合，描述有效组合的风险—收益关系。
- **CAPM / SML（资本资产定价模型 / 证券市场线）**：使用 Beta 衡量系统性风险，推导理论要求收益率。
- **Alpha（阿尔法）**：比较资产预测收益与 CAPM 要求收益的差额。
- **Utility Function / Indifference Curve（效用函数 / 无差异曲线）**：表达投资者的风险偏好，并帮助理解投资者如何选择组合。

相关笔记：
- [[Markowitz-Efficient-Frontier|马科维茨有效前沿]]
- [[Mean-Variance-Utility-Function|效用理论与均值—方差效用函数]]
- [[Indifference-Curve|无差异曲线]]

## 七、考试速记与复习检查

- **CML：$\sigma$，Total Risk，有效投资组合，斜率为市场组合 Sharpe Ratio。**
- **SML：$\beta$，Systematic Risk，CAPM 定价关系，斜率为 Market Risk Premium。**
- CML 上的组合是有效组合；SML 线上表示符合 CAPM 合理定价关系。
- 正 Alpha 在 SML 上方；负 Alpha 在 SML 下方。
- 不要把“所有资产都可用 SML 定价”误读为“现实中所有资产都必然落在 SML 上”。

- [ ] 能写出 CML 和 SML 的公式
- [ ] 能解释两条线横轴为什么不同
- [ ] 能说明 CML 与有效投资组合的关系
- [ ] 能解释 SML、CAPM 与 Beta 的关系
- [ ] 能判断 Alpha 正负及 SML 上下位置
- [ ] 能解释本题为什么 Statement 2 的 “All” 过于绝对
