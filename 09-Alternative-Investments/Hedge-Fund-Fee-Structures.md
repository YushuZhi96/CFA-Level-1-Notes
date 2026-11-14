---
subject: Alternative Investments
topic: Hedge Fund Fee Structures
status: "🟢 单题独立答对，待复测"
created: 2026-11-12
last-reviewed: 2026-11-12
tags: [CFA-L1, Alternative-Investments, Hedge-Funds, Fees, Hurdle-Rate, Fund-of-Funds]
---

# 对冲基金费用结构（Hedge Fund Fee Structures）

[[09-Alternative-Investments/INDEX|返回另类投资目录]]

相关概念：[[Hedge-Fund-Basics|对冲基金基础知识]]（对冲基金、FOF 优势与风险）。本笔记保留收费结构及计算方法。

## 一句话理解

对冲基金（Hedge Fund）常见收费包括**管理费（Management Fee）**和**业绩报酬（Incentive Fee）**。计算前必须确认：管理费以何时点的 AUM 为基数、业绩报酬是否先扣管理费、是否设有门槛收益率（Hurdle Rate）或高水位线（High-Water Mark）。

## 核心概念 / 定义

- **Assets Under Management (AUM)｜管理资产规模**：基金所管理的资产规模；题目可能分别给出期初（Beginning AUM）或期末（Year-end AUM）。
- **Management Fee｜管理费**：按规定的 AUM 计费基础乘以费率，通常与当期投资盈利是否超过门槛无直接关系。
- **Incentive Fee / Performance Fee｜业绩报酬**：根据满足合同规定条件的投资利润计提的费用。
- **Hurdle Rate｜门槛收益率**：决定业绩报酬计提门槛的最低回报要求。
- **Hard Hurdle｜硬门槛**：达到门槛后，一般仅对**超过门槛的利润部分**计提业绩报酬。
- **Soft Hurdle｜软门槛**：一旦超过门槛，一般对**全部符合合同定义的利润**计提业绩报酬，而不仅是超出门槛的部分。
- **High-Water Mark (HWM)｜高水位线**：历史净资产价值高点限制，用于避免在尚未弥补此前亏损时就重复收取业绩报酬；实际调整依合同约定。

## 公式与变量

设：

- $A_0$：期初 AUM（Beginning AUM）
- $A_1$：期末、扣本期费用前的 AUM（Ending AUM Before Fees）
- $m$：管理费率（Management Fee Rate）
- $i$：业绩报酬率（Incentive Fee Rate）
- $h$：硬门槛收益率（Hard Hurdle Rate）

### 1. 管理费（Management Fee）

若明确规定以期末 AUM 为基数：

$$
\text{Management Fee}=A_1\times m
$$

**注意**：若题干规定期初 AUM、平均 AUM 或其他基数，必须按题干执行，不可固定用期末值。

### 2. 业绩报酬（Incentive Fee）：独立于管理费计算 + 硬门槛

当题干说明 **calculated independently from management fees（独立于管理费计算）**、无其他费用限制且不存在影响计算的 HWM 等约束时：

$$
\text{Investment Gain}=A_1-A_0
$$

$$
\text{Hurdle Profit}=A_0\times h
$$

$$
\text{Incentive Fee}=i\times\max\left[0,(A_1-A_0)-A_0h\right]
$$

$$
\text{Total Fees}=\text{Management Fee}+\text{Incentive Fee}
$$

**适用条件**：以上为无外部申购赎回、无其他调整、已明确业绩报酬独立计算的简化题型。若规定先扣管理费（net of management fees），应按题意先调整可计费利润；不能机械套用。

### 3. 先扣管理费后计提业绩报酬（Net of Management Fees）+ Hard Hurdle

当题干明确规定 **Management Fee based on Beginning AUM（管理费按期初 AUM 计提）**、**Incentive Fee net of Management Fees（业绩报酬以扣除管理费后的利润为基础）**，并采用 Hard Hurdle 时，可按以下步骤计算。

管理费：

$
M=A_0m
$

扣除管理费后的可计费利润：

$
G_{\text{after management fee}}=(A_1-A_0)-M
$

硬门槛对应的最低利润（按期初 AUM 计算）：

$
H=A_0h
$

业绩报酬（假设无其他约束）：

