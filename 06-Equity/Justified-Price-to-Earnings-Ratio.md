---
subject: CFA Level I
topic: Equity Valuation — Justified Leading Price-to-Earnings Ratio
status: 持续更新
created: 2026-11-09
tags: [CFA-L1, Equity-Investments, Valuation, P-E, Gordon-Growth]
---

# Justified Leading P/E Ratio｜合理远期市盈率

[[06-Equity/INDEX|返回权益投资目录]] · [[06-Equity/Equity-Investments-Basics|权益投资基础概念]]

## 1. 三个概念：市盈率、远期市盈率、合理市盈率

- **P/E (Price-to-Earnings Ratio，市盈率)**：股票价格与每股收益之比。
- **Leading / Forward P/E（远期市盈率）**：当前价格 \(P_0\) 除以未来一期预期每股收益 \(E_1\)。
- **Trailing P/E（历史市盈率）**：当前价格除以过去一期或过去十二个月每股收益。
- **Justified P/E（合理市盈率）**：根据增长率、股息支付率和股权必要收益率等基本面指标，推导出理论上有依据的 P/E；不同于市场报价形成的实际交易市盈率。

### 1.1 基础 P/E：最重要的两个计算口径

\[
\boxed{P/E=\frac{\text{Share Price}}{\text{Earnings per Share (EPS)}}}
\]

在股数及利润口径匹配的简化条件下：

\[
\boxed{P/E=\frac{\text{Market Capitalization}}{\text{Earnings Available to Common Shareholders}}}
\]

- **Share Price（每股股价）**：观察日股票价格。
- **EPS（每股收益）**：归属于普通股股东的利润除以对应口径的加权平均普通股股数；应留意 Basic EPS 与 Diluted EPS 的差异。
- **Market Capitalization（股票总市值）**：股价乘对应时点股份总数。
- **P/E 是倍数而非百分比**。10× P/E 的含义是投资者愿意为每股 1 元盈利支付 10 元，不保证10年能实际收回股价。
- **股数口径提醒**：报告 EPS 可能用期间加权平均股数，而市值使用时点股数；若期间有回购、增发等，整体市值÷净利润与股价÷报告 EPS 未必精确相等。

### 1.2 历史 P/E 与远期 P/E 的计算

\[
\boxed{\text{Trailing P/E}=\frac{P_0}{E_0}}
\]

\[
\boxed{\text{Forward / Leading P/E}=\frac{P_0}{E_1}}
\]

- **Trailing P/E（历史／滚动市盈率）**：使用已实现 EPS；实务中常采用过去十二个月 EPS（TTM）。
- **Forward / Leading P/E（远期市盈率）**：使用未来一期预测 EPS，具有预测误差风险。
- **示例**：当前股价60元，历史 EPS 5元，下一期预期 EPS 6元。Trailing P/E=60/5=12×；Forward P/E=60/6=10×。股价相同，口径不同，市盈率就不同。

### 1.3 用 P/E 估计股价与估值高低

反推价格：

\[
\boxed{\text{Implied Price}=\text{Target P/E}\times\text{Forecast EPS}}
\]

- 例：预计下一期 EPS=6元，基于可比公司、增长及风险判断目标 P/E=10×，则隐含价格为60元。
- **不是 P/E 越低越便宜**：低 P/E 可能反映利润即将下滑、增长缓慢、风险较高或一次性收益抬高 EPS；高 P/E 也可能反映更高预期增长，但仍可能高估。
- **EPS 为零或负值**：普通 P/E 不具备常规经济解释或不适合比较；不能将负 P/E 直接认定为“更便宜”。
- **同口径比较**：比较不同公司市盈率时，应确认行业、增长率、风险、会计政策和 Trailing/Forward 期间可比。


### 1.4 公式符号与英文全称对照表（必背）

以下符号统一使用本专题的时间口径：下标 \(0\) = 当前或本期（Time 0 / Current Period）；下标 \(1\) = 下一期／未来一期（Time 1 / Next Period）。

