---
subject: Fixed Income
topic: Modified Duration
status: 待复习
created: 2026-11-01
tags: [CFA-L1, Fixed-Income, Duration]
---
# 修正久期（Modified Duration）

## 核心公式
当年化到期收益率 $y$ 以每年 $m$ 次复利、麦考利久期以**年**为单位时：
$$
D_{Mod}=\frac{D_{Mac}}{1+y/m}
$$
小幅平行变动的近似（忽略凸性）：
$$
\frac{\Delta P}{P}\approx -D_{Mod}\Delta y
$$
$\Delta y$ 是年化收益率的小数变化：50 bps = 0.005。

## 易错点
- 收益率上升，普通固定利率债价格通常下降；负号不能漏。
- 久期只提供一阶近似；收益率变化较大时需考虑凸性。
- 不能拿麦考利久期直接代替修正久期做百分比价格变动近似。

## 关联
[[Macaulay-Duration]] · [[Key-Rate-Duration]]
