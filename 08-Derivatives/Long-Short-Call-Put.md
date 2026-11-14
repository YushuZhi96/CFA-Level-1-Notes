---
subject: Derivatives
topic: Long Short Call Put
status: 待复习
created: 2026-11-01
tags: [CFA-L1, Derivatives, Options]
---
# Long / Short / Call / Put：四种期权头寸

## 区分两个维度
- **Call / Put：合约类型**。Call 赋予买方按约定条件**买入**标的的权利，Put 赋予买方按约定条件**卖出**标的的权利。
- **Long / Short：你持有的是哪一边**。Long Option 是持有期权权利；Short Option 是卖出期权并承担相应履约义务。

| 头寸 | 买方/卖方 | 权利或义务 | 到期 Payoff（不含期权费） |
|---|---|---|---|
| Long Call | 买入 Call | 有权买入 | $\max(S_T-K,0)$ |
| Short Call | 卖出 Call | 有义务按合约卖出 | $-\max(S_T-K,0)$ |
| Long Put | 买入 Put | 有权卖出 | $\max(K-S_T,0)$ |
| Short Put | 卖出 Put | 有义务按合约买入 | $-\max(K-S_T,0)$ |

## 易错点
- **Long Call 的直接期权交易对手是 Short Call**，不是 Short Put；两方交易同一类型的 Call 合约。
- Payoff ≠ Profit：买方利润还要扣初始期权费，卖方利润还要加初始收到的期权费（忽略资金时间价值和手续费）。
- 卖出看涨期权 Short Call 并不表示“有权卖出标的”，而是卖出了一份他人的买入权。


## 欧式与美式期权（European vs. American Options）

- **欧式期权（European Option）**：只能在到期日（Expiration Date）行权。
- **美式期权（American Option）**：通常可以在到期日之前的任何允许交易日行权，也可以在到期日行权。
- European / American 描述的是行权时间限制，不是交易地点，也不代表期权标的或币种。

## 看跌期权买方的权利（Long Put）

买入看跌期权（Long Put）赋予持有人按行权价格（Strike Price, K）卖出标的资产的权利，而不是义务。

到期时：
- 若标的价格 \(S_T < K\)，看跌期权处于实值（In the Money），持有人通常会行权，以 K 卖出价值为 \(S_T\) 的标的。
- 若 \(S_T \ge K\)，期权没有正的行权价值，持有人通常放弃行权。

到期收益（Payoff，不含期权费）：

\[
\text{Long Put Payoff}=\max(K-S_T,0)
\]

若买入时支付期权费（Option Premium）为 \(P\)，忽略资金时间价值和交易成本，到期利润为：

\[
\text{Long Put Profit}=\max(K-S_T,0)-P
\]

## 本题判断

投资者买入一份行权价为 $30 的欧式看跌期权：

- 期权类型 Put → 有权卖出股票。
- 行权价 $30 → 若行权，可按每股 $30 卖出。
- European → 只能在到期日行权。
- 买方持有的是权利，不是必须卖出股票的义务。

**正确答案：B. Has a right to sell the stock at $30.**

易错点：C 的 “has an obligation to sell” 描述的是期权卖方在买方行权时承担的履约义务，不是期权买方的义务。


## 期权实值、平值与虚值（Moneyness）

期权的实值状态由标的资产当前价格（或到期价格）与行权价格的关系决定，**不由期权费决定**。

设：
- \(S\)：标的股票价格
- \(K\)：行权价格（Strike Price）

| 期权类型 | 实值（ITM） | 平值（ATM） | 虚值（OTM） |
|---|---|---|---|
| Call 看涨期权 | \(S>K\) | \(S=K\) | \(S<K\) |
| Put 看跌期权 | \(S<K\) | \(S=K\) | \(S>K\) |

到期内在价值（Intrinsic Value）：
- Call：\(\max(S_T-K,0)\)
- Put：\(\max(K-S_T,0)\)

### 本题判断：卖出看涨期权（Writing a Call）

- 行权价格 \(K=30\) 美元。
- 到期股票价格 \(S_T=29\) 美元。
- 因为 \(S_T<K\)，Call 为虚值（Out of the Money, OTM）。
- 买方没有理由以 $30 买入市价 $29 的股票，因此通常不会行权。
- 卖方（Writer）收到的期权费为 $2；到期时 Call payoff 为 0，因此在忽略交易成本等情况下，卖方保留 $2 期权费，取得 $2 的净利润。

注意：题目说 investor is writing a call，说明投资者是期权卖方；但 ITM / ATM / OTM 是对期权合约本身的分类，不因投资者是买方还是卖方而改变。

## 常见考试陷阱

1. Call：股价高于行权价才是实值；Put：股价低于行权价才是实值。
2. ITM / ATM / OTM 只比较标的价格与行权价格，**不把期权费纳入判断**。
3. 期权费影响净利润（Profit），不改变期权的实值状态（Moneyness）。
4. 买入或卖出（Long / Short）不会改变同一份期权合约的 moneyness。