| 符号或英文 | 英文全称 | 中文含义 | 用于哪种公式 |
|---|---|---|---|
| **P/E** | **Price-to-Earnings Ratio** | 市盈率；股价除以每股收益，通常以“倍（×）”表示 | 所有市盈率公式 |
| \(P\) | **Price per Share** | 每股价格／股价 | 基础 P/E |
| \(P_0\) | **Price at Time 0 / Current Share Price** | 当前（估值时点）的每股价格；在 Justified 公式中指合理理论价格 | Trailing、Leading、Justified |
| **Earnings** | **Earnings / Profit Attributable to Common Shareholders** | 盈利；通常关注归属于普通股股东的利润 | P/E 的收益口径 |
| **EPS** | **Earnings per Share** | 每股收益 | 基础 P/E |
| \(E_0\) | **Current / Trailing Earnings per Share** | 当期或最近一期／过去12个月每股收益（按具体题目时间口径） | Trailing P/E |
| \(E_1\) | **Expected Earnings per Share in the Next Period** | 下一期预期每股收益 | Leading P/E |
| \(D_1\) | **Expected Dividend per Share in the Next Period** | 下一期预期每股股息 | Gordon Growth Model、Payout |
| \(p\) | **Dividend Payout Ratio** | 股息支付率：预期每股股息占预期每股收益的比例 \(D_1/E_1\) | Justified P/E |
| \(b\) | **Retention Ratio / Plowback Ratio** | 利润留存率：净利润中未分红、留在企业中的比例 \(1-p\) | Sustainable Growth |
| \(r\) | **Required Return on Equity / Required Rate of Return** | 股权必要收益率；投资者对该股票要求的回报率／贴现率 | Gordon Growth、Justified P/E |
| \(g\) | **Sustainable / Constant Growth Rate** | 可持续增长率／恒定增长率（具体公式假设下） | Gordon Growth、Justified P/E |
| **ROE** | **Return on Equity** | 净资产收益率：公司为普通股股东权益创造收益的能力 | \(g=b\times ROE\) |
| **TTM** | **Trailing Twelve Months** | 过去连续12个月 | 实务中的 Trailing P/E |
| **Market Capitalization** | **Market Capitalization** | 股票总市值，通常等于每股市价 × 在外普通股数量 | 总市值口径 P/E |
| **Net Income** | **Net Income / Earnings Available to Common Shareholders** | 净利润；P/E整体口径应使用归属于普通股股东的利润 | 总市值口径 P/E |
| **Target P/E** | **Target Price-to-Earnings Multiple** | 目标市盈率；分析师选用的合理或参考估值倍数 | 反推股价 |
| **Forecast EPS** | **Forecast Earnings per Share** | 预测每股收益 | 反推股价 |

> **时间下标的注意点**：严格的 Trailing P/E 在实务中通常使用最近12个月 EPS，而教材公式写作 \(E_0\) 时可能代表最近一期已实现 EPS；做题以明确期间定义为准。**E 是 Earnings（收益），不是 Equity（股东权益）；P 是 Price（股价），不是 Payout（分红）。**

### 1.5 本专题全部重要公式与口径一览

**① 基础市盈率（Basic P/E）**

\[
\boxed{P/E=\frac{P}{EPS}}
\]

**② 市值口径（Aggregate P/E，需股数与盈利口径匹配）**

\[
\boxed{P/E\approx\frac{Market\ Capitalization}{Earnings\ Available\ to\ Common\ Shareholders}}
\]

**③ 历史市盈率（Trailing P/E）**

\[
\boxed{Trailing\ P/E=\frac{P_0}{E_0}}
\]

**④ 远期市盈率（Leading / Forward P/E）**

\[
\boxed{Leading\ P/E=\frac{P_0}{E_1}}
\]

**⑤ 戈登增长模型（Gordon Growth Model）**

\[
\boxed{P_0=\frac{D_1}{r-g}}
\]

**⑥ 股息支付率与留存率（Payout and Retention）**

\[
\boxed{p=\frac{D_1}{E_1}\qquad b=1-p}
\]

**⑦ 可持续增长率（Sustainable Growth Rate，简化条件）**

\[
\boxed{g=b\times ROE=(1-p)\times ROE}
\]

**⑧ 合理远期市盈率（Justified Leading P/E）**

\[
\boxed{\frac{P_0}{E_1}=\frac{p}{r-g}}
\]

**⑨ 合理历史市盈率（Justified Trailing P/E，稳定增长条件）**

\[
\boxed{\frac{P_0}{E_0}=\frac{p(1+g)}{r-g}}
\]

**⑩ 目标市盈率估算合理股价（Implied Share Price）**

\[
\boxed{Implied\ Price=Target\ P/E\times Forecast\ EPS}
\]