$
I=i\times\max\left(0,G_{\text{after management fee}}-H\right)
$

投资者最终净收益率（Net Rate of Return）：

$
r_{\text{net}}=\frac{A_1-A_0-M-I}{A_0}
$

若以扣费前收益率 $r=(A_1-A_0)/A_0$ 表示，上述特定条件下的快捷公式：

$
\boxed{r_{\text{net}}=r-m-i\max(0,r-m-h)}
$

**适用条件**：单一计费期、无追加投资或赎回、无影响费用的高水位线、期初 AUM 为管理费和门槛基数、业绩报酬先扣管理费且只有超过硬门槛的部分计费。若合约规定门槛以其他基数、扣费顺序或净值口径计算，需要按题干调整。

**对比记忆**：

- **Independent of Management Fees**：计算业绩报酬时不先扣管理费；此前第 2 小节的公式适用。
- **Net of Management Fees**：先扣管理费后判断超门槛利润；使用本小节公式。
- **Net Rate of Return** 是投资者扣除所有相关基金费用后的收益率，不等于费用合计。

### 4. Hard Hurdle 与 Soft Hurdle

在不考虑其他限制的简化场景中：

- **Hard Hurdle**：业绩报酬率只乘以超过门槛的利润。
- **Soft Hurdle**：若盈利越过门槛，业绩报酬率通常乘以全部符合约定的利润；未越过门槛则不收取。
- 不同基金可约定不同的分配方式；**不能将 Hard/Soft 与 High-Water Mark 混为一谈**。

## 基金中的基金：双层费用（Fund of Hedge Funds and Double-Layered Fees）

### 概念与英文词汇

- **Fund of Hedge Funds (FoHF)｜对冲基金中的基金**：上层基金将资金配置到多只底层对冲基金（Underlying Funds）；其费用可能叠加在底层基金费用之上。
- **Underlying Fund Fees｜底层基金费用**：底层基金按各自合同收取的管理费及业绩报酬。
- **Double-Layered Fees｜双层收费**：投资者可能同时负担底层基金和上层 FoHF 的管理费与业绩报酬。
- **Net of Underlying Fund Fees｜扣除底层基金费用后**：上层基金的相关计费基础先扣除底层基金费用；**不自动表示也先扣除上层基金自身的管理费**。
- **Gross of Fees｜扣费前**；**Net of Fees｜扣费后**。
- **Appreciation｜资产增值**：基金资产价值上涨；题目出现 **before fees** 时，给出的期末价值尚未扣除所述费用。
- **Neither ... nor ...｜既不……也不……**：在费用题中留意其所否定的对象。关于哪些基金适用 Hurdle Rate 或 HWM，应依照完整题干的明确陈述判断，不能由残缺片段假设所有基金都没有限制。

### 计算顺序（通用框架，不预设费率）

设 $V_0$ 为期初资金，$V_1$ 为扣除所有相关费用前的期末资产价值；$M_U$、$I_U$ 为底层管理费、业绩报酬；$M_F$、$I_F$ 为上层 FoHF 管理费、业绩报酬。

1. **底层管理费（Underlying Management Fee）**：依底层基金合同的 AUM 基数、时点和费率计算 $M_U$。
2. **底层业绩报酬（Underlying Incentive Fee）**：按利润、费用扣除顺序、门槛收益率及高水位线等条件计算 $I_U$。
3. **扣除底层费用（Net of Underlying Fund Fees）**：

$
V_{\text{after underlying fees}}=V_1-M_U-I_U
$

4. **上层 FoHF 管理费**：依据合同规定，选择期初、期末扣除底层费用后或其他计费基数，得到 $M_F$。
5. **上层 FoHF 业绩报酬**：确认是否进一步扣除上层管理费，以及是否存在 Hurdle Rate / High-Water Mark，再得到 $I_F$。
6. **全部基金费用（Total Fees Earned by All Funds）**：

$
\boxed{F_{\text{total}}=M_U+I_U+M_F+I_F}
$

**适用边界**：以上是分层计费框架，并非固定的四个费率公式；如题目有多只底层基金，先依规定逐只计费，再汇总其费用或净值。上层管理费与业绩报酬的实际计费基数、扣费顺序及是否设门槛，须由完整条款确定。

### 常见考试陷阱

