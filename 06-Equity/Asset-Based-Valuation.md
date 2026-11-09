---
subject: CFA Level I
topic: Equity Valuation — Asset-Based Valuation
status: 持续更新
created: 2026-11-09
tags: [CFA-L1, Equity, Asset-Based-Valuation, Fair-Value, Liquidation]
---

# Asset-Based Valuation｜资产基础估值法

[[06-Equity/INDEX|返回权益投资目录]] · [[06-Equity/Equity-Investments-Basics|权益投资基础概念]] · [[06-Equity/Justified-Price-to-Earnings-Ratio|P/E估值专题]]

## 1. 定义与公式

**资产基础估值法（Asset-Based Valuation）**：用公司资产价值与负债价值之间的差额估计股权价值（Equity Value），关注资产及负债本身的经济价值，而不是直接从未来股息或利润倍数推导。

\[
\boxed{V_E=FV_A-FV_L}
\]

| 符号 | 英文全称 | 中文 |
|---|---|---|
| \(V_E\) | Equity Value | 股权价值 |
| \(FV_A\) | Fair Value of Assets | 资产公允价值 |
| \(FV_L\) | Fair Value of Liabilities | 负债公允价值 |
| \(FV\) | Fair Value | 公允价值 |

**例**：某公司所有资产的估计公允价值为1000万元，负债公允价值600万元，则理论股权价值约400万元。实际估值需要考虑未确认负债、资产计量、交易费用等具体情形。

### Fair Value vs Book Value｜公允价值与账面价值

- **Fair Value（公允价值）**：根据适用计量原则，估计市场参与者在当前市场条件下对资产和负债的价值。
- **Book Value（账面价值）**：按照会计准则和企业报表计量政策确认的资产或负债金额，可能基于历史成本、摊余成本或公允价值等口径。
- 二者不一定相同。例如一项房地产账面金额200万元，但估计公允价值500万元，资产基础估值时可能需要调整价值。
- **Adjusted Net Asset Value (ANAV，调整后净资产价值)**：重新估计资产、负债价值再计算净资产，常作为资产基础估值的一种实际方法。

## 2. 哪些企业更适合使用？

| 公司类型 | 适用性 | 原因 |
|---|---|---|
| 接近清算的公司（Approaching Liquidation） | **通常适合** | 未来持续经营现金流不再是主要估值基础，资产出售价值重要 |
| 部分金融公司（Financial Institutions） | **可能适合** | 主要资产为贷款、证券等金融资产，经济价值可能较易估计；还需审慎评估信用风险、隐含负债及会计差异 |
| 房地产持有、自然资源类公司（Asset-Heavy Businesses） | **可能适合** | 不动产、资源等资产在具备合理价值估计时可用于资产基础估值 |
| 无形资产占价值很高的公司（Intangible-Asset-Intensive Businesses） | **可能不适合仅使用此法** | 品牌、客户关系、知识产权、组织能力等价值可能未完全在报表反映或难以单独估计 |

**重要判断**：“金融公司”不是资产基础估值法不适用的统一类别。银行等金融机构常具有金融资产、负债基础，净资产及其价值调整是有意义的估值信息。但具体贷款、信用敞口、商誉等估值仍有难度。

### Intangible Assets｜无形资产的局限

- 知识产权（Intellectual Property）、品牌（Brand）、客户关系（Customer Relationships）等可能难以单项准确估值。
- 企业持续经营（Going Concern）所产生的协同和未来增长机会（Growth Opportunities）不一定等于简单的分项净资产价值。
- 因而，对于主要价值来自无形资产的企业，常需要结合 Discounted Cash Flow (DCF，现金流折现法) 等其他方法。

### Liquidation Value vs Fair Value｜清算价值与公允价值

- **Liquidation Value（清算价值）**：企业停止经营并出售资产、偿还债务后可为股东留下的价值，需考虑出售期限、清算费用及适用的债权清偿优先顺序。
- 清算情形下的售价不一定等同于正常有序交易条件下的 Fair Value，尤其快速出售或被迫出售时可能折价。
- Asset-Based Approach 适于评估清算企业，但应使用**与清算场景一致**的价值估计及成本调整，而不能一律直接等同账面净资产。

## 3. 与其他股票估值方法比较

| 方法 | 英文 | 估值基础 | 典型应用 |
|---|---|---|---|
| 资产基础法 | Asset-Based Valuation | 资产价值 − 负债价值 | 清算、资产价值较易估计 |
| 现值法 | Present Value / Discounted Cash Flow (DCF) | 未来现金流折现 | 盈利与未来现金流可预测的持续经营企业 |
| 相对估值法 | Relative Valuation / Multiples | P/E、P/B、EV/EBITDA等倍数 | 对比类似公司与市场估值 |

### Present Value vs Multiplier Models｜现值模型与乘数模型的理论依据

**Present Value Model（现值模型）**：从未来股息或股权自由现金流等经济利益出发，将预计现金流折现到当前，得到绝对估值（Absolute Valuation）。例如，在股息长期稳定增长且 \(r>g\) 时：

\[
\boxed{P_0=\frac{D_1}{r-g}}
\]

- \(P_0\)：Intrinsic Value at Time 0（当前内在价值）。
- \(D_1\)：Expected Dividend per Share（下一期预期每股股息）。
- \(r\)：Required Rate of Return（必要收益率）。
- \(g\)：Constant Growth Rate（稳定股息增长率）。

