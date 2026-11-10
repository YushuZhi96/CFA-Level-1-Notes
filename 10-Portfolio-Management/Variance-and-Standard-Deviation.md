---
subject: Portfolio Management
topic: Variance and Standard Deviation
status: "🟡 解析能懂，待独立验证"
created: 2026-11-10
last-reviewed: 2026-11-10
tags: [CFA-L1, Portfolio-Management, Quantitative-Methods, Variance, Standard-Deviation, Risk]
---

# 方差与标准差（Variance & Standard Deviation）

[[10-Portfolio-Management/INDEX|← 返回投资组合管理目录]]

## 一句话理解

**方差（Variance）**衡量观察值与平均值之间的**平方偏离程度**；**标准差（Standard Deviation）**是方差的平方根，可以把波动幅度恢复到与原始收益率相同的单位，因此在金融分析中更直观。

在投资组合管理中，收益率的**标准差**是衡量总体波动风险（Total Volatility / Total Risk）的常见指标：标准差越大，收益率围绕均值的波动通常越明显，但标准差本身不区分上涨与下跌。

## 核心术语

| 中文 | English | 符号 / 含义 |
|---|---|---|
| 总体均值 | Population Mean | $\mu$ |
| 样本均值 | Sample Mean | $\bar R$ |
| 总体方差 | Population Variance | $\sigma^2$ |
| 样本方差 | Sample Variance | $s^2$ |
| 总体标准差 | Population Standard Deviation | $\sigma$ |
| 样本标准差 | Sample Standard Deviation | $s$ |
| 观测收益率 | Observed Return | $R_i$ |
| 自由度 | Degrees of Freedom | 样本方差使用 $n-1$ |

## 四个核心公式：把样本与总体放在一起记

### 1. 总体方差（Population Variance）

当观测值构成需要描述的**完整总体**时：

$$
\boxed{\sigma^2=\frac{\sum_{i=1}^{N}(R_i-\mu)^2}{N}}
$$

总体均值：

$$
\mu=\frac{1}{N}\sum_{i=1}^{N}R_i
$$

### 2. 样本方差（Sample Variance）

当观测值是用来**估计总体方差的样本**时：

$$
\boxed{s^2=\frac{\sum_{i=1}^{n}(R_i-\bar R)^2}{n-1}}
$$

样本均值：

$$
\bar R=\frac{1}{n}\sum_{i=1}^{n}R_i
$$

### 3. 总体标准差（Population Standard Deviation）

$$
\boxed{\sigma=\sqrt{\sigma^2}}
$$

### 4. 样本标准差（Sample Standard Deviation）

$$
\boxed{s=\sqrt{s^2}}
$$

**口诀：先求均值 → 求偏差 → 偏差平方并求和 → 样本除以 $n-1$（总体除以 $N$）→ 题目若问标准差再开平方。**

### 为什么样本方差分母是 $n-1$？

用样本数据估计了样本均值 $\bar R$，相对于估计总体均值，损失了一个**自由度（Degree of Freedom）**。采用 $n-1$ 的**贝塞尔校正（Bessel's Correction）**，可在独立同分布、方差有限等常见条件下使样本方差成为总体方差的**无偏估计量（Unbiased Estimator）**。

## CFA 例题：对冲基金 A 的五个月月收益率

题目问：**The sample variance of Fund A is closest to:**（基金 A 的样本方差最接近哪一个？）

| 月份 | 基金 A 的月收益率 |
|---|---:|
| January（1 月） | 4% |
| February（2 月） | 2% |
| March（3 月） | −2% |
| April（4 月） | −5% |
| May（5 月） | 3% |

题目同时提供基金 B 的数据，但**求基金 A 自身的样本方差不需要基金 B 的数据**。

### 第一步：算样本均值

$$
\bar R=\frac{4\%+2\%-2\%-5\%+3\%}{5}=\boxed{0.4\%}
$$

### 第二步：偏差与偏差平方

为便于手算，下表暂以**百分数点**表示收益率和偏差：

