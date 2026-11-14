---
subject: Derivatives
topic: Forward vs. Futures Contracts
status: "待复习"
created: 2026-11-14
last-reviewed:
tags: [CFA-L1, Derivatives, Forwards, Futures, Hedging]
---

# 远期与期货合约（Forward vs. Futures Contracts）

## 一句话理解

远期（Forward）和期货（Futures）都属于远期承诺（Forward Commitments），但远期通常是 OTC 定制合约，通常到期结算；期货是在交易所交易的标准化合约，通常通过保证金账户每日盯市结算（Daily Mark-to-Market）。

## 核心概念 / 定义

### 1. 远期合约（Forward Contract）

- 交易双方约定在未来某一日期，以预先确定的价格买卖一定数量的标的资产。
- 通常在场外市场（OTC）交易，条款可根据双方风险敞口定制。
- 典型情况下，盈亏在到期时结算；不采用期货式的每日变动保证金结算。
- 定制化使远期有机会更精确地匹配企业的实际风险敞口。

### 2. 期货合约（Futures Contract）

- 在交易所交易的标准化合约。
- 通常要求交易者缴纳初始保证金（Initial Margin）。
- 每个交易日结束时，交易所根据结算价格（Settlement Price）进行逐日盯市（Mark-to-Market）。
- 当日盈亏通过变动保证金（Variation Margin）反映在保证金账户中。

### 3. 两者共同点：远期承诺（Forward Commitments）

Forward 和 Futures 都约定未来交易，双方原则上都承担合同履约义务，因此都属于 Forward Commitments，而不是 Contingent Claims。

### 4. 远期与期货对比

| 比较维度 | Forward 远期 | Futures 期货 |
|---|---|---|
| 交易市场 | 通常 OTC | 交易所 Exchange |
| 合约条款 | 通常定制 Customized | 标准化 Standardized |
| 结算机制 | 通常到期结算 | 每日盯市 Daily Settlement |
| 保证金 | 视双边合同及抵押安排而定 | 通常有初始保证金和变动保证金制度 |
| 流动性 | 通常较低 | 通常较高 |
| 交易对手风险 | 通常较高，依赖双边信用与抵押安排 | 清算机制通常降低交易对手风险 |
| 主要优势 | 可匹配特定风险敞口 | 标准化、透明、流动性通常较高 |

## 公式与变量

期货每日盯市的简化盈亏：

\[
\text{Daily Gain/Loss}= (F_t-F_{t-1})\times Q
\]

其中：
- \(F_t\)：当日结算价格（Settlement Price）
- \(F_{t-1}\)：前一交易日结算价格；首日可用建仓价格
- \(Q\)：合约数量乘数后的合约规模（按合约报价单位换算）

多头（Long Futures）价格上涨时通常获利，价格下跌时通常亏损；空头（Short Futures）方向相反。

## 完美套期保值（Perfect Hedge）

远期合约可用于建立完美套期保值，因为其标的、金额、期限和交割安排可以定制，以匹配企业已有的风险敞口。

但“完美”通常建立在关键条件能够匹配的假设下，例如：
- 对冲工具与风险敞口的标的完全一致；
- 数量和期限匹配；
- 不存在显著基差风险、交易成本或对手方违约等干扰。

实际对冲未必能做到完全消除所有风险。

## 常见考试陷阱

1. **Forward 和 Futures 都属于 Forward Commitments**，不是只有 Forward 才属于远期承诺。
2. **Daily Settlement 是 Futures 的典型特征**，不是传统远期合约的典型结算机制。
3. 期货每日盯市依据交易所公布的结算价格（Settlement Price），盈亏通过保证金账户反映。
4. 远期合约通常在到期时结算；但 OTC 合同也可能通过抵押品协议定期交换担保品，不能将其与期货每日变动保证金机制简单等同。
5. Forward 的定制化有利于匹配风险敞口，因此可用于建立完美套期保值（Perfect Hedge）；但要实现完美对冲，标的、数量和期限等必须匹配。
6. 两者初始时都约定合约价格，但期货头寸会每日盯市，不能把“约定价格”误解为期货合约每天都不发生现金流结算。

## 典型题型 / 判断路径

题目：Which statement about forward and futures contracts is incorrect?

- Forward contracts can be used to create a perfect hedge. → 正确（在风险敞口与合约条款充分匹配的条件下）。
- Both forward and futures contracts are forward commitments. → 正确。
- Both forward price and futures price are subject to daily settlement. → 错误。每日结算是期货的典型机制，不是远期的典型机制。

**正确答案：C。**

## 易混知识点 / Obsidian 链接

- [[Exchange-Traded-and-OTC-Derivatives]]
- [[Contingent-Claims-and-Forward-Commitments]]

## 我的错因 / 验证记录

- [ ] 能区分远期到期结算与期货每日盯市
- [ ] 能解释 Settlement Price 与 Variation Margin 的作用
- [ ] 能说明远期为什么更容易匹配特定套保需求
- [ ] 能区分 Forward Commitment 与 Contingent Claim


## 远期合约的无套利价格（No-Arbitrage Forward Price）

