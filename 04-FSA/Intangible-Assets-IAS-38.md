---
subject: Financial Statement Analysis
topic: Intangible Assets under IFRS
status: "🟡 解析能懂，待独立验证"
created: 2026-11-03
last-reviewed:
tags: [CFA-L1, FSA, Long-Term-Assets, Intangible-Assets, IAS-38]
---

# 无形资产（Intangible Assets）— IFRS / IAS 38

## 一、核心概念

**Intangible Asset（无形资产）**是可辨认的（Identifiable）、非货币性（Non-monetary）、没有实物形态（Without Physical Substance）的资产。

常见例子：
- Patent（专利权）
- Trademark（商标权）
- Copyright（版权）
- License（许可证）
- Franchise（特许经营权）
- Software（软件）

注意：不是所有没有实物形态的资源都能确认为无形资产。必须满足资产定义及确认条件。

## 二、无形资产的确认条件（Recognition Criteria）

一项资源要确认为无形资产，通常需要满足：

1. **Identifiable（可辨认）**：满足以下至少一项：
   - Separable（可分离）：能够从企业中分离或拆分，并单独或连同相关合同、资产或负债出售、转让、许可、出租或交换；
   - Arises from Contractual or Other Legal Rights（源自合同或其他法定权利）：即使该权利不能转让或不能与企业或其他权利义务分离，也可能满足可辨认性。
2. **Control（控制）**：企业有能力取得该资源带来的未来经济利益，并限制他人取得这些利益。
3. **Future Economic Benefits（未来经济利益）**：例如收入、成本节约或其他利益。
4. **Reliable Measurement of Cost（成本能够可靠计量）**：满足适用确认要求。

## 三、无形资产的初始计量（Initial Measurement）

### 1. 单独购买（Separate Acquisition）
- 初始通常按 Cost（成本）计量。
- 成本通常包括购买价（扣除折扣和返利）、不可退还税费，以及使资产达到预定用途直接相关的支出。
- 一般不包括广告、培训、开办费用和日常管理费用。

### 2. 企业合并中取得（Acquired in a Business Combination）
- 若无形资产可辨认，购买方通常在购买日按 Fair Value（公允价值）单独确认，即使被收购方以前没有在自己的资产负债表中确认该资产。
- 该项无形资产与 Goodwill（商誉）区分；商誉是企业合并中的剩余金额。

### 3. 内部生成（Internally Generated）
内部生成无形资产需要特别谨慎：
- Research Phase（研究阶段）支出：发生时计入费用（Expense），不能资本化为无形资产。
- Development Phase（开发阶段）支出：只有同时满足 IAS 38 规定的开发资本化条件，才可以资本化。
- 若无法区分研究阶段和开发阶段，应将支出视为研究阶段支出，计入费用。

### 4. 开发阶段资本化的六项条件

企业必须能够证明以下全部条件：
1. Technical Feasibility（技术上可行）：完成该无形资产使其能够使用或出售在技术上可行。
2. Intention to Complete（有完成意图）：企业有完成并使用或出售该资产的意图。
3. Ability to Use or Sell（有能力使用或出售）：企业能够使用或出售该资产。
4. Probable Future Economic Benefits（未来经济利益很可能流入）：例如存在市场，或资产对内部使用有用。
5. Adequate Resources（资源充足）：拥有足够的技术、财务和其他资源完成开发并使用或出售。
6. Reliable Measurement（支出能够可靠计量）：开发阶段归属于该无形资产的支出能够可靠计量。

**内部生成品牌（Brands）、报刊名称（Mastheads）、出版名称（Publishing Titles）、客户名单（Customer Lists）和类似项目通常不得确认为无形资产。** 内部生成商誉（Internally Generated Goodwill）也不确认为资产。

## 四、后续计量（Subsequent Measurement）

IAS 38 规定，初始确认后，企业可按会计政策选择以下模型，对某一类无形资产进行后续计量：

### 1. 成本模型（Cost Model）

\[
Carrying\ Amount = Cost - Accumulated\ Amortization - Accumulated\ Impairment
\]

中文理解：

**账面价值 = 成本 − 累计摊销 − 累计减值损失**

