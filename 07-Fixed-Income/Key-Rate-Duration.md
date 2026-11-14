---
subject: Fixed Income
topic: Key Rate Duration
status: 待复习
created: 2026-11-01
tags: [CFA-L1, Fixed-Income, Yield-Curve]
---
# 关键利率久期（Key Rate Duration）

## 一句话理解
衡量**收益率曲线上某个特定期限节点利率变化**时，债券或组合价格的敏感度，其余关键节点尽量保持不变。

## 与修正久期区别
- 修正久期常用于估计收益率整体变化带来的价格影响。
- 关键利率久期用于分析收益率曲线**非平行移动**，如 2 年期上升而 10 年期下降。

## 常见近似
$$
KRD_i\approx\frac{P_i^- - P_i^+}{2P_0\Delta r_i}
$$
$P_i^-$ 和 $P_i^+$ 是对第 $i$ 个关键利率分别下调、上调 $\Delta r_i$ 后重估的价格。

## 易错点
关键利率久期依赖选取的节点、曲线扰动与重新定价方法；不要把某一个节点的 KRD 当作整个组合的总久期。

## 专题总览
[[Duration-Study-Guide|返回 Duration 久期专题：四种指标对比与速判]]