**公式适用边界**：Gordon Growth 相关公式需要长期恒定增长且 \(r>g\)；留存率与 ROE 对增长的关系依赖盈利能力、资本结构等条件；不盈利企业的普通 P/E 常缺乏常规解释力。比较估值时区分**实际市场 P/E**和**理论合理 P/E**。


## 2. 先从 Gordon Growth Model｜戈登增长模型推导

在股息以固定增长率 \(g\) 永续增长且 \(r>g\) 时：

\[
P_0=\frac{D_1}{r-g}
\]

两边除以下一期预期每股收益 \(E_1\)：

\[
\frac{P_0}{E_1}=\frac{D_1/E_1}{r-g}
\]

由于 \(D_1/E_1\) 是预期股息支付率（Dividend Payout Ratio，记为 \(p\)），得到：

\[
\boxed{\text{Justified Leading P/E}=\frac{p}{r-g}}
\]

其中：
- \(P_0\)：当前合理股价（Justified Price at Time 0）。
- \(E_1\)：下一期预期每股收益（Forward Earnings per Share, EPS）。
- \(D_1\)：下一期预期每股股息（Expected Dividend per Share）。
- \(p=D_1/E_1\)：Dividend Payout Ratio（股息支付率）。
- \(r\)：Required Return on Equity（股权必要收益率）。
- \(g\)：Sustainable Growth Rate（可持续增长率）。

**适用条件**：恒定股息增长、合理可持续的假设，以及 \(r>g\)。分母很小时估值对参数极其敏感，不能将模型结论机械应用到不稳定增长或不分红企业。

## 3. 影响 Justified Leading P/E 的三个变量

在**其他变量保持不变（All Else Equal）**的纯公式比较下：

| 变量 | 变化 | 对 Justified Leading P/E 的方向 |
|---|---|---|
| Dividend Payout Ratio（股息支付率） \(p\) | 增加 | 上升（假设 \(r,g\) 固定） |
| Required Return（必要收益率） \(r\) | 增加 | 下降 |
| Sustainable Growth（增长率） \(g\) | 增加 | 上升 |

但题目通常进一步考察 **p 和 g 可能相互影响**。

### 3.1 Retention Ratio and Sustainable Growth｜留存率与可持续增长

- **Retention Ratio / Plowback Ratio（收益留存率）**，记为 \(b\)，与股息支付率互补：

\[
\boxed{b=1-p}
\]

- 在 ROE 不变、增长由留存收益支持的简化条件下：

\[
\boxed{g=b\times ROE=(1-p)\times ROE}
\]

- 因此，**提高股息支付率 \(p\)** 会减少留存率 \(b\)，并可能使未来增长率 \(g\) 下降。

### 3.2 为什么股息支付率与 P/E 的关系可能不确定？

将 \(g=(1-p)ROE\) 代回：

\[
\text{Justified Leading P/E}
=\frac{p}{r-(1-p)ROE}
\]

提高 \(p\) 时：
1. **分子 \(p\) 增加** → 在其他条件不变时有利于 P/E 上升；
2. **\(g=(1-p)ROE\) 降低** → 分母 \(r-g\) 增加，不利于 P/E。

净影响取决于 \(r\) 与 \(ROE\) 的相对大小，不可一概而论。这说明股息支付率与 Justified P/E 存在 **Ambiguous Relation（不确定关系）**，也是本题标准答案。

**进一步代数判断（\(r>g\)，并保持 \(r,ROE\) 不变）**：

\[
\frac{\partial(\text{Leading P/E})}{\partial p}
=\frac{r-ROE}{[r-(1-p)ROE]^2}
\]

- \(r>ROE\)：提高 \(p\) 使 P/E 上升。
- \(r<ROE\)：提高 \(p\) 使 P/E 下降（在仍满足 \(r>g\) 的有效模型范围内）。
- \(r=ROE\)：P/E 不随 \(p\) 变化。

#### 两种方向的数值例子

固定必要收益率 \(r=10\%\)，分别考察两种 \(ROE\)：

| 情形 | \(ROE\) | 股息支付率 \(p\) | \(g=(1-p)ROE\) | 合理远期 P/E |
|---|---:|---:|---:|---:|
| 情形一 | 8% | 50% | 4.0% | \(0.5/(0.1-0.04)=8.33\) |
| 情形一 | 8% | 80% | 1.6% | \(0.8/(0.1-0.016)=9.52\) |
| 情形二 | 15% | 50% | 7.5% | \(0.5/(0.1-0.075)=20.00\) |
| 情形二 | 15% | 80% | 3.0% | \(0.8/(0.1-0.03)=11.43\) |