- 成本作为计量基础。
- 有限使用寿命资产通常持续摊销。
- 还要扣除累计减值损失。

### 2. 重估模型（Revaluation Model）

重估日按 Fair Value（公允价值）计量，之后再扣除重估日后的累计摊销和累计减值：

\[
Carrying\ Amount = Fair\ Value\ at\ Revaluation\ Date
- Subsequent\ Amortization
- Subsequent\ Impairment
\]

**重要限制：公允价值必须能够参考 Active Market（活跃市场）确定。**

- 无形资产通常具有独特性，活跃市场较少，因此重估模型在实践中不常见。
- 采用重估模型时，通常需要对同一类别（Class）的无形资产采用一致政策；若某项资产不存在活跃市场，通常按成本模型计量。
- 重估应足够频繁，以确保报告日账面价值与公允价值没有重大差异。

### 3. 为什么题目中的 Fair Value Model 不正确？

IAS 38 的后续计量选择是：
- Cost Model（成本模型）
- Revaluation Model（重估模型）

**Fair Value 是重估模型使用的计量基础，不是 IAS 38 单独列出的第三种无形资产后续计量模型。**

因此，题目问哪种模型最不可能用于 IFRS 无形资产时，答案是 **Fair Value Model**。不能把 Fair Value Model 与 Revaluation Model 当成同义词。

## 五、使用寿命（Useful Life）：有限与不确定

### 1. 有限使用寿命（Finite Useful Life）
- 在使用寿命内进行 Amortization（摊销）。
- 当资产达到可供使用状态（Available for Use）时开始摊销。
- 摊销方法应反映经济利益消耗方式；若无法可靠确定，则使用直线法（Straight-line Method）。
- 每年至少复核使用寿命、残值（Residual Value）和摊销方法。
- 还需关注是否存在减值迹象。

### 2. 不确定使用寿命（Indefinite Useful Life）
- 不进行定期摊销（No Amortization）。
- 至少每年进行 Impairment Test（减值测试），并在出现减值迹象时测试。
- 每个报告期复核其使用寿命是否仍为不确定。
- Indefinite 不等于 Infinite（无限 / 永远）；它表示在可预见期间内，没有可预见的经济利益流入期限上限。

## 六、减值（Impairment）

无形资产适用 IAS 36 减值要求：
- 若存在减值迹象，应估计 Recoverable Amount（可收回金额）。
- 不确定使用寿命、尚未可供使用的无形资产，以及企业合并取得的商誉，至少每年进行减值测试。
- 若 Carrying Amount（账面价值）高于 Recoverable Amount（可收回金额），确认 Impairment Loss（减值损失）。

\[
Impairment\ Loss = Carrying\ Amount - Recoverable\ Amount
\]

仅当账面价值高于可收回金额时确认减值。

## 七、重估变动计入哪里？（Revaluation Gain / Loss）

重估模型下的变动处理通常如下：

- **Revaluation Increase（重估增值）**：通常计入 OCI，并累计在 Revaluation Surplus（重估盈余）中。
- 但如果该增值是转回同一资产此前计入损益的重估减值，则在此前损失金额范围内计入 Profit or Loss（损益）。
- **Revaluation Decrease（重估减值）**：通常计入 Profit or Loss。
- 但若该资产已有相关 Revaluation Surplus，则在该余额范围内先冲减 OCI 中的重估盈余，超过部分计入损益。

不要简单记成“所有重估增值都进 OCI、所有减值都进损益”；需要考虑同一资产此前的重估记录。

## 八、终止确认（Derecognition）

无形资产在以下情况终止确认：
- 处置（Disposal）；或
- 预计使用或处置该资产不再产生未来经济利益。

处置损益通常为：

\[
Gain\ or\ Loss\ on\ Disposal = Net\ Disposal\ Proceeds - Carrying\ Amount
\]

处置损益通常计入 Profit or Loss（损益），不作为 Revenue（营业收入）列报。

## 九、成本模型与重估模型对照

