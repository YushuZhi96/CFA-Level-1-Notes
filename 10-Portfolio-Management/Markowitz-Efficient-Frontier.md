---
subject: Portfolio Management
topic: Markowitz Efficient Frontier
status: "🟡 解析能懂，待独立验证"
created: 2026-11-10
last-reviewed: 2026-11-10
tags: [CFA-L1, Portfolio-Management, Markowitz, Efficient-Frontier, Diversification]
---

# 马科维茨有效前沿（Markowitz Efficient Frontier）

[[10-Portfolio-Management/INDEX|← 返回投资组合管理目录]]

## 一句话理解

**Markowitz Efficient Frontier（马科维茨有效前沿）**是现代投资组合理论（Modern Portfolio Theory, MPT）在均值—方差框架下得到的一组**有效投资组合（Efficient Portfolios）**：在给定风险下，它们具有可行组合中的最高预期收益；或在给定预期收益下，具有最低风险。

**核心区分：有效前沿由资产的收益、风险与相关性（以及投资限制）确定；个人风险偏好影响投资者最终选择前沿上的哪一个组合，不是绘制前沿必需的市场统一假设。**

## 一、有效前沿的图形怎么读？

常用的风险—收益坐标中：

- **横轴（X-axis）**：Portfolio Risk（组合风险），通常是收益率标准差 $\sigma_p$；
- **纵轴（Y-axis）**：Expected Portfolio Return（组合预期收益率）$E(R_p)$；
- **Global Minimum-Variance Portfolio, GMV（全局最小方差组合）**：所有可行投资组合中方差最低的组合；
- **Efficient Frontier（有效前沿）**：从最小方差组合开始、向预期收益更高的一侧延伸的**上部边界**（常见的仅风险资产、允许适当权重配置的情形下）；
- **Inefficient Portfolio（无效组合）**：可找到另一个组合，在风险不更高时收益更高，或在收益不更低时风险更小。

注意：在常见的“子弹形”可行组合区域里，**不是整条最小方差边界都有效**；GMV 下方的低收益分支通常是无效的。

## 二、构建有效前沿需要什么输入？

| 关键输入 | 英文 | 作用 |
|---|---|---|
| 每项资产的预期收益率 | Expected Returns | 决定组合预期收益 |
| 每项资产收益率的标准差 / 方差 | Standard Deviations / Variances | 决定单个资产的波动风险 |
| 资产收益率两两相关系数 / 协方差 | Pairwise Correlations / Covariances | 决定组合资产之间如何共同波动 |
| 可行权重与投资限制 | Portfolio Weights / Constraints | 界定可投资组合集合，例如是否允许做空 |

**本题的措辞提示：**严格来说，相关性讨论的是**资产实际收益率这一随机变量之间**的相关性（Correlation of Asset Returns），而不是把各个资产的“预期收益率”这些常数再算相关系数。题目 A 的意图是考查两两相关系数这一必要输入。

**不需要的条件：Homogeneous Risk Attitude（所有投资者具有相同风险态度）。** 不同投资者可以根据自身风险厌恶程度选取不同的有效组合，无须在市场中拥有一致的风险态度。

## 三、关键公式

### 1. 组合预期收益率（Expected Portfolio Return）

$$
\boxed{E(R_p)=\sum_{i=1}^{n}w_iE(R_i)}
$$

两资产时：

$$
E(R_p)=w_AE(R_A)+w_BE(R_B)
$$

其中 $w_i$ 是资产 $i$ 的配置权重。完全投资的简单组合通常满足：

$$
\sum_{i=1}^{n}w_i=1
$$

若允许卖空，部分 $w_i$ 可以小于 $0$，其他权重也可能大于 $1$。

### 2. 两资产组合方差（Two-Asset Portfolio Variance）

$$
\boxed{\sigma_p^2=w_A^2\sigma_A^2+w_B^2\sigma_B^2+2w_Aw_B\sigma_A\sigma_B\rho_{AB}}
$$

其中：

- $\sigma_A,\sigma_B$：单项资产收益率的标准差（Standard Deviation）；
- $\sigma_p^2$：投资组合收益率方差（Portfolio Variance）；
- $\rho_{AB}$：资产 A、B 收益率的相关系数（Correlation Coefficient）；
- $\operatorname{Cov}(R_A,R_B)=\sigma_A\sigma_B\rho_{AB}$：协方差（Covariance）。

组合**标准差**还需开平方：

$$
\boxed{\sigma_p=\sqrt{\sigma_p^2}}
$$

### 3. 多资产组合方差（General Portfolio Variance）

$$
\boxed{\sigma_p^2=\sum_{i=1}^{n}\sum_{j=1}^{n} w_iw_j\operatorname{Cov}(R_i,R_j)}
$$

等价矩阵写法：

$$
\boxed{\sigma_p^2=\boldsymbol{w}^{\mathsf T}\boldsymbol{\Sigma}\boldsymbol{w}}
$$

