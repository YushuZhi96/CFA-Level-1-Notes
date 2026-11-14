---
subject: Derivatives
topic: Exchange-Traded and OTC Derivatives
status: "待复习"
created: 2026-11-14
last-reviewed:
tags: [CFA-L1, Derivatives, Market-Structure]
---

# 场内与场外衍生品（Exchange-Traded vs. OTC Derivatives）

## 一句话理解

场内衍生品（Exchange-Traded Derivatives, ETD）通常采用交易所制定的标准化合约，在集中市场交易，流动性通常较高，并通过清算和保证金制度降低交易对手风险；场外衍生品（Over-the-Counter Derivatives, OTC）由交易双方协商合约条款，定制灵活，但需要更加关注交易对手风险和流动性。

## 核心概念 / 定义

### 1. 场内交易衍生品（ETD）

在交易所挂牌并按照交易所规则交易的衍生品。

典型特征：
- **标准化（Standardized）**：交易所统一规定合约标的、规模、到期日、报价单位、交割方式等。
- **集中交易（Exchange Trading）**：交易在有组织的交易所市场进行，报价和交易规则较透明。
- **流动性通常较高（Generally More Liquid）**：标准化使不同市场参与者更容易交易同一类合约，但具体流动性仍取决于合约和市场活跃度。
- **交易对手风险较低（Lower Counterparty Risk）**：中央对手方清算、保证金和逐日盯市等机制降低风险，但不代表违约风险为零。

常见例子：
- 期货（Futures）
- 部分期权（Options）

### 2. 场外交易衍生品（OTC）

交易双方通常通过经纪商或直接协商，在交易所之外订立的衍生品合约。

典型特征：
- **定制化（Customized）**：可协商名义本金、期限、标的、支付安排和结算方式。
- **交易安排灵活（Flexible Terms）**：可以更贴合企业或投资者特定的风险敞口。
- **流动性通常较低（Generally Less Liquid）**：定制条款降低了合约的可替代性，退出或转让可能更困难。
- **交易对手风险相对较高（Higher Counterparty Risk）**：双方需要评估对手方信用，并可通过抵押品、净额结算等安排管理风险。

常见例子：
- 远期（Forwards）
- 互换（Swaps）
- 部分期权（Options）

## ETD 与 OTC 对比

| 比较维度 | 场内 ETD | 场外 OTC |
|---|---|---|
| 合约条款 | 通常标准化（Standardized） | 通常定制化（Customized） |
| 交易场所 | 交易所（Exchange） | 交易双方协商的场外市场 |
| 流动性 | 通常较高 | 通常较低，取决于合约和市场 |
| 交易对手风险 | 通常较低，清算机制降低风险 | 通常较高，需管理对手方信用风险 |
| 清算方式 | 通常通过中央对手方清算 | 可双边清算，也可能通过 CCP 清算 |
| 灵活性 | 较低，受标准合约约束 | 较高，可按需求设计条款 |

## 为什么 ETD 通常流动性更高？

1. 合约规格统一，市场参与者交易的是相同或高度可替代的合约。
2. 交易集中在交易所，买卖报价更容易汇集。
3. 更容易通过反向交易平仓，而不必重新协商一份定制合同。

注意：**标准化和集中交易有助于提高流动性，但不保证每一种场内合约都活跃或容易成交。**

## 为什么 ETD 的违约风险相对较低？

中央对手方（Central Counterparty, CCP）介入交易双方之间，成为每个卖方的买方、每个买方的卖方。配合以下机制管理风险：

- **初始保证金（Initial Margin）**：覆盖潜在未来风险的担保资金。
- **变动保证金（Variation Margin）**：根据市场价格变化结算已发生的损益。
- **逐日盯市（Mark-to-Market）**：定期按市场价格重估头寸并结算损益。
- **违约管理机制（Default Management）**：在参与者违约时，按照清算规则处置风险敞口。

这些机制降低交易对手风险，但不能将其完全消除。部分 OTC 衍生品也可能通过 CCP 清算，因此不能简单认为“OTC 一定是双边清算”。

## 常见考试陷阱

