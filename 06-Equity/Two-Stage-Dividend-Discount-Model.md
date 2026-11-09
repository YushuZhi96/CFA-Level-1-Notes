---
subject: CFA Level I
topic: Equity Valuation — Two-Stage Dividend Discount Model
status: 持续更新
created: 2026-11-09
tags: [CFA-L1, Equity-Investments, DDM, Dividend-Discount-Model, Two-Stage-Growth]
---

# Two-Stage Dividend Discount Model (DDM)｜两阶段股息贴现模型

[[06-Equity/INDEX|返回权益投资目录]] · [[06-Equity/Justified-Price-to-Earnings-Ratio|P/E 与戈登增长模型专题]]

## 1. 核心概念

- **Dividend Discount Model (DDM，股息贴现模型)**：将持有股票未来预计获得的股息按必要收益率折现，以估算股票当前内在价值（Intrinsic Value）。
- **Two-Stage DDM（两阶段股息贴现模型）**：假设股息经历两个增长阶段：第一阶段以较高或特殊增长率变化，之后进入长期稳定增长阶段。
- **Gordon Growth Model（戈登增长模型）**：长期稳定增长阶段的终值（Terminal Value）计算公式，需满足长期增长率小于股权必要收益率（\(r>g_L\)）。
- **本题特殊设定**：只有**未来第一年**以5%增长；**第二年开始**以2%长期稳定增长。题目要求 **Current Dividend per Share \(D_0\)**，而不是 \(D_1\)。

## 2. 数学公式和变量完整中英文释义

**一般两阶段模型**（第一阶段持续 \(N\) 年）：

\[
\boxed{P_0=\sum_{t=1}^{N}\frac{D_t}{(1+r)^t}+\frac{P_N}{(1+r)^N}}
\]

\[
\boxed{P_N=\frac{D_{N+1}}{r-g_L}}
\]

| 符号 | 英文全称 | 中文含义 |
|---|---|---|
| \(P_0\) | **Current Intrinsic Value / Stock Price at Time 0** | 当前（时间0）的股票内在价值 |
| \(P_N\) | **Terminal Value at the End of Year N** | 第N年末终值，代表此后稳定股息的现值（以第N年为估值时点） |
| \(D_0\) | **Current Dividend per Share** | 当前每股股息，通常指最新已支付或当前基期每股股息 |
| \(D_t\) | **Expected Dividend per Share in Year t** | 第t年预期每股股息 |
| \(D_1\) | **Dividend per Share in Year 1** | 下一年末预计每股股息 |
| \(D_2\) | **Dividend per Share in Year 2** | 第二年末预计每股股息 |
| \(D_{N+1}\) | **Dividend in the First Stable-Growth Year** | 进入稳定增长期后的第一笔股息 |
| \(r\) | **Required Rate of Return on Equity** | 股权必要收益率／贴现率 |
| \(g_H\) | **First-Stage / High Dividend Growth Rate** | 第一阶段／较高阶段股息增长率 |
| \(g_L\) | **Long-Run / Stable Dividend Growth Rate** | 长期稳定股息增长率 |
| \(N\) | **Length of the First Stage (Years)** | 第一阶段持续年数 |
| \(t\) | **Year / Time Index** | 年份／时间下标 |

**变量时间顺序是高频考试陷阱**：

\[
\boxed{D_1=D_0(1+g_H)}
\]

\[
\boxed{D_2=D_1(1+g_L)}
\]

只针对本题 \(N=1\) 的情形：

\[
\boxed{P_1=\frac{D_2}{r-g_L}}
\]

\[
\boxed{P_0=\frac{D_1+P_1}{1+r}}
\]

**为什么** \(P_1\) **要用** \(D_2\)**？** 因为 \(P_1\) 是第一年末（除息后的）价值，代表从第二年末开始的所有后续股息。

### 2.1 笔记本必背公式卡｜通用公式、单年特例、快捷反推

**① 必背：一般两阶段 DDM（第一阶段共 \(N\) 年）**

\[
\boxed{P_0=\sum_{t=1}^{N}\frac{D_t}{(1+r)^t}+\frac{P_N}{(1+r)^N}}
\]

\[
\boxed{P_N=\frac{D_{N+1}}{r-g_L}}
\]

**理解**：前 \(N\) 年每期股息的现值之和，再加第 \(N\) 年末终值的现值。长期稳定增长阶段必须满足 \(r>g_L\)。

**② 理解：第一阶段恰好1年的特例**

\[
\boxed{P_0=\frac{D_1+P_1}{1+r}}
\]

\[
\boxed{P_1=\frac{D_2}{r-g_L}}
\]

**理解**：第一年末可获得 \(D_1\) 股息与除息后股票价值 \(P_1\)，两者都属于一年后的价值，因此一起除以 \(1+r\) 折算到今天。此时 \(D_2=D_1(1+g_L)\)。

**③ 考场快捷：从当前股价反推当前股息（仅第一阶段1年）**

由于 \(P_0=D_1/(r-g_L)\)，且 \(D_1=D_0(1+g_H)\)，可推出：

\[
\boxed{D_0=\frac{P_0(r-g_L)}{1+g_H}}
\]

**本题**：

\[
\boxed{D_0=\frac{30(0.07-0.02)}{1+0.05}\approx\$1.43}
\]

**切勿误用**：第三式不是一般 \(N\) 年两阶段 DDM 的通用式，只有第一阶段恰好1年、从第二年起股息按 \(g_L\) 永续增长、折现率在该模型中为 \(r\) 时才可使用；持续多年时回到公式①。

**本卡符号对照**（上面的完整中英文对照表见本章开头）：

