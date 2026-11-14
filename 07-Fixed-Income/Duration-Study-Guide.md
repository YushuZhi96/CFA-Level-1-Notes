---
subject: Fixed Income
topic: Duration and Interest Rate Risk
status: 持续更新
created: 2026-11-14
tags: [CFA-L1, Fixed-Income, Duration, Interest-Rate-Risk]
---

# Duration 专题｜债券久期与利率风险

> CFA Level I 复习主入口：将已有 [[Macaulay-Duration]]、[[Modified-Duration]]、[[Key-Rate-Duration]] 及本次新整理的 Effective Duration 合并成一套完整的学习框架。原专项文件保留，便于按概念深入复习。

## 1. 最重要的总览：Duration 到底衡量什么？

Duration（久期）常用于衡量债券对利率变动的敏感性；不同久期的定义、适用场景不同。

| 指标 | 中文 | 回答的问题 | 最典型的使用情景 |
|---|---|---|---|
| **Macaulay Duration** | 麦考利久期 | 现金流按现值加权后，平均何时收回？ | 固定现金流债券的平均收款时间 |
| **Modified Duration** | 修正久期 | YTM 变动，债券价格约变化多少？ | 现金流固定、无利率敏感型期权 |
| **Effective Duration** | 有效久期 | 基准利率变动且现金流可能改变，价格约变化多少？ | Callable / Putable / MBS 等 |
| **Key Rate Duration (KRD)** | 关键利率久期 | 收益率曲线某个特定期限节点变化，价格受多大影响？ | 分析非平行曲线变动 |

**速记口诀**：Macaulay 看**时间**；Modified 看**固定现金流下的价格敏感度**；Effective 看**利率可能改变现金流时的敏感度**；Key Rate 看**哪个期限节点的利率变化**。

## 2. Macaulay Duration｜麦考利久期

**核心定义**：债券各期现金流（Cash Flows）以其现值占债券价格的比例加权后的平均收款时间。

\[
\boxed{D_{Mac}=\sum_{t=1}^{N}t\frac{PV(CF_t)}{P}}
\]

- \(PV(CF_t)\)：第 \(t\) 期现金流现值；\(P=\sum PV(CF_t)\) 为债券价格。
- 若 \(t\) 用付息期数计算，算出来的单位就是“期”；要除以每年付息次数 \(m\) 才是“年”。
- 一般的固定正现金流债券：零息债券（Zero-Coupon Bond）的 Macaulay Duration = 到期期限（Maturity）；定期付息债券的 Macaulay Duration 通常小于其到期期限。
- 它的定义是**时间加权**，不能直接拿它替代 Modified Duration 估计收益率变动引发的价格百分比变化。

**直觉**：现金流越早收到，现值权重越靠前，Macaulay Duration 通常越短。

详见：[[Macaulay-Duration]]。

## 3. Modified Duration｜修正久期

**核心定义**：衡量**现金流保持不变**时，债券价格对到期收益率（Yield to Maturity, YTM）微小变化的敏感程度。

当 Macaulay Duration 以年计、年化 YTM 为 \(y\)、每年复利/付息次数为 \(m\)：

\[
\boxed{D_{Mod}=\frac{D_{Mac}}{1+y/m}}
\]

价格变化一阶近似：

\[
\boxed{\frac{\Delta P}{P}\approx-D_{Mod}\Delta y}
\]

- \(\Delta y\) 以小数表示：50 bps = 0.005；100 bps = 0.01。
- **负号**：通常 YTM 上升，价格下降；YTM 下降，价格上升。
- **例题**：Modified Duration = 5，YTM 上升 50 bps，则价格约变化 \(-5\times0.005=-2.5\%\)。
- 这是小幅变动下的一阶近似；变动较大时还要考虑 Convexity（凸性）。
- **前提**：未来合同现金流不因利率变化而发生变化。对于含利率敏感型赎回/回售条款的债券，单靠 Modified Duration 往往不够。

详见：[[Modified-Duration]]。

## 4. Effective Duration｜有效久期

