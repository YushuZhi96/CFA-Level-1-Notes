---
subject: Portfolio Management
topic: Indifference Curve
status: "🟡 解析能懂，待独立验证"
created: 2026-11-10
last-reviewed: 2026-11-10
tags: [CFA-L1, Portfolio-Management, Indifference-Curve, Utility-Theory, Risk-Aversion]
---

# 无差异曲线（Indifference Curve）

[[10-Portfolio-Management/INDEX|← 返回投资组合管理目录]]

## 一句话理解

**无差异曲线（Indifference Curve）**表示：对同一位投资者而言，能够带来**相同效用水平（Same Utility Level）**的不同风险—预期收益组合。

在常见的风险—收益图中，投资者愿意承担更高风险，但需要获得更高预期收益作为补偿，才能保持效用不变。

## 一、从效用函数推导无差异曲线

之前学习的均值—方差效用函数（Mean-Variance Utility Function）：

$$
\boxed{U=E(R)-\frac12 A\sigma^2}
$$

其中：
- $U$：效用（Utility）；
- $E(R)$：预期收益率（Expected Return）；
- $A$：风险厌恶系数（Risk Aversion Coefficient）；
- $\sigma$：收益率标准差（Standard Deviation）；
- $\sigma^2$：收益率方差（Variance）。

对于同一条无差异曲线，效用 $U$ 固定。移项得到：

$$
\boxed{E(R)=U+\frac12 A\sigma^2}
$$

这就是本题的关键变形。

若横轴取**方差** $\sigma^2$，纵轴取预期收益率 $E(R)$，可写成直线形式：

$$
y=\underbrace{U}_{\text{截距}}+
\underbrace{\frac12 A}_{\text{斜率}}\underbrace{x}_{\sigma^2}
$$

因此：
- **Intercept（截距）= $U$：代表投资者的效用水平。**
- **Slope（斜率）= $A/2$：代表风险厌恶系数的一半。**

## 二、坐标轴要看清：方差 vs 标准差

CFA 图形和题目可能用方差或标准差作为风险轴，斜率表达式会不同。

### 横轴为方差 $\sigma^2$

$$
E(R)=U+\frac12 A\sigma^2
$$

- 截距：$U$；
- 斜率：$A/2$；
- 图形：在 $E(R)$—$\sigma^2$ 坐标下为直线（$A$ 固定时）。

### 横轴为标准差 $\sigma$

$$
E(R)=U+\frac12 A\sigma^2
$$

此时它是关于 $\sigma$ 的二次曲线，而不是直线。对 $\sigma$ 求导：

$$
\boxed{\frac{dE(R)}{d\sigma}=A\sigma}
$$

- 截距仍然是 $U$；
- 曲线斜率（边际补偿要求）为 $A\sigma$，会随风险水平变化；
- 对风险厌恶者（$A>0$），曲线向上且凸。

**考试提醒：**无论风险轴用标准差还是方差，令风险为零时，截距都是 $U$；但不能不看横轴就直接说斜率是 $A/2$。

## 三、无差异曲线如何解读？

1. **同一条曲线（Same Curve）**：曲线上所有组合对该投资者具有相同效用。
2. **更高的曲线（Higher Indifference Curve）**：在通常的风险—收益坐标中，代表更高效用；投资者更偏好。
3. **向上倾斜（Upward Sloping）**：风险增加时，投资者要求更高预期收益，才能维持相同效用。
4. **风险厌恶程度更高（Higher Risk Aversion）**：在相同风险水平下，需要更高的预期收益补偿额外风险；在标准差坐标下曲线更陡（给定 $\sigma>0$）。
5. **不同效用水平（Different Utility Levels）**：同一投资者可以有多条无差异曲线，每条曲线代表一个不同的效用水平；曲线之间不应混为一条。

## 四、典型 CFA 选择题：截距代表什么？

题目：*Which of the following statements about the indifference curve is most accurate?*

- **A. The slope represents the utility for the investor.（斜率代表投资者效用。）**
  - 错误。斜率体现风险厌恶程度及风险补偿要求，不是效用水平本身。
- **B. The intercept term represents the utility for the investor.（截距项代表投资者效用。）**
  - **正确答案 B。** 将效用函数变形为 $E(R)=U+\frac12 A\sigma^2$，风险轴为零时，纵轴截距为 $U$。
- **C. The intercept term is determined by the risk-free rate.（截距项由无风险利率决定。）**
  - 错误。截距由该条无差异曲线对应的效用水平 $U$ 决定，并非由无风险利率直接决定。

**易错提醒：**如果某条无差异曲线恰好经过无风险资产点 $(\sigma=0,E(R)=R_f)$，则该条曲线的效用截距数值会等于 $R_f$；这是曲线经过该点时的结果，不表示一般情况下截距由无风险利率决定。

## 五、数字例子：同一效用水平

假设投资者风险厌恶系数 $A=4$，希望维持效用 $U=4\%$。

$$
E(R)=0.04+\frac12(4)\sigma^2
$$

若标准差为 $10\%$：

$$
E(R)=0.04+2(0.10)^2=0.06=\boxed{6\%}
$$

若标准差为 $20\%$：

$$
E(R)=0.04+2(0.20)^2=0.12=\boxed{12\%}
$$

所以，组合风险从 $10\%$ 增加到 $20\%$ 时，投资者需要的预期收益率从 $6\%$ 提高到 $12\%$，才能保持相同的 $4\%$ 效用水平。

这两个风险—收益点位于同一条无差异曲线上。

## 六、与有效前沿（Efficient Frontier）的关系

- **Markowitz Efficient Frontier（马科维茨有效前沿）**：由可行资产组合的收益、风险、相关性及投资限制决定，显示风险—收益有效的组合。
- **Indifference Curve（无差异曲线）**：由某位投资者的效用函数与风险偏好决定，显示对该投资者而言效用相同的组合。
- **Optimal Portfolio（最优投资组合）**：在标准均值—方差图中，通常是投资者能够达到的最高无差异曲线与有效前沿相切的位置（在常见凸性、可行性等条件下）。

记忆：
**有效前沿告诉你“有哪些有效组合”；无差异曲线告诉你“投资者偏好哪些风险—收益组合”；两者结合决定最优选择。**

关联笔记：
- [[Mean-Variance-Utility-Function|效用理论与均值—方差效用函数]]
- [[Markowitz-Efficient-Frontier|马科维茨有效前沿]]

## 七、考试速记与复习检查

| 关键词 | 记忆 |
|---|---|
| Same Indifference Curve | 相同效用 |
| Intercept | 效用水平 $U$ |
| Slope（横轴为方差） | $A/2$ |
| Slope（横轴为标准差） | $A\sigma$，随风险变化 |
| Higher Indifference Curve | 更高效用 |
| Higher Risk Aversion | 对额外风险要求更高收益补偿 |

- [ ] 能从 $U=E(R)-\frac12 A\sigma^2$ 推导无差异曲线方程
- [ ] 能解释为什么截距代表效用水平
- [ ] 能区分方差横轴和标准差横轴下的斜率
- [ ] 能解释风险厌恶程度如何影响无差异曲线
- [ ] 能区分无差异曲线与 Markowitz 有效前沿
- [ ] 能解释二者相切点为什么代表常见模型下的最优组合
