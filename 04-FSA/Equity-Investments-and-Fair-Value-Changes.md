---
subject: Financial Statement Analysis
topic: Financial Asset Classification and Reporting
status: "🟡 解析能懂，待独立验证"
created: 2026-11-03
last-reviewed:
tags: [CFA-L1, FSA, Financial-Assets, Trading, AFS, FVOCI, FVTPL]
---

# 金融资产分类与报表处理区别（Financial Asset Classification & Reporting）

## 学习目标

本笔记只聚焦 CFA 题目中容易混淆的金融资产分类及其报表处理：
1. 传统分类：Trading、Available-for-Sale（AFS）、Held-to-Maturity（HTM）。
2. 现行 IFRS 9 分类：FVTPL、FVOCI、Amortized Cost。
3. 股利、利息、公允价值变动分别进入哪里。
4. 出售时累计 OCI 如何处理。

> **先看题目使用哪套准则 / 分类术语。** Trading、AFS、HTM 是传统分类术语；FVTPL、FVOCI、Amortized Cost 是 IFRS 9 的现行分类。两套术语不能机械地一一对应。

## 一、先区分两类金融工具

| 项目 | Equity Securities（权益证券） | Debt Securities（债务证券） |
|---|---|---|
| 代表什么 | 对企业的所有权 | 对发行人的债权 |
| 典型例子 | 普通股（Common Shares） | 公司债、国债（Bonds） |
| 投资回报 | 股利（Dividends）、价格变动 | 利息（Interest）、价格变动 |
| 到期日 | 普通股通常没有固定到期日 | 通常有合同到期日（Maturity Date） |

这一区分很重要：传统 HTM 只适用于符合条件的债务证券，不适用于普通股。

## 二、传统分类框架（Traditional Classification）

这套分类常见于旧版教材 / 题库。考试遇到 Trading、AFS、HTM 时，先按题目采用的传统框架理解。

### 1. Trading Securities（交易性证券）

- **适用对象**：传统框架下可包括权益证券和债务证券。
- **持有目的**：主要为近期出售、赚取短期价格波动收益。
- **资产负债表（Balance Sheet）**：按公允价值（Fair Value）列示。
- **未实现公允价值收益 / 损失（Unrealized Fair Value Gain / Loss）**：计入当期损益（Income Statement / Profit or Loss）。
- **股利 / 利息收入**：符合确认条件时计入当期损益。

记忆：Trading → Fair Value → 未实现变动进 Income Statement。

### 2. Available-for-Sale Securities（可供出售证券，传统 AFS）

- **适用对象**：传统分类框架下可涉及债务证券；部分旧教材 / 旧准则题目也将权益证券列入 AFS。具体要看题目所依据的旧准则体系。
- **持有目的**：不属于 Trading，也不符合 / 不指定为 HTM 的可供出售投资。
- **资产负债表**：按公允价值列示。
- **未实现公允价值收益 / 损失**：通常计入其他综合收益（OCI），而不是当期净利润。
- **股利 / 利息收入**：符合确认条件时通常计入当期损益。

记忆：传统 AFS → Fair Value → 未实现变动进 OCI。

### 3. Held-to-Maturity Securities（持有至到期证券，HTM）

- **适用对象**：仅适用于符合条件的债务证券（Debt Securities），不适用于普通股。
- **条件**：具有固定或可确定的付款及固定到期日，企业有明确意图和能力持有至到期。
- **资产负债表**：按摊余成本（Amortized Cost）计量。
- **一般市场价格变动**：不因市场报价涨跌而将账面金额调整为公允价值。
- **利息收入**：按适用的实际利率 / 有效利率方法确认利息收入。

记忆：HTM → Debt Only → Amortized Cost。

### 4. 传统分类对照表

| 比较项目 | Trading | Traditional AFS | HTM |
|---|---|---|---|
| 中文 | 交易性证券 | 可供出售证券 | 持有至到期证券 |
| 典型适用对象 | 股票 / 债券 | 依旧准则框架，可能包括股票 / 债券 | 符合条件的债务证券 |
| 资产负债表计量 | Fair Value | Fair Value | Amortized Cost |
| 未实现公允价值变动 | Income Statement | OCI | 通常不确认一般市场价格变动 |
| 股利收入 | Income Statement | Income Statement（若为权益投资） | 不适用普通股股利 |
| 利息收入 | Income Statement | Income Statement（若为债务投资） | Income Statement |

## 三、现行 IFRS 9 分类（Current IFRS 9 Categories）

