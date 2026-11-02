---
subject: Financial Statement Analysis
topic: Earnings Per Share (EPS)
status: "🟡 解析能懂，待独立验证"
created: 2026-11-02
last-reviewed:
tags: [CFA-L1, FSA, EPS, Diluted-EPS]
---

# 每股收益（Earnings Per Share, EPS）

## 一句话理解
**EPS（Earnings Per Share，每股收益）**衡量归属于普通股股东的利润平均分配到每股普通股上的金额。Basic EPS 使用实际加权平均普通股股数；Diluted EPS 进一步考虑具有稀释作用的潜在普通股（Potential Common Shares）。

## 一、基本每股收益（Basic EPS）

### 1. 公式

$$
Basic\ EPS =
\frac{Net\ Income - Preferred\ Dividends}
{Weighted\ Average\ Common\ Shares\ Outstanding}
$$

- **Net Income（净利润）**：本期净利润。
- **Preferred Dividends（优先股股息）**：应从归属于普通股股东的利润中扣除。
- **Weighted Average Common Shares Outstanding（发行在外普通股加权平均股数）**：根据普通股在本期发行在外的时间加权计算。

若公司没有优先股，分子通常就是 Net Income。

### 2. 为什么使用加权平均股数？
普通股可能在年度中途发行或回购，因此不能简单使用期末股数。应按各批股份在本期发行在外的时间比例加权。

简化示例：
- 年初有 100 股，全年发行在外；
- 7 月 1 日新发行 20 股，假设下半年发行在外 6 个月。

$$
Weighted\ Average\ Shares
=100+20\times\frac{6}{12}=110
$$

股票股利（Stock Dividends）和股票拆分（Stock Splits）通常需要对比较期间及加权平均股数作追溯调整，仿佛相关变化在最早列报期间开始时已经发生。

### 3. 优先股股息处理
- **Cumulative Preferred Shares（累积优先股）**：计算当期 Basic EPS 时，扣除本期应计优先股股息，即使本期尚未宣告也通常需要扣除。
- **Non-cumulative Preferred Shares（非累积优先股）**：通常扣除本期已宣告的优先股股息。

## 二、稀释每股收益（Diluted EPS）

### 1. 核心概念
Diluted EPS 假设所有具有稀释作用（Dilutive）的潜在普通股都按相关条款转换或行权，从而重新计算每股收益。

潜在普通股（Potential Common Shares）可能包括：
- 可转换债券（Convertible Debt / Convertible Bonds）
- 可转换优先股（Convertible Preferred Shares）
- 股票期权（Stock Options）
- 认股权证（Warrants）

**Dilutive（具有稀释作用）**：纳入后 EPS 下降。
**Anti-dilutive（反稀释）**：纳入后 EPS 上升，或减少每股亏损；反稀释工具不得纳入 Diluted EPS。

### 2. 总体思路

$$
Diluted\ EPS =
\frac{Adjusted\ Earnings\ Available\ to\ Common\ Shareholders}
{Adjusted\ Weighted\ Average\ Common\ Shares}
$$

根据不同潜在普通股的假设转换 / 行权方法，分别调整分子和分母。

## 三、假设转换法（If-Converted Method）

适用于可转换债券和可转换优先股。

核心假设：将可转换证券视为在报告期初已经转换为普通股；若该证券在报告期内才发行，则从发行日起假设转换。该方法是计算稀释 EPS 的会计假设，并不表示证券在现实中已经转换或当时已经实际可转换。

### 1. 可转换债券（Convertible Debt）

**分子 Numerator：加回税后利息**

若债券转换成普通股，公司不再承担债券利息费用，但也失去利息税前扣除带来的税收利益。因此加回的是税后利息：

$$
After\text{-}tax\ Interest
=Interest\ Expense\times(1-Tax\ Rate)
$$

$$
Adjusted\ Net\ Income
=Net\ Income+After\text{-}tax\ Interest
$$

利息费用通常按债券面值 × 票面利率（Coupon Rate）计算；若题目给出实际利率、折价 / 溢价摊销或其他具体条件，应按题目要求确定利息费用。

**分母 Denominator：加上假设转换新增股份**

$$
New\ Shares =
\frac{Convertible\ Debt\ Face\ Value}{Conversion\ Denomination}
\times Shares\ per\ Denomination
$$

### 2. 可转换优先股（Convertible Preferred Shares）

若假设优先股转换成普通股：
- 分子：加回原本扣除的优先股股息（Preferred Dividends）。
- 分母：加上转换后新增的普通股股数。

优先股股息通常不享有债务利息相同的所得税抵扣，因此不乘以 (1 − Tax Rate)。

### 3. 本次 Gordon Co. 题目

题目数据：
- Net Income = $100 million
- Weighted Average Common Shares = 100 million
- Convertible Debentures 面值 = $10 million
- Coupon Rate = 10%
- 每 $100 债券可转换为 120 股
- Tax Rate = 30%
- 债券 2019 年全年发行在外；实际可转换日期为 2020 年 7 月 31 日。

**第一步：计算 Basic EPS**

$$
Basic\ EPS=\frac{100}{100}=\$1.00
$$

**第二步：计算税前利息**

$$
Interest=10\ million\times10\%=\$1\ million
$$

**第三步：加回税后利息**

$$
After\text{-}tax\ Interest
=1\times(1-30\%)=\$0.7\ million
$$

调整后分子：

$$
100+0.7=\$100.7\ million
$$

**第四步：计算新增股份**

$$
New\ Shares =
\frac{10,000,000}{100}\times120
=12,000,000
$$