| 比较 | Cost Model | Revaluation Model |
|---|---|---|
| 初始计量 | Cost | 初始也按成本确认 |
| 后续计量基础 | 成本 | 重估日 Fair Value |
| 关键条件 | 无需活跃市场 | Fair Value 必须参考 Active Market |
| 后续摊销 | 有限寿命资产需要 | 有限寿命资产需要 |
| 后续减值 | 需要考虑 | 需要考虑 |
| 重估变动 | 不适用 | 按 IAS 38 规定计入 OCI 或损益 |

## 十、CFA 高频易错点

1. IAS 38 规定的后续计量模型是 Cost Model 和 Revaluation Model，不存在独立的 Fair Value Model。
2. Revaluation Model 必须有 Active Market 作为公允价值计量依据；无形资产的活跃市场通常罕见。
3. Finite Useful Life：摊销；Indefinite Useful Life：不摊销，但至少每年减值测试。
4. Research Phase 支出必须费用化；Development Phase 只有同时满足六项条件才资本化。
5. 企业合并取得的可辨认无形资产通常按购买日公允价值单独确认，不必因为被收购方以前未入账就并入商誉。
6. 内部生成品牌、客户名单及内部生成商誉通常不得确认为无形资产。
7. 重估增值通常进 OCI，但可能转回以前计入损益的重估减值；重估减值也可能先冲减已有重估盈余。
8. 处置无形资产的收益 / 损失通常进入损益，不列为营业收入。

## 十一、本题记录与复习检查

本题问 IFRS 下哪种模型最不可能用于报告无形资产。正确答案 **B：Fair Value Model**。IAS 38 允许 Cost Model 或满足活跃市场条件的 Revaluation Model；Fair Value 是重估模型的计量基础，不是独立的第三种模型。

- [ ] 能解释无形资产的定义和确认条件
- [ ] 能区分研究阶段与开发阶段支出
- [ ] 能说出开发阶段资本化的六项条件
- [ ] 能区分 Cost Model、Revaluation Model 与 Fair Value
- [ ] 能区分有限与不确定使用寿命的后续处理
- [ ] 能解释重估增值 / 减值的 OCI 与损益处理
- [ ] 能计算摊销、减值和处置损益


## 十二、研发支出：IFRS 与 US GAAP 对比（Research and Development Costs）

### 1. 核心对比表

先记住最重要的总规则：**研究阶段两套准则都费用化；开发阶段 IFRS 有条件允许资本化，US GAAP 通常费用化，但软件开发有专门例外。**

| 研发支出类型 | IFRS（IAS 38） | US GAAP | 核心判断 |
|---|---|---|---|
| Research Costs（研究支出） | 发生时费用化，不得资本化 | 通常发生时费用化 | 两套准则一致 |
| Development Costs（一般开发支出，非软件） | 六项条件全部满足后，满足条件的支出可资本化 | 通常发生时费用化 | 主要差异 |
| Software to be Sold / Leased / Marketed（对外销售、出租或营销的软件） | 研究阶段费用化；开发阶段满足 IAS 38 六项条件后可资本化 | ASC 985-20：达到 Technological Feasibility 后至产品可供一般发布前，符合条件的成本资本化 | US GAAP 有软件专门规则 |
| Internal-use Software（内部使用软件） | 按 IAS 38：研究阶段费用化；开发阶段满足六项条件后可资本化 | ASC 350-40：满足条件的 Application Development Stage（应用开发阶段）成本可资本化 | 两套准则的具体资本化门槛不同 |

**一句话记忆：**
- IFRS：Research Expense；Development 过六关后 Capitalize。
- US GAAP：R&D 通常 Expense；Software 有特定 Capitalization Exception。

### 2. IFRS：研究与开发如何划分？

- **Research（研究）**：旨在获取新科学或技术知识的原创性、有计划调查，技术与商业结果仍存在较大不确定性。
- **Development（开发）**：将研究成果或其他知识用于商业化生产或使用前的设计与开发，例如原型、工艺或产品。

**IFRS / IAS 38 的规则：**
1. Research Costs 必须在发生时 **Expensed as Incurred（发生时费用化）**。
2. Development Costs 只有从企业能够证明 IAS 38 六项资本化条件**同时满足之日**起，才可将之后符合条件的支出确认为无形资产。
3. 在六项条件满足之前已经费用化的支出，不得因为后续项目成功而重新资本化。
4. 若无法可靠地区分 Research 与 Development，全部支出按研究阶段费用化。

