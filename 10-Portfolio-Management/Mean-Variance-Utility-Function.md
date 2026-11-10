---
subject: Portfolio Management
topic: Mean-Variance Utility Function and Risk Aversion
status: "🟡 解析能懂，待独立验证"
created: 2026-11-10
last-reviewed: 2026-11-10
tags: [CFA-L1, Portfolio-Management, Utility-Theory, Risk-Aversion]
---

# 效用理论与均值—方差效用函数（Utility Theory & Mean-Variance Utility Function）

[[10-Portfolio-Management/INDEX|← 返回投资组合管理目录]]

## 一句话理解

在 CFA 常见的**均值—方差效用模型（Mean-Variance Utility Model）**中，投资者既关心预期收益（Expected Return），也关心风险（Risk）；对于**风险厌恶型投资者（Risk-Averse Investor）**，在其他条件不变时，风险越高，效用（Utility）越低。

## 核心公式与变量

$$
\boxed{U=E(R)-\frac{1}{2}A\sigma^2}
$$

| 符号 | 英文 | 含义 |
|---|---|---|
| $U$ | Utility | 模型下投资者赋予资产或组合的效用评分（按收益率单位表示） |
| $E(R)$ | Expected Return | 预期收益率 |
| $A$ | Risk Aversion Coefficient | 风险厌恶系数 |
| $\sigma$ | Standard Deviation | 收益率标准差 |
| $\sigma^2$ | Variance | 收益率方差 |

分解：

$$
U=\underbrace{E(R)}_{\text{收益带来的效用}}-
\underbrace{\frac{1}{2}A\sigma^2}_{\text{风险惩罚项}}
$$

**计算单位要一致：**将收益率与标准差统一用小数代入（例如 $10\%=0.10$，$20\%=0.20$），避免把 $20$ 直接平方使用。

## 风险厌恶系数 A 如何理解？

- $A>0$：**Risk-Averse（风险厌恶）**；同等预期收益下，风险越高，效用越低。
- $A=0$：**Risk-Neutral（风险中性）**；在这个模型中，效用只取决于预期收益。
- $A<0$：**Risk-Seeking（风险偏好）**；在这个模型中，方差项增加效用。

对于相同的风险资产，当 $A>0$ 且 $\sigma^2>0$，$A$ 越大，风险惩罚越重。**风险厌恶程度不同的人可能作出不同资产选择。**

## 无风险资产为什么与 A 无关？（本题核心）

在本题的理论模型中，无风险资产（Risk-Free Asset）的收益是确定的，因此：

$$
\sigma_f^2=0
$$

代入：

$$
U_f=E(R_f)-\frac12 A(0)=\boxed{R_f}
$$

因此，**同一个无风险收益率**在这个标准化均值—方差公式中，对不同风险厌恶系数 $A$ 的投资者给出的效用评分相同。

**限制条件：**这不是说现实中所有人的财富效用、消费偏好都相同；只是在采用同一个归一化公式、面对同一无风险收益率时，风险惩罚项为零。

## 典型选择题：哪项关于效用理论的说法正确？

题目要点：“Which of the following statements relating to utility theory is most likely correct?”

- **A. A risk-free asset will generate the same utility for all individuals.（正确）** 在本题使用的均值—方差效用公式下，同一无风险收益率有 $U_f=R_f$，不依赖 $A$。
- **B. A risk-free asset's utility is dependent on the investor's risk attitude.（错误）** 因为 $\sigma_f^2=0$，$A$ 项消失。
- **C. A risk-free asset has a variance of nonzero.（错误）** 理论上无风险收益率的方差为零。

**正确答案：A（限于题设模型）。**

## 数字例题 1：无风险资产 vs 风险资产

假设：

- 无风险资产：$R_f=4\%$，$\sigma_f=0$；
- 风险资产：$E(R)=10\%$，$\sigma=20\%$；
- 某投资者 $A=2$。

无风险资产：

$$
U_f=0.04-\frac12(2)(0)^2=0.04=4\%
$$

风险资产：

$$
U_{\mathrm{risky}}=0.10-\frac12(2)(0.20)^2=0.06=6\%
$$

在这些候选资产中，$A=2$ 的投资者对风险资产有更高的模型效用评分。

若风险厌恶系数改成 $A=4$：

$$
U_{\mathrm{risky}}=0.10-\frac12(4)(0.20)^2=0.02=2\%
$$

无风险资产的评分仍为 $4\%$，风险资产的评分降至 $2\%$；在两者之间，该投资者更偏好无风险资产。

## 数字例题 2：预期收益高不一定效用高

给定 $A=4$：

| 组合 | 预期收益率 $E(R)$ | 标准差 $\sigma$ |
|---|---:|---:|
| 组合 A | 8% | 10% |
| 组合 B | 12% | 25% |

$$
U_A=0.08-\frac12(4)(0.10)^2=0.06=6.0\%
$$

$$
U_B=0.12-\frac12(4)(0.25)^2=-0.005=-0.5\%
$$

虽然组合 B 的预期收益率更高，但其风险惩罚更大，**在该投资者的效用评分中组合 A 更优**。

注意：负的效用评分**不等于**投资组合的实际回报为负，它只是此模型下的风险调整评价结果。

## 考试判断路径与易错点

1. 看到 **Utility Theory / Risk Aversion**，先写 $U=E(R)-\frac12 A\sigma^2$。
2. 看到 **Risk-Free Asset**，马上代入 $\sigma=0$，得到 $U=R_f$，与 $A$ 无关。
3. 题目问哪项资产更受偏好时，**分别计算效用值并比较**；不能仅看预期收益率大小。
4. 注意区分 **Standard Deviation（标准差，$\sigma$）**与 **Variance（方差，$\sigma^2$）**。题目给的是标准差时，务必先平方。
5. 不要把“对所有投资者效用相同”扩大为普遍效用理论的结论；其成立依赖题目给定的均值—方差模型及相同的无风险收益率。
6. **本题公式属于特定的均值—方差效用表述**，不能把效用评分直接等同于实际实现的收益率。

## 关联知识 / Obsidian 链接

- [[Time-Weighted-Return|时间加权收益率（Time-Weighted Return, TWR）]]：TWR 衡量多期间复利投资表现，与本题的效用理论不是同一类公式。
- 后续可连接：**无差异曲线（Indifference Curve）**、**最优投资组合（Optimal Portfolio）**、**风险收益权衡（Risk–Return Trade-off）**。

## 我的错因 / 验证记录

- 本次题目选 A 正确。后续需巩固：**无风险资产方差为零，因此风险厌恶系数 A 不再影响效用评分**。
- [ ] 能闭卷写出效用函数并解释每个变量
- [ ] 能解释为什么无风险资产对 A 不敏感
- [ ] 能正确区分标准差与方差并代入小数
- [ ] 能独立比较两个组合的效用评分
- [ ] 能说明此结论的模型适用范围
