---
subject: Portfolio Management
topic: Pooled Investment Vehicles and Liquidity Management
status: "🟡 解析能懂，待独立验证"
created: 2026-11-11
last-reviewed: 2026-11-11
tags: [CFA-L1, Portfolio-Management, Pooled-Investments, Open-End-Funds, Closed-End-Funds, Private-Equity, Liquidity]
---

# 集合投资工具及流动性管理（Pooled Investment Vehicles & Liquidity）

[[10-Portfolio-Management/INDEX|← 返回投资组合管理目录]]

## 一句话理解

**集合投资工具（Pooled Investment Vehicles）**汇集多个投资者的资金，由专业管理人集中投资。

**核心区分：基金持有人能否向基金本身频繁赎回，以及基金是否必须为赎回准备流动资金。**

- **开放式基金（Open-end Funds）**：典型的每日开放申赎共同基金持续面对投资者赎回，须管理较高的日常流动性需求。
- **封闭式基金（Closed-end Funds）**：份额通常相对固定，投资者主要通过二级市场转让份额，而不是要求基金每天赎回。
- **私募股权基金（Private Equity Funds）**：一般具有较长投资期限及资金锁定安排，投资者通常不能每日赎回。

## 一、基本概念与术语

| 中文 | English | 要点 |
|---|---|---|
| 集合投资工具 | Pooled Investment Vehicles | 汇集投资者资金、统一投资 |
| 流动性 | Liquidity | 资产能否较快、以较低交易成本变现 |
| 流动性需求 | Liquidity Requirements / Needs | 基金履行赎回与其他现金支付义务所需的流动资金 |
| 申购 | Subscription | 投资者向基金投入资金以获得份额 |
| 赎回 | Redemption | 投资者按基金规则向基金交回份额并取得款项 |
| 资产净值 | Net Asset Value (NAV) | 基金资产减负债后的价值；每份 NAV 为净资产除以相应基金份额 |
| 赎回压力 | Redemption Pressure | 投资者集中申请赎回带来的现金支付压力 |
| 流动性错配 | Liquidity Mismatch | 允许较快赎回，但持有的底层资产不易快速出售 |

## 二、三类基金的主要区别

| 维度 | Open-end Fund（开放式基金） | Closed-end Fund（封闭式基金） | Private Equity Fund（私募股权基金） |
|---|---|---|---|
| 份额机制 | 随申购赎回通常可变动 | 存续期内通常相对固定 | 根据基金协议、承诺出资和分配安排运作 |
| 常见投资者退出方式 | 按规则向基金赎回 | 在二级市场将份额转让给其他投资者 | 通过基金持有资产退出和后续分配，或受限的份额转让 |
| 典型每日赎回需求 | **较高**（每日开放申赎的情形） | 通常没有基金直接每日赎回义务 | 通常没有每日赎回义务 |
| 基金资产持有期限 | 需要兼顾赎回流动性 | 相对更能实施长期策略 | 通常用于较长期、非流动性投资 |
| 重要约束 | 赎回管理、现金与高流动性资产 | 二级市场价格可能偏离 NAV | 长期锁定、资本调用（Capital Calls）、分配与退出 |

**比较口径：**这里讨论的是**基金自身需要为持有人每日赎回准备的流动性**，而不是投资者能否随时在交易所卖出份额。

## 三、为什么开放式基金的流动性要求较高？

典型开放式共同基金（Open-end Mutual Fund）的投资者可以在规定的开放日申请赎回。

假设某基金：
- 管理规模（Assets under Management, AUM）：10 亿元；
- 某日赎回申请：5,000 万元。

基金需要按照适用规则支付赎回款。如果可用现金不够，可能需要卖出证券，或采用基金合同和监管允许的流动性管理措施。

基金因此要管理：
1. **Cash and Cash Equivalents（现金及现金等价物）**；
2. **Highly Liquid Assets（高流动性资产）**；
3. **Redemption Pressure（赎回压力）**；
4. **Liquidity Mismatch（流动性错配）**；
5. **Transaction Costs（交易成本）**及在市场承压时卖出资产的潜在折价。

