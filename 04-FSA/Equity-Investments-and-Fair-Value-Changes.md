---
subject: Financial Statement Analysis
topic: Equity Investment Classification and Fair Value Changes
status: "🟡 解析能懂，待独立验证"
created: 2026-11-02
last-reviewed:
tags: [CFA-L1, FSA, Financial-Assets, Fair-Value, OCI]
---

# 权益投资分类与公允价值变动（Equity Investment Classification & Fair Value Changes）

## 一句话理解
股票投资（Equity Investment）在资产负债表上的计量金额，以及公允价值变动进入利润表（Income Statement）还是其他综合收益（Other Comprehensive Income, OCI），取决于适用会计准则和初始分类 / 指定。**不能仅因为股票尚未出售，就认为公允价值上涨不确认。**

## 一、本题数据与计算

题意：
- Gordon 于 2018 年 12 月 31 日买入上市公司普通股 1,000 million 股。
- 每股买入价 $7。
- 2019 年 12 月 31 日仍持有，年末每股公允价值 $10。

初始投资成本（Initial Cost）：

$$
1,000\ million\ shares\times\$7=\$7,000\ million
$$

年末公允价值（Fair Value）：

$$
1,000\ million\ shares\times\$10=\$10,000\ million
$$

公允价值上涨 / 未实现收益（Unrealized Gain）：

$$
(\$10-\$7)\times1,000\ million
=\$3,000\ million
$$

所以，年末资产负债表应按题目所适用的公允价值计量口径反映 $10,000 million；关键争议是 $3,000 million 的未实现收益进入 Net Income 还是 OCI。

## 二、题目采用的传统分类框架

本题选项使用 Trading / Available-for-Sale / Held-to-Maturity 术语，属于传统金融资产分类框架。按该题库的考试口径：

### 1. Trading Securities（交易性证券）
- 持有目的通常是近期出售、从短期价格波动中获利。
- 资产负债表：按公允价值列示。
- 未实现公允价值收益或损失：计入当期损益（Income Statement / Net Income）。

若本题归类为 Trading：
- Balance Sheet：$10,000 million。
- Income Statement：确认 $3,000 million gain。

### 2. Available-for-Sale Securities（可供出售证券，传统分类）
- 传统框架下通常按公允价值列示。
- 未实现公允价值变动通常计入其他综合收益（OCI），而不是当期净利润。
- 因此，若选项写成 AFS、资产 $10,000 million、同时把 $3,000 million gain 计入 Income Statement，则其损益列报不符合传统 AFS 处理。

### 3. Held-to-Maturity Securities（持有至到期证券）
- 仅适用于符合条件的债务证券（Debt Securities），不适用于普通股（Common Shares）。
- 需要有固定或可确定的付款以及固定到期日，并满足持有至到期的意图和能力等条件。
- 传统框架下通常按摊余成本（Amortized Cost）计量，而不是因市场价格上涨就调到公允价值。
- 普通股没有合同约定的到期日，因此本题不能分类为 HTM。

**本题正确选项：A（Trading Securities，资产负债表 $10,000 million；利润表确认 $3,000 million gain）。**

## 三、为什么“未出售”仍可能确认收益？

- **Realized Gain（已实现收益）**：通常在出售资产时实现。
- **Unrealized Gain（未实现收益）**：资产仍持有，但其计量价值已经上升。

在 Trading / FVTPL 类别下，未实现公允价值变动也计入当期损益。因此“没有卖出”不等于“利润表没有收益”。

## 四、现代准则口径提醒：不要把旧分类与新分类混为一谈

题目使用 Trading / AFS / HTM 的传统术语。学习时必须留意会计准则及教材版本。

### IFRS 9（国际财务报告准则第9号）
- 权益投资通常以公允价值计量且变动计入损益（Fair Value Through Profit or Loss, FVTPL），除非符合条件的非交易性权益工具在初始确认时作出不可撤销的 FVOCI 选择。
- **FVTPL**：公允价值变动进入 Profit or Loss（损益）。
- **FVOCI election for eligible equity investments**：符合条件的非交易性权益投资可选择将公允价值变动计入 OCI；该选择通常不可撤销，且处置时累计 OCI 不重分类至损益。

### US GAAP（美国会计准则）
- 对于适用 ASC 321 的权益证券，通常按公允价值计量，公允价值变动计入 Net Income；存在权益法、合并等适用例外。
- 传统 AFS / HTM 分类主要用于债务证券；不要把传统 AFS 债务证券的 OCI 处理机械套用到普通股权益证券。

因此，本题的 A 答案应结合题库所采用的传统分类术语理解；遇到明确要求 IFRS 9 或现行 US GAAP 的题目，应按相应现行准则作答。

## 五、关键术语对照

| 英文 | 中文 | 核心处理 |
|---|---|---|
| Trading Securities | 交易性证券 | 传统框架下公允价值变动进损益 |
| Available-for-Sale (AFS) | 可供出售证券 | 传统框架下未实现变动通常进 OCI |
| Held-to-Maturity (HTM) | 持有至到期证券 | 仅债务证券；传统框架下摊余成本 |
| FVTPL | 公允价值计量且变动计入损益 | 公允价值变动进损益 |
| FVOCI | 公允价值计量且变动计入其他综合收益 | 公允价值变动进 OCI |
| OCI | 其他综合收益 | 不直接计入当期净利润的特定综合收益项目 |
| Unrealized Gain | 未实现收益 | 持有期间公允价值上涨形成的收益 |
| Fair Value | 公允价值 | 计量日市场参与者有序交易中的退出价格 |

## 六、常见考试陷阱

1. 股票未出售，不代表公允价值变动一定不确认；Trading / FVTPL 下未实现收益也进损益。
2. 传统 Trading 与 AFS 的核心区别之一，是未实现公允价值变动进入 Income Statement 还是 OCI。
3. HTM 只适用于符合条件的债务证券，不适用于普通股。
4. AFS 在传统框架下也按公允价值列示，但未实现变动通常进 OCI，不是当期 Net Income。
5. IFRS 9 的 FVOCI 权益工具选择与传统 AFS 并不完全相同；处置时累计 OCI 通常不重分类至损益。
6. 先确认题目适用的准则与教材分类框架，再判断选项，避免将不同年代的准则术语混用。

## 七、本次题目记录

正确答案：**A**。投资成本为 $7,000 million，年末公允价值为 $10,000 million，未实现收益为 $3,000 million。按题目所用分类口径，Trading Securities 以公允价值列示，未实现收益计入 Income Statement。

- [ ] 能区分 Trading、传统 AFS、HTM
- [ ] 能区分 FVTPL 与 FVOCI
- [ ] 能解释 OCI 与 Net Income 的区别
- [ ] 能说明 HTM 为什么不适用于普通股
- [ ] 能根据题目指定准则选择正确处理
