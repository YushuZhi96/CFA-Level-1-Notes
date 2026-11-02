---
subject: Financial Statement Analysis
topic: Goodwill Initial Recognition and Measurement
status: "🟡 解析能懂，待独立验证"
created: 2026-11-02
last-reviewed:
tags: [CFA-L1, FSA, Goodwill, Business-Combination]
---

# 商誉的初始确认与计量（Goodwill: Initial Recognition & Measurement）

## 一句话理解
**商誉（Goodwill）是在企业合并（Business Combination）中，购买方转移的对价及其他规定项目，超过所取得可辨认净资产公允价值份额的剩余金额。** 计算时关注可辨认净资产的公允价值（Fair Value），而不是被收购方原有的账面价值（Book Value）。

## 一、基础公式：100% 收购

在购买方取得 100% 股权、没有原先持有权益等简单情形下：

$$
Goodwill = Purchase\ Price - FV(Net\ Identifiable\ Assets)
$$

其中：

$$
FV(Net\ Identifiable\ Assets)
=FV(Identifiable\ Assets)-FV(Liabilities\ Assumed)
$$

- **Purchase Price / Consideration Transferred（购买价格 / 转移的对价）**：购买方为取得被收购方控制权而转移的对价。
- **Identifiable Assets（可辨认资产）**：符合确认条件、能够与商誉区分的资产。
- **Liabilities Assumed（承担的负债）**：购买方在企业合并中承担的负债。
- **Fair Value（公允价值）**：企业合并购买日的公允价值计量基础。

## 二、完整公式：企业合并

若不是简单的 100% 收购，IFRS 3 下商誉计算一般为：

$$
\begin{aligned}
Goodwill ={}& Consideration\ Transferred \\
&+ Fair\ Value\ of\ NCI \\
&+ Fair\ Value\ of\ Previously\ Held\ Equity\ Interest \\
&- FV(Net\ Identifiable\ Assets)
\end{aligned}
$$

- **NCI (Non-controlling Interest，非控制性权益)**：被收购方中不归属于购买方的权益。
- **Previously Held Equity Interest（原先持有的股权）**：分阶段收购（Step Acquisition）中，购买方在取得控制权前已持有的权益；取得控制权日需按规定重新计量。
- 若购买方收购 100%，没有 NCI，也没有原先持有权益，完整公式就简化为基础公式。

注意：IFRS 3 下，对每笔企业合并，NCI 可按公允价值（Full Goodwill Method）或按其在可辨认净资产中的比例份额（Partial Goodwill Method）计量；具体选项影响确认的商誉金额。

## 三、计算示例

假设购买方收购一家公司的全部股权：

| 项目 | 金额 |
|---|---:|
| Purchase Price（购买价格） | $1,200万 |
| Identifiable Assets 的公允价值 | $1,500万 |
| Liabilities Assumed 的公允价值 | $700万 |
| Net Identifiable Assets 的公允价值 | $800万 |

先计算可辨认净资产公允价值：

$$
1,500-700=800\text{ 万}
$$

再计算商誉：

$$
Goodwill=1,200-800=\boxed{400\text{ 万}}
$$

若被收购方账面净资产只有 $500 万，也不能用 $1,200 万减 $500 万计算商誉；应先按购买日公允价值计量可辨认资产和负债。

## 四、为什么 Book Value 不直接影响商誉？

被收购方原有资产负债表上的账面价值（Book Value）是按其过去的会计计量基础形成的，可能与购买日公允价值不同。

企业合并时，购买方需要识别并计量取得的可辨认资产和承担的负债，通常按购买日公允价值确认（适用准则另有规定的项目除外）。

因此：
- Purchase Price / Consideration：影响商誉。
- Fair Value of Identifiable Net Assets：影响商誉。
- Acquiree's historical Book Value：不是商誉公式中的直接变量。

账面价值仍可能作为评估和公允价值调整的参考信息，但不能直接替代购买日公允价值。

## 五、廉价购买收益（Bargain Purchase Gain）

如果在重新检查所有计量后：

$$
FV(Net\ Identifiable\ Assets)
> Consideration + FV(NCI) + FV(Previously\ Held\ Interest)
$$

则差额可能形成 **Bargain Purchase Gain（廉价购买收益）**，通常在购买日计入损益，而不是确认“负商誉”。

## 六、商誉后续计量（Subsequent Measurement）

- 商誉在资产负债表中作为资产单独列示，但不能独立于业务或现金产生单元产生现金流。
- IFRS 下商誉不进行定期摊销（Amortization），而是至少每年进行减值测试（Impairment Test），并在出现减值迹象时测试。
- 商誉减值损失（Goodwill Impairment Loss）通常计入当期损益；IFRS 下已确认的商誉减值不得转回。

## 七、常见考试陷阱

1. 计算商誉使用可辨认净资产的 **Fair Value**，不是被收购方原有 **Book Value**。
2. Net Identifiable Assets = 可辨认资产公允价值 − 承担负债公允价值。
3. 100% 收购的简化公式：Purchase Price − FV(Net Identifiable Assets)。
4. 非 100% 收购可能还需加上 NCI；分阶段收购还需考虑 Previously Held Equity Interest。
5. NCI 的计量方法可能影响确认的商誉金额（Full vs Partial Goodwill）。
6. 计算结果为负数时，重新检查计量后可能形成 Bargain Purchase Gain，不是确认负商誉。
7. IFRS 下商誉不定期摊销，但需要进行减值测试。

## 八、本次题目记录

题目问商誉初始确认最不可能受哪项影响。正确答案 **C：Acquiree's Book Value**。

判断路径：
- A Purchase Price：进入公式，影响商誉。
- B Fair Value of Identifiable Net Assets：进入公式，影响商誉。
- C Acquiree's Book Value：不是公式中的直接变量，因此最不可能影响商誉。

- [ ] 能独立写出 100% 收购商誉公式
- [ ] 能独立写出包含 NCI 和原先持有权益的完整公式
- [ ] 能区分 Fair Value 与 Book Value
- [ ] 能计算 Bargain Purchase Gain
- [ ] 能解释商誉后续减值处理