对于不产生收入、也没有持有成本的简单投资资产，若按年复利：

\[
F_0(T)=S_0(1+r)^T
\]

其中：
- \(F_0(T)\)：今天确定、在 T 时点交割的远期价格（Forward Price）。
- \(S_0\)：标的资产当前现货价格（Spot Price）。
- \(r\)：期限匹配的无风险利率（Risk-free Rate）。
- \(T\)：以年表示的期限（Time to Maturity）。

若采用连续复利，则：

\[
F_0(T)=S_0e^{rT}
\]

### 本题计算

- 现货价格 \(S_0=\$1,000\)
- 无风险利率 \(r=3\%\)
- 期限 \(T=1\) 年

\[
F_0(1)=1000(1+0.03)^1=\boxed{\$1,030}
\]

**正确答案：B. $1,030。**

### 为什么要加上无风险利率？

若投资者今天买入资产，需要投入 \(S_0\)；若改为一年后通过远期买入，则今天可以保留资金并按无风险利率投资。无套利时，两种策略的到期成本应一致，因此远期交割价格等于现货价格的融资成本调整值。

### 空头远期（Short Forward）与套期保值

- 持有标的资产、担心未来价格下跌的投资者，可以卖出远期合约（Short Forward）锁定未来出售价格。
- 到期时空头远期的收益（不含初始价值，且按每单位标的计算）为 \(F_0(T)-S_T\)。
- 远期价格的计算不因投资者选择多头还是空头而改变；多空方向只改变到期收益的正负方向。

### 重要假设与易错点

1. 本题使用简单无收入、无持有成本资产的公式；若资产产生已知收入，远期价格需扣除收入的现值影响。
2. 若存在存储成本、保险费或便利收益（Convenience Yield），需相应调整持有成本模型。
3. **Forward Price ≠ Forward Contract Value**：远期价格是合约约定的交割价格；新签订的公平远期合约初始价值通常为零。
4. Short Forward 不是“今天卖出资产”，而是约定未来按交割价格卖出标的。


## 远期价格与远期合约价值的区别（Forward Price vs. Forward Contract Value）

### 1. 合约成立时（At Initiation）

- 双方约定交割价格 \(K\)，也就是该份现有合约的固定 Forward Price。
- 在公平定价、无初始支付的情况下，新签订远期合约的初始价值通常为零：\(V_0=0\)。

### 2. 合约成立后（After Initiation）

- 原合约约定的交割价格 \(K\) 固定，不会因现货价格变化而自动重设。
- 标的现货价格（Spot Price）变化，会改变这份既有远期合约对持有人的当前价值（Forward Contract Value）。
- 市场上若此时重新签订一份新远期合约，其当前市场远期价格（Current Market Forward Price）会随现货价格及剩余期限、利率和持有成本等因素变化；但这不是原合约已经约定的交割价格。

### 3. 简化估值公式

对于无收入、无持有成本的资产，离到期还有 \(T-t\) 年，按年复利计算：

多头远期（Long Forward）的当前价值：

\[
V_t=S_t-\frac{K}{(1+r)^{T-t}}
\]

其中：
- \(S_t\)：当前现货价格。
- \(K\)：原合约固定的交割价格。
- \(r\)：期限匹配的无风险利率。
- \(T-t\)：剩余期限。

空头远期（Short Forward）的价值为：

\[
V_t^{\text{short}}=-V_t^{\text{long}}
\]

因此，现货价格变化会影响 Forward Value，而原合约的固定交割价格不变。

### 本题判断

Once the forward contract initiates, changes in the underlying spot price lead to:

- Only the forward price fluctuates → 错误；原合约的约定交割价格固定。
- Only the forward value fluctuates → 正确。
- Both fluctuate → 错误；混淆了既有合约的固定交割价格与当前市场新合约价格。

**正确答案：B. The fluctuation of only the forward value.**

记忆：
- Forward Price (contract delivery price K) → fixed after initiation.
- Forward Contract Value → changes as market conditions change.
- Current Market Forward Price → price of a newly initiated forward contract; may change over time.


## 持有成本与持有收益对远期价格的影响（Cost of Carry）

远期价格不仅受现货价格和无风险利率影响，也会受持有标的资产期间产生的成本和收益影响。

### 1. 基本关系

按年复利、成本与收益以估值日现值表示的简化公式：

\[
F_0(T)=\big[S_0+PV(\text{Costs})-PV(\text{Benefits})\big](1+r)^T
\]

其中：
- \(S_0\)：当前现货价格（Spot Price）。
- \(PV(\text{Costs})\)：持有资产期间成本的现值，例如仓储费（Storage Costs）和保险费。
- \(PV(\text{Benefits})\)：持有资产期间收益的现值，例如股息（Dividends）、利息收入或便利收益（Convenience Yield）的相应价值。
- \(r\)：无风险利率（Risk-free Rate）。
- \(T\)：到期期限（Time to Maturity）。

### 2. 方向判断