其中 $\boldsymbol{\Sigma}$ 是资产收益率的协方差矩阵（Covariance Matrix）。

## 四、从公式理解分散化（Diversification）

在权重与单资产风险固定时，较低的资产相关性通常能降低组合方差：

- $\rho_{AB}=+1$：两资产完全正相关（Perfect Positive Correlation）；在两个正权重的组合中没有相关性带来的分散化收益；
- $-1<\rho_{AB}<+1$：存在不同程度的分散化可能；
- $\rho_{AB}=-1$：完全负相关（Perfect Negative Correlation）；在允许合适权重、且两资产标准差为正的条件下，可构造零方差组合。

**例子**：将 A、B 各配置 50%，已知：

| 指标 | A | B |
|---|---:|---:|
| 预期收益率 | 10% | 8% |
| 标准差 | 20% | 10% |

两资产收益率相关系数为 $\rho_{AB}=0.2$。

收益：

$$
E(R_p)=0.5(0.10)+0.5(0.08)=\boxed{9\%}
$$

方差：

$$
\sigma_p^2=(0.5)^2(0.20)^2+(0.5)^2(0.10)^2
+2(0.5)(0.5)(0.20)(0.10)(0.2)
$$

$$
=0.0100+0.0025+0.0020=0.0145
$$

标准差：

$$
\sigma_p=\sqrt{0.0145}\approx\boxed{12.04\%}
$$

比较：两项标准差的简单加权平均为 $0.5(20\%)+0.5(10\%)=15\%$；**组合的实际标准差 12.04% 更低**，体现相关性较低时的分散化效果。不能把组合标准差机械当作单资产标准差的加权平均。

## 五、如何从“可行组合”找到有效前沿？

1. 估计各资产的 $E(R_i)$、$\sigma_i$ 和协方差/相关系数；
2. 设定权重条件和约束（例如 $\sum w_i=1$，是否允许 $w_i<0$）；
3. 使用权重计算各候选组合的预期收益率与方差；
4. 识别可行集合中的最小方差边界，并保留**风险相同下预期收益最高**的有效部分；
5. 投资者再结合个人风险厌恶程度，在有效前沿上选择**最优投资组合（Optimal Portfolio）**。

**不要把“构建有效前沿”与“选择个人最优组合”混为一谈。** 只有后者需要引入个人效用偏好。

## 六、本次 CFA 选择题（概念型）

题目要点：*To construct the Markowitz efficient frontier, which of the following is least likely to be considered?*

- **A. The paired correlations of all assets' expected returns.**
  - 题意关注两两相关系数。**需要**：相关性决定不同资产组合后的协方差与风险。
- **B. The standard deviations of all assets' expected returns.**
  - 题意关注资产收益率标准差。**需要**：标准差刻画单项资产风险。
- **C. Homogeneous risk attitude in the financial market.**
  - **不需要，正确答案 C**：构建资产机会集合的有效边界，不要求所有投资者风险态度相同。

核心辨析：

> **Expected Returns + Variances + Covariances → Efficient Frontier；Investor Risk Preferences → Preferred/Optimal Portfolio。**

## 七、与效用函数（Utility Function）的衔接

我们此前学过的均值—方差效用函数：

$$
U=E(R_p)-\frac12 A\sigma_p^2
$$

其中 $A$ 为风险厌恶系数（Risk Aversion Coefficient）。

- **Markowitz Efficient Frontier**：用资产数据求“哪些组合在风险—收益上有效”；
- **Utility Function**：给定某位投资者的 $A$，评价组合；
- **Optimal Portfolio**：在可选的组合中寻找使该投资者效用最大的组合（具体选择受投资限制影响）。

**相关笔记：**[[Mean-Variance-Utility-Function|效用理论与均值—方差效用函数]]；[[Time-Weighted-Return|时间加权收益率（TWR）]]（收益绩效衡量，与均值—方差优化是不同考点）。

## 八、常见考试陷阱与复习检查

- 把 **Expected Return、Standard Deviation、Correlation/Covariance** 中任何一项漏掉：都无法完整建立风险—收益的均值—方差关系。
- 把“投资者相同的风险偏好”当成有效前沿的构建条件：**错误**。
- 把全体可行组合都当有效组合：**错误**；只有在某种意义下无法被其他组合支配的上部边界有效。
- 把 $\sigma_p^2$（方差）错认为 $\sigma_p$（标准差）：**标准差需要开平方**。
- 把均值—方差模型中的“预测输入”当成现实中确定的已知数：实际投资中，这些量需要估计，结果会受到估计误差和配置约束影响。

### 我的验证记录

- 本题答案：**C**。
- [ ] 不看解析能解释有效前沿与最小方差组合的关系
- [ ] 能列出预期收益、标准差、两两相关/协方差三类主要输入
- [ ] 能正确写出两资产组合预期收益与方差公式
- [ ] 能解释个人风险偏好不决定有效前沿本身
- [ ] 能区分“建立有效前沿”和“在前沿上选择最优组合”