**核心定义**：衡量债券价格相对于**基准收益率曲线（Benchmark Yield Curve）**变化的敏感性，并允许预期现金流在利率变化后重新估计。

\[
\boxed{D_{Eff}=\frac{PV_- - PV_+}{2PV_0\Delta Curve}}
\]

- \(PV_0\)：当前债券价格。
- \(PV_-\)：基准曲线下移 \(\Delta Curve\) 后，**重新估计现金流并重新估值**所得价格。
- \(PV_+\)：基准曲线上移 \(\Delta Curve\) 后，**重新估计现金流并重新估值**所得价格。
- \(\Delta Curve\) 使用小数，如 25 bps = 0.0025；该形式通常考察基准曲线**平行移动**。
- **关键词**：Uncertain Future Cash Flows（未来现金流不确定）、Interest-Sensitive Embedded Options（利率敏感型嵌入期权）。

适用例子：

- **Callable Bond（可赎回债券）**：利率下降时发行人可能提前赎回，预期未来票息期数减少；因此价格上涨可能受到限制。
- **Putable Bond（可回售债券）**：利率上升时持有人可能行使回售权，从而改变未来现金流。
- **Mortgage-Backed Securities (MBS，抵押贷款支持证券)**：市场利率变化可能改变提前还款（Prepayment）速度，从而改变投资者实际收到本金的时间。

**简化计算例子**：假设 \(PV_0=100\)，曲线上移25 bps 后 \(PV_+=98\)，下移25 bps 后 \(PV_-=102\)：

\[
D_{Eff}=\frac{102-98}{2(100)(0.0025)}=8
\]

这表示对小幅的基准利率变动，债券价格的敏感度约为8，而不是说“平均8年收回现金流”。

**注意**：并非只要现金流含不确定性就一定选择有效久期；核心是**预期现金流可能随利率变化**，且估值模型允许这种变化。对现金流固定且其他假设一致的债券，Effective Duration 通常与 Modified Duration 相近。

## 5. Key Rate Duration｜关键利率久期

**核心定义**：衡量收益率曲线上**某一个特定期限节点的利率**变化时，债券或投资组合的价格敏感度；其他关键节点尽量保持不变。

\[
\boxed{KRD_i\approx\frac{P_i^- - P_i^+}{2P_0\Delta r_i}}
\]

- \(P_i^-\) 与 \(P_i^+\)：只对第 \(i\) 个关键期限节点利率分别下调、上调 \(\Delta r_i\) 后重估的价格。
- \(P_0\)：当前债券/组合价值。
- **用途**：识别收益率曲线非平行移动（Non-Parallel Shift）带来的风险，例如2年期收益率上升、10年期收益率下降。
- 不能把某一个期限节点的 KRD 误当作整只债券的总久期。
- **补充**：在节点划分和曲线扰动一致的适用框架下，各节点 KRD 之和可近似对应总的平行曲线久期，但不应把此作为在所有模型中无条件精确成立的恒等式。

详见：[[Key-Rate-Duration]]。

## 6. 四种久期之间的区别：同一题如何选？

| 题干关键词（英文） | 中文理解 | 选用 |
|---|---|---|
| Weighted Average Time / Present Value Weights | 现金流现值加权平均时间 | **Macaulay** |
| Fixed Cash Flows / YTM Sensitivity | 固定现金流下对YTM变化的敏感度 | **Modified** |
| Uncertain Future Cash Flows / Callable / Putable / MBS | 利率变化使预期现金流可能改变 | **Effective** |
| Specific Maturity Node / Non-Parallel Shift | 特定期限节点利率变化、非平行变动 | **Key Rate** |