IFRS 9 不再使用 Trading / AFS / HTM 作为统一分类。分类主要依据：
- **Business Model（业务模式）**：企业如何管理该金融资产以产生现金流。
- **SPPI Test（Solely Payments of Principal and Interest，本金及利息测试）**：合同现金流是否仅为本金及以未偿本金为基础的利息支付。

### 1. Amortized Cost（摊余成本）

通常需要同时满足：
- 业务模式是持有金融资产以收取合同现金流（Hold to Collect）；并且
- 通过 SPPI Test。

处理：
- 资产负债表按摊余成本计量。
- 按实际利率法（Effective Interest Method）确认利息收入。
- 不因一般市场利率或市场报价变化而确认公允价值重估损益。
- 仍需考虑预期信用损失（Expected Credit Loss, ECL）减值要求。

### 2. FVOCI（Fair Value Through Other Comprehensive Income）

**债务工具（Debt Instruments）**通常需要同时满足：
- 业务模式是既收取合同现金流又出售（Hold to Collect and Sell）；并且
- 通过 SPPI Test。

处理：
- 资产负债表按公允价值计量。
- 利息收入、减值损失及适用的汇兑损益按规定进入损益。
- 其他公允价值变动进入 OCI。
- 债务工具终止确认 / 出售时，累计 OCI 通常重分类至损益（Recycling）。

**权益工具（Equity Instruments）**：
- 默认分类为 FVTPL。
- 对非交易性权益投资，可在初始确认时逐项作出不可撤销的 FVOCI 选择。
- 股利通常进入损益（除非明显代表收回部分投资成本）。
- 公允价值变动进入 OCI；处置时累计 OCI 不重分类至损益（No Recycling），可在权益内部转入留存收益。

### 3. FVTPL（Fair Value Through Profit or Loss）

- 是 IFRS 9 下的默认类别，除非满足并采用其他分类条件 / 选择。
- 交易性金融资产通常归入 FVTPL。
- 不符合 Amortized Cost 或 FVOCI 条件的金融资产通常归入 FVTPL。
- 资产负债表按公允价值计量。
- 公允价值变动计入损益。

### 4. IFRS 9 分类对照表

| 分类 | 适用对象 / 条件 | 资产负债表 | 公允价值变动 | 收益确认 |
|---|---|---|---|---|
| Amortized Cost | 债务工具；Hold to Collect + SPPI | 摊余成本 | 不确认一般市场报价变动 | 实际利率法利息进损益 |
| FVOCI – Debt | 债务工具；Hold to Collect and Sell + SPPI | Fair Value | OCI；出售时通常 Recycling | 利息、减值等按规定进损益 |
| FVOCI – Equity Election | 符合条件的非交易性权益工具，初始确认时不可撤销选择 | Fair Value | OCI；出售时不 Recycling | 股利通常进损益 |
| FVTPL | 交易性，或不满足其他分类条件 / 未作 FVOCI 选择 | Fair Value | Income Statement | 公允价值变动进损益 |

## 四、股利、利息与公允价值变动：分别如何处理？

先把三种收益拆开：

### 1. Dividend Income（股利收入）
- 来自权益投资（股票）。
- 通常在投资方取得收取股利的权利时确认。
- 在传统 Trading / AFS 权益投资题目中，股利通常进入 Income Statement。
- IFRS 9 的 FVOCI 权益工具选择下，股利通常也进入损益；若股利明显代表收回部分投资成本，则另行判断。

### 2. Interest Income（利息收入）
- 来自债务投资（债券）。
- 传统分类框架下，Trading、AFS、HTM 债务证券的利息收入通常进入 Income Statement。
- IFRS 9 下，Amortized Cost 与 FVOCI 债务工具按实际利率法确认利息收入；FVTPL 债务工具的计量变动进入损益，具体列报按准则处理。

### 3. Unrealized Fair Value Gain / Loss（未实现公允价值收益 / 损失）
- 资产仍持有，尚未出售，但公允价值发生变化。
- 进入 Income Statement 还是 OCI，取决于分类。

| 情况 | Trading（传统） | AFS（传统） | IFRS 9 FVTPL | IFRS 9 FVOCI Debt | IFRS 9 FVOCI Equity |
|---|---|---|---|---|---|
| 未实现公允价值变动 | Income Statement | OCI | Income Statement | OCI | OCI |
| 出售时累计 OCI | 不适用 | 传统 AFS 通常重分类至损益（依适用旧准则） | 不适用 | 通常重分类至损益 | 不重分类至损益 |
| 现金股利 | Income Statement | Income Statement | — | — | 通常 Income Statement |
| 债券利息 | Income Statement | Income Statement | 按适用 FVTPL 规则进损益 | Effective Interest Method | — |