1. **Customized 是 OTC 的典型特征，不是 ETD。**
2. **Highly liquid 是 ETD 的典型特征**，但题目中的通常（generally）很重要，不应理解为所有场内合约都高度活跃。
3. **ETD 并非没有违约风险（No Default Risk）**。更准确的说法是交易对手风险较低（Lower Counterparty Risk）。
4. **OTC 并不等于一定不清算**。部分 OTC 合约也可以通过中央对手方清算。
5. **Options 不只存在于场内**：期权既可以是交易所交易，也可以是场外定制。
6. 不要把“合约标准化”与“标的资产标准化”混为一谈；ETD 的标准化主要指合约条款和规格。

## 典型题型 / 判断路径

题目问：Which best describes exchange-traded derivatives?

- Customized → 通常指向 OTC。
- Subject to default risk → 不是 ETD 的最佳典型描述；ETD 通常通过 CCP 和保证金机制降低交易对手风险。
- Highly liquid → 通常是 ETD 的典型特征。

**本题答案：C. Highly liquid（流动性高）。**

快速判断：
- Exchange-traded → Standardized → Centralized trading → Generally more liquid.
- OTC → Customized → Flexible terms → Counterparty risk needs greater attention.

## 易混知识点 / Obsidian 链接

- [[Long-Short-Call-Put]]
- 期货（Futures）与远期（Forwards）的具体定价和结算差异，后续单独整理。

## 我的错因 / 验证记录

- [x] 能区分 ETD 与 OTC 的典型特征
- [ ] 不看解析能独立解释 CCP、保证金和逐日盯市如何降低风险
- [ ] 能独立完成一道 ETD 与 OTC 的变式题


## 补充：信息透明度与监管（Transparency and Regulation）

### 信息透明度（Transparency）

- **ETD 通常透明度更高**：交易集中在交易所，市场参与者通常可以观察到公开报价（Public Quotes）、成交价格和成交量。
- **OTC 通常透明度相对较低**：交易双方协商具体条款，报价和交易信息可能是双边或非公开的，不一定向整个市场披露。
- 这并不意味着 OTC 完全没有市场报价或披露要求；具体透明度取决于产品、交易报告制度和监管规则。

### 监管（Regulation）

- ETD 在交易所规则和相关监管框架下交易，合约规格、交易和清算流程较为统一。
- OTC 不通过交易所集中撮合，条款更灵活；但不能据此认为 OTC 完全不受监管。不同司法管辖区可能要求 OTC 衍生品进行报告、保证金管理或中央清算。

### 本题判断

题目：Which of the following best describes the exchange-traded derivatives but not the over-the-counter derivatives?

- Customized → OTC 的典型特点。
- Transparent → ETD 的典型特点，正确答案。
- Less regulation → 更接近 OTC 相对于交易所市场的传统特征，但不是“OTC 不受监管”。

**正确答案：B. Transparent（透明度高）。**

快速记忆：
- ETD → Standardized + Exchange-traded + Generally more liquid + More transparent.
- OTC → Customized + Bilateral negotiation + Generally less transparent + Counterparty risk management is important.


## 补充：场外衍生品的结算方式（Settlement Methods）

OTC 合约的结算安排可以根据双方约定设计，常见方式包括：

- **实物交割（Physical Delivery）**：按合约实际交付标的资产或约定的本金。
- **现金结算（Cash Settlement）**：不交付标的资产，而是按合约约定，以现金支付相关价值差额。

具体采用哪种方式取决于合约条款和产品结构；不能据此认为所有 OTC 合约都采用同一种结算方式。

### 题目判断

关于 OTC derivatives，哪项陈述错误？

- Customized → 正确，OTC 通常允许双方定制条款。
- More liquid and transparent → 错误，OTC 通常不如 ETD 流动性高、透明度高。
- Physical or cash settlement → 可作为 OTC 合约可能采用的结算安排，具体取决于合同。

**正确答案：B. They are more liquid and transparent.**

术语提醒：Physical Delivery 和 Cash Settlement 是结算方式（Settlement Methods）；Exercise（行权）是期权持有人是否使用期权权利的行为。题目将 “exercised by physical or cash delivery” 混用，严格术语上不够准确，应理解为“可采用实物交割或现金结算”。