**常见陷阱**：
1. Duration 不等于 Maturity；Macaulay 也只有在零息债等特定结构下才等于到期期限。
2. 修正久期的 \(\Delta y\) 必须是收益率的**绝对变动量**（小数）；上升1个百分点是0.01，不是1。
3. Modified 与 Effective 不是只差一个计算公式：**前者固定现金流，后者允许按利率情景重新建模现金流**。
4. Effective Duration 通常用于基准曲线变化；Modified Duration 通常基于债券 YTM；不能在不同基准和信用利差假设下随意替换。
5. Key Rate Duration 不是另一种“平均期限”，而是不同收益率曲线节点的风险分解。
6. 大幅利率变化时，单用一阶久期近似可能有误差，需要考虑 Convexity。

## 7. Duration 与 Convexity｜久期与凸性的联系

一阶近似：

\[
\frac{\Delta P}{P}\approx-D\Delta y
\]

加入凸性后的常用二阶近似：

\[
\frac{\Delta P}{P}\approx-D_{Mod}\Delta y+\frac12 Convexity(\Delta y)^2
\]

- 这条式子是对**固定现金流债券、相应 YTM 口径下**的常见近似形式。
- 对含期权债券进行利率风险分析时，应使用与定价模型及曲线变动一致的有效久期和相应的有效凸性（Effective Convexity）度量。
- 这里先记住“久期是一阶敏感度，凸性修正曲线弯曲造成的误差”；凸性的深入计算可另作专题。

## 8. CFA 真题型练习与速判

**题型一：For bonds with uncertain future cash flows, which duration is most suitable to measure interest rate risk?**

- A. Macaulay Duration
- B. Modified Duration
- C. Effective Duration

**正确答案 C**。因为未来现金流可能随利率变化，需要在利率上下行情景中重新估计并重新定价。

**题型二：A bond has Modified Duration 5; its YTM rises by 50 bps. Estimate the price change.**

\[
\frac{\Delta P}{P}\approx-5\times0.005=-2.5\%
\]

**题型三：The 2-year yield rises while the 10-year yield falls. Which measure identifies exposures by maturity?**

选择 **Key Rate Duration**。总久期一个数不足以完整描述不同期限节点的风险。

**题型四：Which duration measures the present-value-weighted average time to receive a bond's cash flows?**

选择 **Macaulay Duration**。

## Duration 与价格风险、再投资风险及 Immunization

- **Price Risk（价格风险）**：收益率上升通常导致债券市场价格下降；Modified/Effective Duration 用于近似衡量价格对利率的敏感度。
- **Reinvestment Risk（再投资风险）**：收益率下降时，未来收到的票息可能只能以更低利率投资，降低持有期末的累积金额。
- **两种效应方向相反**：利率上升时价格效应不利但再投资效应可能有利；利率下降时价格效应有利但再投资效应可能不利。
- **Duration Matching（久期匹配）与 Immunization（免疫策略）**：通过使资产久期与目标负债或投资期限相匹配等条件，尽量让小幅利率变动带来的价格效应与再投资效应相互抵消。免疫策略还受初始收益率、现金流匹配、凸性、曲线非平行变化和再平衡等条件影响，不能仅凭一个久期数值保证完全免疫。
- **CFA 速判**：普通付息债券 + Hold to Maturity + Payments Made as Promised → 在 Market Price Risk、Reinvestment Risk、Default Risk 三者中优先选择 **Reinvestment Risk**。

详见 [[Fixed-Income-Basics]] 的 “Interest Rate Risk Components｜利率风险的组成”。

## 9. 10秒考前记忆卡

- **Macaulay = Time**：现金流现值加权平均时间。
- **Modified = YTM Sensitivity**：现金流固定，价格对YTM敏感度。
- **Effective = Option-sensitive Cash Flows**：利率变化可改变现金流，重估价格。
- **Key Rate = Curve Node**：某期限节点的利率风险。
- **Duration × Yield Change ≈ Price Change**：通常反向，注意负号。
- **Convexity**：大幅利率变动时用于改进价格变动近似。

---

## 相关专项笔记

- [[Macaulay-Duration|麦考利久期]]
- [[Modified-Duration|修正久期]]
- [[Key-Rate-Duration|关键利率久期]]
- [[Embedded-Options-in-Bonds|嵌入式期权债券]]
- [[Fixed-Income-Basics|固定收益基础概念]]