| 月份 | 收益率（%） | 与均值 0.4% 的偏差（百分点） | 偏差平方（百分点²） |
|---|---:|---:|---:|
| 1 月 | 4 | 3.6 | 12.96 |
| 2 月 | 2 | 1.6 | 2.56 |
| 3 月 | −2 | −2.4 | 5.76 |
| 4 月 | −5 | −5.4 | 29.16 |
| 5 月 | 3 | 2.6 | 6.76 |
| **合计** | | | **57.20** |

### 第三步：算样本方差

$$
s^2=\frac{57.20}{5-1}=14.30\ \text{（百分点）}^2
$$

如果把收益率统一写成小数，方差为：

$$
\boxed{s^2=\frac{14.30}{100^2}=0.00143}
$$

原题选项把这个数值写成 **$0.14\%$**（因 $0.00143\times100=0.143$），因此选 **A：0.14%**。

**特别注意单位：**严格地说，方差的单位是“收益率单位的平方”，不应把它当成与标准差同量纲的普通百分比。推荐记录为 **$0.00143$（小数收益率平方）** 或 **$14.30\text{（百分点）}^2$**；原题的“0.14%”只是考试选项采用的数值写法。

### 第四步：若题目改问样本标准差

$$
s=\sqrt{0.00143}=0.037815\ldots=\boxed{3.78\%}
$$

因此该题三个选项中：

- **A：0.14% → 样本方差的试题表示（正确）**
- **C：3.78% → 样本标准差，开了平方根（不是本题问的方差）**
- **B：0.11% → 误用总体分母 $N=5$ 附近的结果**（总体方差 $0.001144$，按选项习惯约写为 $0.11\%$）

## 直觉和用途

1. 计算平方偏差，是为了避免正负偏差相互抵消，并让大偏差受到更大的权重。
2. 方差将离均程度表达为平方单位；**标准差把单位开方恢复**，便于跟原始收益率直接比较。
3. 在现代投资组合理论（Modern Portfolio Theory）中，**组合标准差**常作为风险轴，而不是只看各资产标准差的简单平均。

## 考试高频陷阱

| 题干关键词 | 正确动作 | 常见错误 |
|---|---|---|
| **Sample Variance** | 除以 $n-1$，**不开平方** | 用 $n$ 或误开平方 |
| **Population Variance** | 除以 $N$，**不开平方** | 把总体当样本 |
| **Sample Standard Deviation** | 样本方差算完**开平方** | 把方差直接当标准差 |
| **Population Standard Deviation** | 总体方差算完**开平方** | 混用两种分母 |
| 收益率以百分数给出 | 统一计算单位、留意平方后换算 | 将 $14.30$ 直接写为 14.30% |
| 两个基金的数据并列 | 先确认问的是单一资产方差、组合方差还是协方差 | 为单资产方差误用另一只基金数据 |

## 与投资组合管理其他知识点的联系

- **Portfolio Risk（投资组合风险）**：组合方差不仅与每项资产的方差有关，还与资产之间的**协方差（Covariance）**或**相关系数（Correlation）**有关。
- [[Markowitz-Efficient-Frontier|马科维茨有效前沿（Markowitz Efficient Frontier）]]：横轴通常是投资组合收益率的标准差，纵轴是预期收益率。
- [[Mean-Variance-Utility-Function|均值—方差效用函数（Mean-Variance Utility Function）]]：公式 $U=E(R)-\frac12 A\sigma^2$ 中的 $\sigma^2$ **是方差，不是标准差**；题目给出标准差时先平方。
- 本知识点也是数量方法（Quantitative Methods）的基础公式，后续在数量方法笔记中可通过链接引用，避免重复建立同内容文件。

## 当前掌握情况 / 复习检查

**状态：🟡 解析能懂，待独立验证**

- [ ] 不看资料写出总体 / 样本方差公式
- [ ] 知道样本使用 $n-1$，总体使用 $N$
- [ ] 能从方差正确算出标准差
- [ ] 能独立复算基金 A 的 $0.00143$ 和 $3.78\%$
- [ ] 能解释平方单位换算与题目 “0.14%” 的关系