调整后分母：

$$
100+12=112\ million\ shares
$$

**第五步：计算 Diluted EPS**

$$
Diluted\ EPS=\frac{100.7}{112}
=\boxed{\$0.8991}
$$

因此正确选项为 **A：$0.8991**。

**为什么不按 2020 年 7 月 31 日对 2019 年股份进行时间加权？**
If-Converted Method 假设报告期初转换（若证券本期发行，则从发行日开始），而不是按未来实际可转换日期计算实际发行股数。题目给出债券 2019 年全年发行在外，因此本题按全年假设转换处理。实际转换日不等于假设转换法的计算起点。

## 四、库存股法（Treasury Stock Method）

适用于股票期权（Stock Options）和认股权证（Warrants）。

核心假设：
1. 假设期权 / 认股权证在期初（或发行日）行权。
2. 公司收到行权款（Exercise Proceeds）。
3. 假设公司使用行权所得，按本期普通股平均市价（Average Market Price）回购普通股。
4. 只有净增加的股份计入 Diluted EPS。

### 1. 公式

$$
Shares\ Repurchased =
\frac{Exercise\ Proceeds}{Average\ Market\ Price}
$$

$$
Incremental\ Shares =
Options\ Exercised\ Shares - Shares\ Repurchased
$$

若有 N 份期权，每份可购买一股，行权价为 X，平均市价为 P：

$$
Incremental\ Shares=N-\frac{N\times X}{P}
$$

### 2. 示例
- 期权数量：1 million
- 行权价：$10
- 平均市场价格：$20

假设全部行权，公司收到 $10 million，并按 $20 回购：

$$
Shares\ Repurchased=\frac{10}{20}=0.5\ million
$$

$$
Incremental\ Shares=1-0.5=0.5\ million
$$

分母只增加 0.5 million 股，而不是全部 1 million 股。

### 3. 重要判断
- 若 Average Market Price 高于 Exercise Price，通常产生增量股份，具有稀释性。
- 若 Exercise Price 不低于 Average Market Price，则没有正的增量股份，通常不产生稀释。
- Treasury Stock Method 通常不调整分子，因为假设行权不产生债券利息或优先股股息的节省。

## 五、稀释性与反稀释性（Dilutive vs Anti-dilutive）

不能看到潜在普通股就全部纳入。必须判断其是否降低 EPS。

对于单一可转换工具，可用其增量 EPS 进行初步判断：

$$
Incremental\ EPS =
\frac{Earnings\ Added\ Back}{Shares\ Added}
$$

- 若 Incremental EPS 低于当前 EPS，纳入后通常会降低 EPS，属于 Dilutive。
- 若 Incremental EPS 高于当前 EPS，纳入后通常会提高 EPS，属于 Anti-dilutive，应排除。

若存在多种潜在普通股，需要按稀释程度从高到低逐项测试，并在每一步重新计算；反稀释工具不能纳入。

## 六、方法对照

| 项目 | If-Converted Method | Treasury Stock Method |
|---|---|---|
| 适用工具 | 可转换债券、可转换优先股 | 股票期权、认股权证 |
| 分子调整 | 债券加回税后利息；优先股加回股息 | 通常不调整 |
| 分母调整 | 加上假设转换的全部新增股份 | 只加净增量股份 |
| 核心假设 | 假设转换为普通股 | 假设行权，再用所得回购股份 |

## 七、常见考试陷阱

1. Basic EPS 的分子不是一概等于 Net Income；有优先股时要考虑 Preferred Dividends。
2. 分母使用 Weighted Average Common Shares，不一定是期末股数。
3. 可转换债券加回的是税后利息：Interest × (1 − Tax Rate)。
4. 可转换优先股加回优先股股息，不按债券利息方式税后调整。
5. Treasury Stock Method 只增加净增量股份，不是全部期权股份。
6. 若工具具有 Anti-dilutive 效果，不能纳入 Diluted EPS。
7. If-Converted Method 是假设转换，不代表实际转换；通常按报告期初或发行日作为假设起点。
8. Coupon Rate 是票面利率；若题目给出债券折价 / 溢价和实际利率信息，需辨别用于计算的利息费用口径。

## 八、典型题型 / 解题路径

**Basic EPS：**
1. 先确定 Net Income。
2. 扣除适用的 Preferred Dividends。
3. 计算 Weighted Average Common Shares。
4. 相除得到 Basic EPS。

**Convertible Debt / Preferred：**
1. 识别转换工具。
2. 用 If-Converted Method。
3. 调整分子：加回税后利息或优先股股息。
4. 调整分母：加转换后的普通股。
5. 检查是否 Dilutive；Anti-dilutive 则排除。

**Options / Warrants：**
1. 识别行权数量和行权价。
2. 计算行权所得。
3. 假设按平均市价回购股份。
4. 只把净增量股份计入分母。
5. 检查是否产生稀释。

## 我的错因 / 验证记录

Gordon Co. 题目答对，关键计算：
- 税后利息加回：$10m × 10% × (1 − 30%) = $0.7m。
- 新增股份：($10m / $100) × 120 = 12m 股。
- Diluted EPS = ($100m + $0.7m) / (100m + 12m) = $0.8991。

需继续巩固：
- [ ] 能独立计算 Basic EPS 与加权平均股数
- [ ] 能独立运用 If-Converted Method
- [ ] 能独立运用 Treasury Stock Method
- [ ] 能识别 Dilutive 与 Anti-dilutive securities
- [ ] 能解释税后利息为何加回
- [ ] 能独立完成一道同类新题
