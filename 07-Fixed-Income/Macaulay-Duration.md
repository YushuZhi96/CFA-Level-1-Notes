---
subject: Fixed Income
topic: Macaulay Duration
status: 待复习
created: 2026-11-01
tags: [CFA-L1, Fixed-Income, Duration]
---
# 麦考利久期（Macaulay Duration）

## 一句话理解
债券现金流**按现值占总价格的比例加权**后的平均收款时间（单位：期，转换后可为年）。

## 必记公式
$$
D_{Mac}=\sum_{t=1}^{N}t\frac{PV(CF_t)}{P}
$$
其中 $P=\sum PV(CF_t)$；$t$ 必须与折现周期保持一致。若 $t$ 用每半年付息期数表示，最终除以每年付息次数，才得到“年”。

## 直观记忆
每笔现金流“多重要”用现值权重衡量，“等多久”用时间衡量。

## 易错点
- **麦考利久期**是时间；**修正久期**用于债券收益率变动带来的价格敏感度近似。
- 对正现金流的普通固定利率债，零息债券的麦考利久期等于到期期限；付息债的久期通常短于到期日。
- 收益率、付息频次、时间单位不能混用。

## 关联
[[Modified-Duration]] · [[Key-Rate-Duration]]

## 专题总览
[[Duration-Study-Guide|返回 Duration 久期专题：四种指标对比与速判]]