| 符号 | 英文全称 | 中文含义 |
|---|---|---|
| \(P_0\) | Current Intrinsic Value | 当前内在股价 |
| \(P_1\) | Terminal Value at Year 1 | 第一年底终值 |
| \(P_N\) | Terminal Value at Year N | 第N年底终值 |
| \(D_0\) | Current Dividend per Share | 当前每股股息 |
| \(D_1,D_2\) | Expected Dividends in Years 1 and 2 | 第一、第二年预期每股股息 |
| \(D_t\) | Dividend at Time t | 第t年的预期股息 |
| \(D_{N+1}\) | First Dividend in Stable Growth Stage | 稳定增长期首年股息 |
| \(r\) | Required Return on Equity | 股权必要收益率 |
| \(g_H\) | First-Stage Dividend Growth Rate | 第一阶段股息增长率 |
| \(g_L\) | Long-Run Stable Growth Rate | 长期稳定股息增长率 |
| \(N\) | Number of Years in First Stage | 第一阶段持续年数 |
| \(t\) | Time Index | 时间下标 |

**记忆顺序**：① 通用公式必须背；② 一年特例要理解“股息＋终值一起折现”；③ 快捷反推只用于一年特例。

## 3. 本题原文与中文翻译

> Sam is an analyst. Recently he uses two-stage DDM model to estimate Company X’s price per share. Calculate closest current dividend per share using the data below:

**中文翻译**：Sam 是一位分析师，使用两阶段 DDM 估算 X 公司每股价值。给定以下数据，计算**当前每股股息**最接近哪一个数值。

| 条件 | 英文 | 数值 |
|---|---|---:|
| 当前内在价值 | Intrinsic Value | $30 |
| 第一年的股息增长率 | Dividend Growth Rate for the Next Year | 5% |
| 此后长期股息增长率 | Dividend Growth Rate Thereafter | 2% |
| 股权必要收益率 | Required Rate of Return | 7% |

**选项**：A. $1.32 / B. $1.36 / **C. $1.43**。

## 4. 从完整两阶段模型一步步反推 D0

已知：

\[
P_0=30,\qquad g_H=5\%,\qquad g_L=2\%,\qquad r=7\%
\]

**第一步：表示未来股息**

\[
D_1=1.05D_0,\qquad D_2=1.02D_1=1.071D_0
\]

**第二步：第一年末终值**

\[
P_1=\frac{D_2}{r-g_L}=\frac{1.071D_0}{0.07-0.02}
=21.42D_0
\]

**第三步：将第一年股息和终值折现回当前**

\[
30=\frac{1.05D_0+21.42D_0}{1.07}
=\frac{22.47D_0}{1.07}
=21D_0
\]

**第四步：反推出当前股息**

\[
\boxed{D_0=\frac{30}{21}\approx\$1.42857\approx\$1.43}
\]

**正确答案：C. $1.43。**

**验证**：\(D_0=1.428571\) 时，\(D_1=1.50\)，\(D_2=1.53\)，\(P_1=1.53/0.05=30.60\)；现值：

\[
P_0=\frac{1.50+30.60}{1.07}=30.00
\]

## 5. 本题更快的考场解法（只适用于第一阶段恰好1年）

由于本题 \(N=1\)，且 \(D_2=D_1(1+g_L)\)，可以代数化简：

\[
P_0=\frac{D_1+D_2/(r-g_L)}{1+r}
\]

\[
=\frac{D_1+D_1(1+g_L)/(r-g_L)}{1+r}
=\frac{D_1}{r-g_L}
\]

故：

\[
\boxed{D_1=P_0(r-g_L)=30(0.07-0.02)=1.50}
\]

再还原当期股息：

\[
\boxed{D_0=\frac{D_1}{1+g_H}=\frac{1.50}{1.05}=\$1.42857\approx\$1.43}
\]

**注意**：这个简化是因为第一阶段只有一年、稳定增长从 \(D_2\) 开始才成立。若第一阶段持续多于一年，必须使用一般两阶段求和与终值折现，不能直接照搬该捷径。

## 6. 易错点与 CFA 考试速记

1. **Current Dividend ≠ Next Year Dividend**：本题所求 \(D_0\)，不是 \(D_1=1.50\)。
2. **P1 用 D2**：第一年末终值反映从第二年开始的稳定现金流，不能用 D1 代替 D2。
3. **Terminal Value 也要折现**：\(P_1\) 是第一年末的价值，不是当前 \(P_0\)。
4. **Long-Run Growth 从第二年开始**：本题第一年增长5%，之后才是2%，不能将两阶段增长率混用。
5. **必要收益率要高于长期增长率**：\(r=7\%>g_L=2\%\)，稳定增长永续公式才有正常有限值。
6. **复杂题先画时间线**：\(D_0\xrightarrow{+5\%}D_1\xrightarrow{+2\%}D_2\)，并标注 \(P_1=D_2/(r-g_L)\)。

**记忆口诀**：先画时间线 → 算每年股息 → 算终值 → 一起折现 → 反推当前股息。

## 7. 自测

**Q1**：这道题若求 Next Year Dividend（下一年股息），应选什么？  
**A1**：$1.50，而不是 $1.43。

**Q2**：为什么不能把 \(P_1\) 与 \(P_0\) 混为一谈？  
**A2**：\(P_1\) 属于一年后，仍需用 \(1+r\) 折现，且第一年的股息也应单独计入。

**Q3**：若第一阶段持续3年，可否直接使用 \(D_1=P_0(r-g_L)\)？  
**A3**：不可以，需要一般两阶段 DDM 的逐年折现与第3年末终值。

## 8. 参考

- CFA Institute, [Discounted Dividend Valuation (2026)](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/discounted-dividend-valuation)。
- 关联：[[06-Equity/Justified-Price-to-Earnings-Ratio|P/E 与 Gordon Growth Model]]。