同样把股息支付率从50%提高至80%，合理远期 P/E 在第一种情形上升、第二种情形下降。故**关系不确定**。

## 4. Dividend Paid vs Dividend Payout Ratio｜股息金额与股息支付率

- **Dividend Paid / Dividends per Share（股息金额／每股股息）**：支付了多少现金股息。
- **Dividend Payout Ratio（股息支付率）**：股息占同期每股收益的比例：

\[
p=\frac{D_1}{E_1}
\]

**区别**：股息金额提高并不意味着 P/E 一定提高，因为 EPS、留存率、未来增长和必要收益率可能同时改变。仅仅把股息支付率提高、却假设增长率固定，才可直接断言 P/E 随支付率上升。因此选择题中的正向关系表述必须留意“其他条件不变”这一前提。

## 5. CFA 题目解析｜The justified leading P/E ratio ...

> The justified leading P/E ratio:
>
> A. is positively related to dividend paid.  
> B. is positively related to required rate of return.  
> C. has an ambiguous relation with dividend payout ratio.

**答案：C。**

- **A（不是最佳答案）**：在固定 \(E_1,r,g\) 的条件下，预期股息支付更多可提高理论合理 P/E。但在财务政策变化的实际场景中，更高分红会减少留存、影响可持续增长，因而不能不加条件地认定正相关。另外股息支付额与股息支付率不是同一概念。
- **B（错误）**：\(\text{P/E}=p/(r-g)\)，当 \(r\) 上升且其他因素不变时，分母增大，P/E 应**下降（Negatively Related）**。
- **C（正确）**：提高支付率同时可能压低长期增长率，二者对 P/E 的影响方向相反，最终结果视 \(r\) 与 \(ROE\) 等条件而定。

### 重要措辞提醒

单看 \(\text{P/E}=p/(r-g)\) 并**保持 \(g\) 不变**，可以说股息支付率与 P/E 正相关。题目并未为 A 加上这些条件，且 C 考查的是增长随留存率内生变化的更完整关系。学习时必须将两个比较的假设条件分清，不能认为“公式中分子变大”就证明在所有情形下 P/E 必然变大。

## 6. Leading vs Trailing P/E｜远期市盈率与历史市盈率

**Justified Leading P/E**：

\[
\boxed{\frac{P_0}{E_1}=\frac{p}{r-g}}
\]

在 \(E_1=E_0(1+g)\) 等增长假设成立时，**Justified Trailing P/E**：

\[
\boxed{\frac{P_0}{E_0}=\frac{p(1+g)}{r-g}}
\]

**考试陷阱**：Leading 使用下一期预期 \(E_1\)，Trailing 使用当期／过去一期 \(E_0\)，二者不要漏掉 \(1+g\) 因子。

## 7. Review Checklist｜复习清单

- [ ] 能解释 P、E、EPS、P₀、E₀、E₁、D₁、p、b、r、g、ROE、TTM 的英文全称及中文含义
- [ ] 能写出 P/E = Price / EPS，并区分 Trailing 与 Forward 的 EPS 口径
- [ ] 能用 Target P/E × Forecast EPS 估算股价，理解负 EPS 与低 P/E 陷阱
- [ ] 能从 Gordon Growth Model 推导合理远期 P/E
- [ ] 能区分 Dividend Paid（金额）与 Dividend Payout Ratio（比例）
- [ ] 能写出 \(b=1-p\) 和 \(g=b\times ROE\)
- [ ] 能解释为何 \(p\) 提高可能同时降低 \(g\)
- [ ] 能证明 \(r\) 与 P/E 反向变化（其他变量不变）
- [ ] 能区分 Leading 与 Trailing P/E 的公式

**一句话速记**：Justified Leading P/E = Payout / (Required Return − Growth)；Payout ↑ → Direct Effect Positive but Growth Effect Negative → **Ambiguous Overall**。

## Reference｜资料依据

- CFA Institute (2026), [Discounted Dividend Valuation](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/discounted-dividend-valuation)。
- CFA Institute (2026), [Market-Based Valuation: Price and Enterprise Value Multiples](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/market-based-valuation-price-enterprise-value-multiples)。