开发阶段资本化六项条件见本笔记第三章：Technical Feasibility、Intention to Complete、Ability to Use or Sell、Probable Future Economic Benefits、Adequate Resources、Reliable Measurement。

### 3. US GAAP：软件开发的两类例外

US GAAP 的一般研究与开发规则见 ASC 730：Research and Development Costs 通常在发生时费用化。但软件开发受专门准则约束，不能简单地说所有软件成本都费用化或都资本化。

**A. 对外销售、出租或营销的软件（ASC 985-20）**
- Technological Feasibility（技术可行性）达到之前：相关软件开发成本通常费用化。
- 达到技术可行性之后：到产品可供一般发布（Available for General Release）之前，符合条件的开发成本资本化。
- 产品可供一般发布之后：通常费用化后续维护和客户支持成本；符合条件的升级 / 增强成本另按规则判断。

**B. 内部使用软件（ASC 350-40）**
- Preliminary Project Stage（初步项目阶段）：通常费用化。
- Application Development Stage（应用开发阶段）：在项目已完成初步阶段、管理层授权并承诺资金，且完成和使用软件具有合理可能性等条件下，符合条件的直接成本资本化。
- Post-implementation / Operation Stage（实施后 / 运行阶段）：维护、培训等成本通常费用化，具体按准则判断。

### 4. 为什么 CFA 本题答案是 C？

题目比较 Hagar（US GAAP）与 Salome（IFRS）：

- A 错：IFRS 的 Research Phase 不会因为达到 Technical Feasibility 就变成可资本化的研究支出。技术可行性是开发阶段资本化条件之一；一旦项目进入开发阶段并且六项条件全部满足，才资本化符合条件的开发支出。
- B 错：IFRS 并非只有软件开发成本可以资本化；符合 IAS 38 六项条件的一般开发支出也可以资本化。
- C 对：Research Costs 在 IFRS 与 US GAAP 下通常都不得资本化，应在发生时费用化。

**正确答案：C。**

### 5. 费用化与资本化对财务报表的影响

在其他条件相同、资本化条件满足且暂不考虑后续摊销和减值的简化情形下：

| 影响 | Expensing（费用化） | Capitalization（资本化） |
|---|---|---|
| Income Statement（利润表） | 当期费用较高、当期利润较低 | 初始费用较少、当期利润较高；未来确认摊销或减值 |
| Balance Sheet（资产负债表） | 不确认对应开发资产 | 确认无形资产，初始资产及权益通常较高 |
| Cash Flow Statement（现金流量表） | 现金支出仍真实发生 | 现金支出仍真实发生；现金流分类需按准则判断 |

现金流量表提醒：IFRS 下符合条件并资本化的开发支出通常列为投资活动现金流（CFI），费用化的研发支出通常列为经营活动现金流（CFO）。US GAAP 下软件支出的现金流分类应结合具体规则和事实判断，不要仅凭“资本化”一词机械套用。**资本化不会让现金流出消失，只改变会计确认时点、利润确认节奏及可能的现金流列报分类。**

### 6. 考试速记

| 看到题目关键词 | 快速判断 |
|---|---|
| Research costs under IFRS | Expense as incurred |
| Development costs under IFRS | 六项条件全部满足后可资本化 |
| R&D costs under US GAAP | 通常费用化 |
| Software under US GAAP | 先判断外售软件还是内部使用软件，再套专门准则 |
| Technical feasibility | IFRS 开发阶段六项条件之一；外售软件 US GAAP 的重要资本化起点 |

### 7. 自测

- [ ] 能说出 IFRS 与 US GAAP 对 Research Costs 的共同处理
- [ ] 能解释 IFRS 为什么允许符合条件的 Development Costs 资本化
- [ ] 能区分 US GAAP 外售软件与内部使用软件的资本化门槛
- [ ] 能解释费用化 / 资本化对利润表、资产负债表和现金流量表的影响