**Multiplier Model（乘数模型）**：通过价格相对于某个财务指标的倍数来进行估值，例如 P/E（Price-to-Earnings Ratio，市盈率）、P/B（Price-to-Book Ratio，市净率）。可比公司法（Method of Comparables）典型地以 Law of One Price（一价定律）为经济依据：

\[
\boxed{\text{Implied Share Price}=\text{Comparable P/E}\times\text{Forecast EPS}}
\]

- **Comparable P/E**：可比公司参考市盈率。
- **Forecast EPS**：预测每股收益（Forecast Earnings per Share）。

**Law of One Price（一价定律）**：在理想无套利条件下，具有相同未来现金流和风险的金融资产应具有相同价格。用于相对估值时，要求可比标的在风险、增长、盈利质量等方面真正足够相似；同一行业不代表必定同价或具有相同 P/E。

**重要理论区分**：Present Value Model 的直接逻辑是 Future Benefits Discounted to Present Value（未来收益折现）；Method of Comparables 的典型经济依据是 Law of One Price。根据预测基本面推导合理估值倍数（Fundamentals-Based Multiples）又可以利用 DCF 思路，因此不能笼统宣称所有乘数模型只使用一价定律。

#### 为什么两种方法可能得出不同估值？

| 维度 | Present Value Model | Multiplier Model / Method of Comparables |
|---|---|---|
| 主要输入 | 预计股息／现金流、增长率、贴现率 | 可比公司市场估值倍数、目标公司 EPS 等指标 |
| 典型逻辑 | Absolute Valuation（绝对估值） | Relative Valuation（相对估值） |
| 主要敏感因素 | 现金流预测、折现率、永续增长假设 | 可比公司选取、市场定价、风险和增长差异 |
| 可能结论 | 以预计未来现金流推算的内在价值 | 相对于同行可比证券的隐含价值 |

**同一目标公司的教学假设**：
- 现值模型：\(D_1=2\)元，\(r=9\%\)，\(g=4\%\)，则 \(P_0=2/(0.09-0.04)=40\)元。
- 乘数模型：目标公司 Forecast EPS=4元，参考同行 Comparable P/E=15倍，则估计价值 \(P=15\times4=60\)元。
- **40元与60元并不矛盾**：它们使用的假设和信息来源不同；也不能由此直接证明哪一个模型正确。模型与输入估计即使都合理，也可能得出不完全一致的数值和投资建议。

#### 本题：Law of One Price 是否保证两种估值结论相同？

> An analyst states that since the rationale behind multiplier model and present value are both the law of one price, those two methods will generate same conclusion on valuation. Is his comment reasonable?

- **A. Yes, it is right — 错误**。估值模型输入和假设不同，不能保证结论完全相同；题干关于二者理论依据的表述也不够准确。
- **B. No, it is wrong — 正确**。两个方法可以产生不同的估值结论。
- **C. There is no answer — 错误**。可以明确判断原论断并不合理。

**考试速记**：Present Value = Discount Future Cash Flows；Comparables = Law of One Price；Different Inputs / Assumptions → Different Value Estimates；**Same Valuation Purpose ≠ Guaranteed Same Result**。

**官方参考**：
- [CFA Institute — Equity Valuation: Concepts and Basic Tools (2026)](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/equity-valuation-concepts-basic-tools)。
- [CFA Institute — Market-Based Valuation: Price and Enterprise Value Multiples (2026)](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/market-based-valuation-price-enterprise-value-multiples)。

## 4. 本题解析：Least Accurately Describes Asset-Based Valuation

> Which of the following statements least accurately describes the asset-based valuation?
>
> A. Asset-based model assumes that equity value can be estimated by the difference between the fair value of asset and the fair value of liability.
>
> B. Asset-based model is inappropriate for companies holding lots of intangible assets or financial companies.
>
> C. Asset-based model is appropriate for valuing firms approaching liquidation.

**正确答案：B（最不准确）。**

- **A 正确描述（不选）**：Equity Value = Fair Value of Assets − Fair Value of Liabilities；是该模型的基本原理。
- **B 最不准确（应选）**：无形资产价值大量无法准确估计的企业往往不适合仅依赖资产基础法，但部分金融公司恰好可能适用，例如金融资产可以估值的银行、投资基金等。因此 “or financial companies” 的笼统排除不成立。
- **C 正确描述（不选）**：企业接近 Liquidation（清算），净资产变现价值成为重要估值依据，此法通常适用。

**做题关键词**：Fair Value of Assets Minus Liabilities → Asset-Based；Lots of Intangibles → Caution；Financial Companies → Not Automatically Inappropriate；Liquidation → Often Appropriate。

## 5. 复习清单

- [ ] 记住 \(V_E=FV_A-FV_L\)，能写出每个符号的英文全称和中文释义
- [ ] 区分 Fair Value 与 Book Value
- [ ] 能解释为什么无形资产多的公司估值困难
- [ ] 能解释为什么部分金融公司可能适合使用资产基础法
- [ ] 区分清算价值与持续经营价值、折现现金流价值
- [ ] 能在 “least accurately” 题目中识别 B 的错误

## 6. 参考资料

- [CFA Institute — Equity Valuation: Concepts and Basic Tools (2026)](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/equity-valuation-concepts-basic-tools)
- [CFA Institute — Analysis of Financial Institutions (2026)](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/analysis-of-financial-institutions)
- [CFA Institute — Analysis of Long-Term Assets (2026)](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/analysis-of-long-term-assets)