## 五、出售金融资产（Disposal）时的处理

### 1. Trading / FVTPL
- 出售时确认处置价款与出售前账面价值之间的差额。
- 由于持有期间公允价值变动已进入损益，出售时不能把同一累计收益重复确认一次。

### 2. 传统 AFS
- 持有期间未实现公允价值变动通常进入 OCI。
- 按传统 AFS 债务工具框架，出售 / 终止确认时累计 OCI 通常重分类至损益（Reclassification Adjustment / Recycling）。
- 若旧准则题目明确涉及 AFS 权益证券，按该题目采用的准则版本处理。

### 3. IFRS 9 FVOCI Debt vs. FVOCI Equity
- FVOCI 债务工具：终止确认时累计 OCI 通常重分类至损益（Recycling）。
- FVOCI 权益工具：处置时累计 OCI 不重分类至损益（No Recycling）；可在权益内部转移，不经过当期损益。

## 六、OCI 与 AOCI 的区别

- **OCI（Other Comprehensive Income，其他综合收益）**：本期发生、按准则计入其他综合收益的项目。
- **AOCI（Accumulated Other Comprehensive Income，累计其他综合收益）**：历期 OCI 累计留在股东权益中的余额。

$$
Total\\ Comprehensive\\ Income=Net\\ Income+OCI
$$

OCI 不等于现金流，也不等于普通的投资收益；它是综合收益列报中的特定组成部分。

## 七、题目案例：股利与未实现收益的区别

Company A：
- 以 $50,000 买入 Company B 股票。
- 年内收到现金股利 $10,000。
- 年末股票公允价值为 $65,000。

未实现收益：

$$
65,000-50,000=\\$15,000
$$

按题目采用的传统分类框架：

| 项目 | Traditional AFS | Trading |
|---|---:|---:|
| Dividend Income | $10,000 → Income Statement | $10,000 → Income Statement |
| Unrealized Gain | $15,000 → OCI | $15,000 → Income Statement |
| Income Statement 合计 | **$10,000** | **$25,000** |

因此题目问两种分类下的利润表影响时，答案为 **$10,000 & $25,000**。

## 八、CFA 常见考试陷阱

1. **Trading 不等于“持有不超过一年”**：不能只根据持有期限分类，重点看分类定义和适用准则。
2. **HTM 只适用于符合条件的债务证券**：普通股没有固定到期日，不能分类为 HTM。
3. **传统 AFS 与 IFRS 9 FVOCI 不完全相同**：特别是权益工具处置时累计 OCI 的处理。
4. **股利与未实现收益分开判断**：股利通常进损益；公允价值变动按分类进入损益或 OCI。
5. **未实现不代表不确认**：Trading / FVTPL 的未实现公允价值变动也进入当期损益。
6. **出售时不要重复确认收益**：持有期间已按公允价值重估并进入损益的金额，出售时只确认相对于最新账面价值的差额。
7. **Amortized Cost 不等于永远不变**：仍会因实际利率法、收款、减值等发生变化，只是不确认一般市场报价波动。

## 九、考题判断顺序

遇到金融资产分类题，按以下顺序判断：

1. 题目使用传统 Trading / AFS / HTM，还是 IFRS 9 的 FVTPL / FVOCI / Amortized Cost？
2. 投资是 Equity Instrument（权益工具）还是 Debt Instrument（债务工具）？
3. 资产负债表按 Fair Value 还是 Amortized Cost 计量？
4. 收益属于 Dividend、Interest，还是 Unrealized Fair Value Change？
5. 未实现变动进入 Income Statement 还是 OCI？
6. 若题目涉及出售，判断累计 OCI 是否 Recycling。

## 十、复习检查

- [ ] 能区分传统 Trading、AFS、HTM 的计量与报表处理
- [ ] 能区分 IFRS 9 下 Amortized Cost、FVOCI、FVTPL
- [ ] 能区分权益工具与债务工具适用的分类
- [ ] 能判断股利收入、利息收入和未实现公允价值变动的列报
- [ ] 能区分 FVOCI Debt 与 FVOCI Equity 的出售处理
- [ ] 能解释 OCI、AOCI 与 Net Income 的关系
