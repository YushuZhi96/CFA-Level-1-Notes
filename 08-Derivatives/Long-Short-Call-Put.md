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