1. **只算底层费用**：题干问 *all funds* 时，不能漏算上层 FoHF 费用。
2. **Net of Underlying vs. Net of Own Management Fee**：扣除底层基金费用不等于一定先扣除 FoHF 自己的管理费。
3. **Gross vs. Net Asset Value**：题目给出扣费前期末资产价值时，不能当成已经扣费后的金额。
4. **Missing Fee Terms**：仅凭期初、期末资产规模，若不知道两层费率和计费顺序，就无法唯一算出总费用；不应根据选项反推出假设费率并视为题目事实。
5. **No Hurdle / HWM**：即使题目明确没有门槛和高水位线，也仍需根据合同规则计算管理费、业绩报酬及两层之间的扣减顺序。

### 复习记录

- 已学习 Fund of Hedge Funds 的双层费用结构和 *net of underlying fund fees* 的含义。
- 该截图只提供部分题干，**未核实两层收费费率及计费基数，不归档任何推测的数值答案**。
- 本知识点状态：🟡 规则已讲解，完整计算待验证。

## 直观理解 / 记忆方法

- **Management Fee：管多少钱，就按题目指定的 AUM 基数算管理费。**
- **Incentive Fee：赚多少钱能分成，先看门槛与高水位线。**
- **Hard = only excess（只对超额部分收费）**。
- **Soft = once above threshold, charge on eligible profits（超过门槛后对约定的全部适用利润收费）**。

## 常见考试陷阱

1. **Beginning vs. Year-end AUM**：管理费基数应按题干，不要未经判断就取期初资产。
2. **Independently vs. Net of Management Fees**：业绩报酬是否预先扣除管理费，直接影响结果。
3. **Hard vs. Soft Hurdle**：硬门槛只对超出部分计费；软门槛越过门槛后通常对全部适用利润计费。
4. **Hurdle Rate vs. High-Water Mark**：前者是回报门槛，后者关注是否重新超过历史高点；两者可以同时存在，计算优先次序以合同为准。
5. **Gross vs. Net / Fees timing**：基金计费基数、估值时点和是否发生资金流入流出，需要按题目口径调整。
6. **Units**：AUM 为 billion 时费用答案也是 billion；不能混淆金额与收益率。
7. **Total Fees vs. Net Return**：总费用是金额；投资者净收益率是扣除管理费和业绩报酬后收益除以期初资本。

## 典型题型 / 判断路径

1. 标注期初与期末 AUM、管理费率、业绩报酬率。
2. 圈出收费基数和 **independently / net of** 关键词。
3. 识别 **Hard / Soft Hurdle** 以及是否有 **High-Water Mark**。
4. 依约计算 Management Fee 与 Incentive Fee；如果求 **Total Fees**，则两项费用相加；如果求 **Net Rate of Return**，则从期末资产减去全部费用后计算净收益率。

## 易混知识点 / Obsidian 链接

- [[Alternative-Investments-Basics|另类投资基础：分类、管理、收益与风险]]
- [[GP-Catch-Up|GP Catch-Up（私募基金追赶机制）]]：私募基金分配瀑布与对冲基金业绩报酬算法是不同机制，不可直接混用。

## 我的错因 / 验证记录

- 已完成一道典型的 **Year-end AUM + Independent Incentive Fee + Hard Hurdle** 计算题，**独立答对一次**。
- 新增一组 **Beginning AUM + Net of Management Fees + Hard Hurdle + Net Rate of Return** 计算规则；不以题目展示的答案状态推定已独立掌握。
- 复习状态：🟢 曾独立答对一题；**净收益率及费用顺序的变式仍待独立验证**。
- 题目原文、选项与原题数字不归档。

## 复习检查清单

- [x] 已独立答对一次硬门槛计算题
- [ ] 不看提示能解释 Hard Hurdle 与 Soft Hurdle 的区别
- [ ] 能处理 independent 与 net of management fees 两种计费顺序及其不同公式
- [ ] 能解释 HWM 的作用并识别相关约束
- [ ] 能根据期初/期末管理费基数计算投资者 Net Rate of Return
- [ ] 能说明 FoHF 双层收费的计算顺序及相关计费基数
- [ ] 能解释 net of underlying fund fees 与 net of management fees 的区别
- [ ] 能独立完成一道变式题