**关键逻辑：开放申赎 → 可能发生频繁现金流出 → 基金需备有充足流动性。**

但不要将“开放式”与“所有开放式基金均可每日赎回”完全画等号；申赎频率以基金合同和适用规则为准。

## 四、封闭式基金为什么日常赎回需求较低？

传统封闭式基金通常发行相对固定的份额。投资者若希望提前退出，往往通过二级市场（Secondary Market）出售给其他投资者。

交易发生在投资者之间，**基金通常不必因份额转手而将底层证券变现、支付每日赎回款**。

注意区分：
- **Investor Liquidity（投资者层面的流动性）**：份额是否容易找到买家、以什么价格卖出；
- **Fund Redemption Liquidity（基金层面的赎回流动性）**：基金是否必须向申请赎回者支付现金。

封闭式基金份额可能在交易所交易，但流动性不一定高；成交价也可能相对于 NAV 出现溢价（Premium）或折价（Discount）。

## 五、私募股权基金的流动性特点

私募股权基金（Private Equity Funds）通常是较长期、投资于非上市企业等流动性较低资产的投资工具。

常见安排：
- 较长锁定期（Lock-up Period）；
- 承诺出资（Capital Commitment）和按项目调用资金（Capital Call）；
- 基金通过资产出售、上市、并购等事件退出，再向出资人分配（Distributions）；
- 一般不允许投资者每天按 NAV 直接赎回。

**边界提醒：**没有每日赎回义务 ≠ 没有流动性风险。私募股权基金仍要管理资本调用、投资支出和退出时间的不确定性；基金份额转让也常受限制。

## 六、常见易错点

1. **最高日常赎回流动性需求**：在题目所比较的典型开放式基金、传统封闭式基金和私募股权基金中，通常是 **Open-end Funds**。
2. **Closed-end Fund** 可以在二级市场交易，不代表基金自身必须每日赎回。
3. 私募股权基金的底层资产流动性往往低，但其**投资者每日赎回义务通常也低**；不要把“底层资产不易卖”误判成“需要最大每日赎回现金”。
4. 开放式基金的申赎安排可能受到频率、期限、暂停赎回或流动性管理规则约束，不应绝对化。
5. **ETF（Exchange-Traded Fund，交易所交易基金）**可能采用开放式基金法律结构，但普通投资者主要在二级市场交易，一级市场申购赎回通常通过授权参与者（Authorized Participants, APs）完成；不可将所有 ETF 简单等同于传统每日现金申赎的共同基金。

## 七、考试速记

- **Open-end = Fund-level Redemption = Higher Liquidity Need（典型每日开放申赎情境）**
- **Closed-end = Secondary-market Trading ≠ Daily Fund Redemption**
- **Private Equity = Long Holding Period / Lock-up, No Routine Daily Redemption**
- **Liquidity of Fund Shares（份额交易流动性）与 Liquidity Needed by Fund（基金支付赎回所需流动性）不是一回事。**

## 八、关联知识与自测清单

- [[Portfolio-Management-Process|投资组合管理流程]]：流动性需求（Liquidity Needs）属于投资约束的重要内容，与 Planning 阶段的 IPS 制定和后续监控有关。
- [[Time-Weighted-Return|时间加权收益率（TWR）]]：基金申购赎回也是分析投资绩效时需要正确处理的外部现金流。

- [ ] 能区分 Open-end Fund、Closed-end Fund 和 Private Equity Fund 的典型退出机制
- [ ] 能解释开放式基金为何需要管理日常赎回现金流
- [ ] 能区分投资者在二级市场卖出份额与向基金直接赎回
- [ ] 能解释底层资产流动性差不等于基金每日赎回需求大
- [ ] 能说明开放式基金和 ETF 的规则差异及例外