| 因素 | 对远期价格的影响 | 直觉 |
|---|---|---|
| 现货价格上升 | 上升 | 当前买入资产的成本更高 |
| 无风险利率上升 | 通常上升 | 融资或机会成本提高 |
| 持有成本上升 | 上升 | 持有现货更贵 |
| 持有收益上升 | 下降 | 持有现货更有价值，远期买方无需提前持有即可避免放弃收益 |

记忆：
- **Costs ↑ → Forward Price ↑**
- **Benefits ↑ → Forward Price ↓**

### 3. 例子

假设某资产当前现货价格为 $100，一年期无风险利率为 5%，一年内会支付现值为 $3 的现金收益，且没有其他持有成本：

\[
F_0=(100-3)(1.05)=\$101.85
\]

如果忽略这 $3 的持有收益，远期价格会被高估为 $105。

### 4. 持有收益的例子

- **股息（Dividends）**：股票持有人在持有期间可获得股息，通常会降低股票远期价格。
- **利息收入（Interest Income）**：生息资产的持有人可能获得利息收入，通常会降低远期价格。
- **便利收益（Convenience Yield）**：实物商品持有人因能够立即使用或保障生产供应而获得的非现金收益；便利收益越高，商品远期价格通常越低。

持有成本的例子：
- **仓储成本（Storage Costs）**：持有商品产生的仓储费用，通常会提高远期价格。
- **保险费用（Insurance Costs）**：持有实物资产期间支付的保险费用，通常会提高远期价格。

### 本题判断

Which statement about pricing and valuation of forward contracts is most accurate?

- Benefits of holding an asset increase forward price → 错误，持有收益会降低远期价格。
- Costs of holding an asset decrease forward price → 错误，持有成本会提高远期价格。
- Benefits of holding an asset decrease forward price → 正确。

**正确答案：C。**

注意：不同资产的具体公式还需考虑收益支付时间、成本支付时间、连续复利约定，以及便利收益等因素；本节公式用于掌握方向和基础定价逻辑。


## 远期价格的影响因素：股息、便利收益与违约风险溢价

本题问：Which factor is least likely to influence the price of a forward contract?

- **股息（Dividends）**：会影响股票远期价格。预计股息是持有股票可获得的收益，通常降低远期价格。
- **便利收益（Convenience Yield）**：会影响商品远期价格。持有实物商品带来的即时使用或供应保障价值属于持有收益，便利收益越高，远期价格通常越低。
- **违约风险溢价（Default Risk Premium）**：不是基础无套利远期定价公式中的标准变量。基础模型主要考虑现货价格、无风险利率、持有成本和持有收益。

**正确答案：C. The default risk premium.**

### 现实市场的补充区别

基础无套利远期价格（Theoretical No-Arbitrage Forward Price）与考虑交易对手信用风险后的实际衍生品估值并非完全相同。若交易对手存在违约风险，实际估值可能通过信用估值调整（Credit Valuation Adjustment, CVA）等方式反映信用风险；但这不意味着 Default Risk Premium 是基础远期价格公式中的一般决定因素。

快速记忆：
- Dividends / Convenience Yield → Benefits of Holding → Forward Price ↓
- Storage Costs / Other Carrying Costs → Forward Price ↑
- Default Risk Premium → Not a standard input in the basic no-arbitrage forward pricing formula.


## 利率期货与借款人、贷款人的套期保值（Interest Rate Futures Hedging）

### 1. 利率与期货报价的反向关系

对于以短期利率为基础、采用指数报价的标准利率期货，常见报价方式为：

\[
\text{Futures Price}=100-\text{MRR}
\]

其中 MRR 是市场参考利率（Market Reference Rate）。

因此：
- MRR 上升 → 利率期货价格下降。
- MRR 下降 → 利率期货价格上升。
- 期货多头（Long Futures）在期货价格上涨时获利，在价格下跌时亏损。
- 期货空头（Short Futures）的盈亏方向相反。

示例：
- MRR 从 3% 上升至 4%。
- 期货报价从 97 降至 96。
- 多头期货价格下跌而亏损；空头期货获利。

### 2. 借款人与贷款人的风险及对冲方向

| 参与者 | 主要风险 | 希望对冲的情形 | 常见利率期货头寸 |
|---|---|---|---|
| 借款人（Borrower） | 利率上升，未来利息支出增加 | MRR 上升 | 做空 Short Futures |
| 贷款人（Lender） | 利率下降，未来利息收入减少 | MRR 下降 | 做多 Long Futures |

逻辑：
- **借款人**担心利率上涨。利率上涨时，期货价格下降，空头期货获利，可抵消融资成本上升。
- **贷款人**担心利率下降。利率下降时，期货价格上涨，多头期货获利，可抵消利息收入下降。

### 本题判断

When MRR increases:
- Long interest rate futures position → 期货报价下降，多头亏损。
- Borrowers should generally short interest rate futures to hedge rising-rate risk.
- Lenders should generally long interest rate futures to hedge falling-rate risk.

**正确答案：A. When MRR increases, investors who are long interest rate futures will lose.**

注意：100 − MRR 是短期利率期货常见的指数报价惯例。题目若使用债券期货或其他利率期货合约，应结合其具体报价规则和标的判断；本题按 MRR 指数报价的利率期货框架理解。
