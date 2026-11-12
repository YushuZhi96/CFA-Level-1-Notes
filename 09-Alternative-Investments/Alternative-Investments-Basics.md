---
subject: Alternative Investments
topic: Alternative Investment Categories, Active Management and Diversification
status: "🟡 解析能懂，待独立验证"
created: 2026-11-11
last-reviewed: 2026-11-12
tags: [CFA-L1, Alternative-Investments, Categories, Diversification, Active-Management, Alpha]
---

# 另类投资基础：分类、主动管理与分散化（Categories, Active Management and Diversification）

[[09-Alternative-Investments/INDEX|返回另类投资目录]]

## 一句话理解

另类投资基金（Alternative Investment Funds）通常采取**主动管理（Active Management）**，希望通过主动选资产、运营改善、特殊交易策略或寻找市场低效机会，争取获得**正 Alpha（Positive Alpha）**。**追求正 Alpha 不代表一定能获得正 Alpha。**

## 传统投资与另类投资的界限

- **Traditional Investments｜传统投资**：典型包括公开交易的股票（Equities）、债券（Bonds）、现金和现金等价物（Cash and Cash Equivalents）。
- **Alternative Investments｜另类投资**：传统股债现金投资以外的资产或投资策略；具体基金可能通过非上市股权、实物资产、特殊策略或数字资产获取收益。
- **Treasury Bonds｜国债**与**Preferred Stocks｜优先股**都属于传统证券类别；即使国债有时与股票低相关，也不因此变成另类投资。

## 另类投资包含哪些内容？（Categories of Alternative Investments）

以下为复习时便于识别的四部分概览框架，具体产品可能跨类别：

1. **Private Capital｜私募资本**
   - **Private Equity｜私募股权**：投资非公开市场股权，如 **Venture Capital｜风险投资** 与 **Leveraged Buyout (LBO)｜杠杆收购**。
   - **Private Debt｜私募债务**：通过非公开渠道向企业提供债务融资，例如 **Direct Lending｜直接贷款**。
2. **Real Assets｜实物资产**
   - **Real Estate｜房地产**：住宅、写字楼、商业及物流物业等；回报可能来自租金收入（Rental Income）与资产增值（Property Appreciation）。
   - **Infrastructure｜基础设施**：机场、收费道路、电网等，回报可能受合同、监管、使用量影响。
   - **Natural Resources｜自然资源**：包括 **Commodities｜大宗商品**（如能源、金属）及 **Farmland｜农田**、**Timberland｜林地** 等。
3. **Hedge Funds｜对冲基金**：主要依策略区分，而非仅看其持有的资产；常见 **Long/Short｜多空**、**Event-Driven｜事件驱动**、**Arbitrage｜套利**；可能运用 **Leverage｜杠杆** 与 **Derivatives｜衍生品**。对冲基金即使持有股票，也可以属于另类投资。
4. **Digital Assets｜数字资产**：例如 **Cryptocurrencies｜加密货币**、**Tokens｜代币** 等；涉及 **Blockchain｜区块链** 技术及相应资产风险。

### 典型特征（不是每项资产必然具备）

- 可能存在较低流动性（Liquidity）、较低透明度（Transparency）、较复杂估值（Valuation）和更高管理成本（Management Costs）。
- 往往较依赖主动管理（Active Management），但有些另类资产产品也采用规则化或被动策略。
- 资产类别和实际投资工具不完全等价：例如直接持有房地产与购买上市房地产证券，其流动性和股票市场相关性可能不同。

## 投资组合分散化与低相关性（Diversification and Low Correlation）

- **Correlation｜相关性**描述两项收益率之间的线性联动程度；相关系数（Correlation Coefficient）$\\rho$ 取值范围为 $[-1,1]$。
- **Portfolio Diversification｜投资组合多样化**：组合持有相关性不完全为 $+1$ 的资产，通常能够降低组合风险；在其他条件相同时，相关性越低，潜在分散化效益越明显。

$
\\rho_{A,B} = \\frac{\\operatorname{Cov}(R_A,R_B)}{\\sigma_A\\sigma_B}
$

- $\\rho=+1$：完全正线性相关；$\\rho=0$：无线性相关（**不表示统计独立**）；$\\rho=-1$：完全负线性相关。
- **Diversification Benefits｜分散化效益**是另类投资可能带来的重要价值，但**另类投资并不保证低相关、低波动或不会亏损**。在金融压力时期，房地产、股票等也可能同步下跌。
- **Low Correlation ≠ Low Risk**：低相关说的是与其他资产的联动，不代表资产本身风险低。
- **Traditional vs. Alternative** 是资产/策略分类；**Correlation** 是两种收益的统计关系。国债属于传统投资，也可能在部分时期与股票低相关；房地产属于另类投资，但并非始终与股债低相关。

## 核心概念 / 定义

- **Active Management｜主动管理**：管理人依靠研究、判断和具体投资决策，试图取得超越适当风险调整基准的表现。
- **Passive Management｜被动管理**：主要复制指数、规则化跟踪基准或尽量降低主动偏离；并非另类投资基金的典型管理方式。
- **Alpha｜阿尔法（风险调整后超额收益）**：投资组合相对于给定风险定价模型所预期收益的超出部分；不应简单等同于“收益率为正”。
- **Beta｜贝塔（系统性风险敏感度）**：衡量组合收益对市场或相关风险因子变动的敏感程度；并非“市场收益率”的同义词。
- **Market Inefficiency｜市场低效**：市场价格未能充分或即时反映相关信息、流动性或结构性因素时，管理人可能寻找定价机会。
- **Efficient Market Hypothesis (EMH)｜有效市场假说**：市场价格在相应有效性形式下反映相关信息；市场越有效，持续创造风险调整后超额收益通常越困难。

## 公式与变量

Alpha 的一般理解：

$$
\alpha = R_{\text{actual}}-R_{\text{model expected}}
$$

如果明确采用 CAPM 作为预期收益模型，可写为 Jensen's Alpha（詹森 Alpha）：

$$
\alpha_p = R_p - \left[R_f + \beta_p(R_m - R_f)\right]
$$

- $R_p$：投资组合收益率（Portfolio Return）
- $R_f$：无风险收益率（Risk-Free Rate）
- $R_m$：市场组合收益率（Market Return）
- $\beta_p$：投资组合的市场 Beta（Portfolio Beta）

**适用条件**：第二个公式仅对应以 CAPM 衡量的 Alpha；另类投资策略可能存在多风险因子、非线性敞口等，具体 Alpha 衡量应以适当模型为准。

## 典型策略与直观理解

- **Private Equity｜私募股权**：主动选择、收购和经营改善企业，尝试增加投资价值。
- **Hedge Funds｜对冲基金**：主动采用多空、套利或其他交易策略，寻求投资机会。
- **Real Estate｜房地产投资**：通过选址、运营、租约管理或资产升级改善回报。

这些例子说明另类投资为何通常依赖管理人能力，但具体产品未必都采用主动管理。

## 易混知识点 / 考试陷阱

1. **Active vs. Passive**：另类投资基金通常是 Active，不要因为“基金”一词就默认是被动指数基金。
2. **Alpha vs. Beta**：Alpha 是模型风险调整后的超额部分；Beta 表示风险敏感度。基金涨幅高不自动意味着 Alpha 为正。
3. **Seek vs. Achieve**：“寻求正 Alpha”是管理目标，不是收益承诺。
4. **EMH vs. Alpha**：有效市场假说不等于绝对不存在错误定价或正 Alpha；但强市场效率会增加持续创造超额收益的难度。
5. **Typically vs. Always**：题干若说“通常”，不应误解成所有另类投资基金一律主动管理。
6. **Asset Category vs. Correlation**：国债即使与股票低相关仍属于传统投资；房地产虽属另类投资，也不保证始终低相关。
7. **Low Correlation vs. Low Risk**：低相关与低风险不同；判断资产时不能只看波动或“安全性”。

## 我的错因 / 验证记录

- 易错倾向：将另类投资基金误认为通常采用 **Passive Management**。
- 修正逻辑：另类投资基金通常由管理人积极选择投资机会，以争取 **Positive Alpha**。
- 易错倾向：把“国债可能与股票低相关”误当作“国债属于另类投资”。
- 修正逻辑：**先判断资产类别（Traditional / Alternative），再分析与其他资产的收益相关性（Correlation）**。
- 复习状态：🟡 解析能懂，待独立验证。

## 复习检查清单

- [ ] 能说清 Active Management 和 Passive Management 的区别。
- [ ] 能区分 Alpha 与 Beta，不把高绝对收益当作必然的正 Alpha。
- [ ] 能解释为何市场低效可能为主动管理创造机会。
- [ ] 能识别 “typically / seek positive alpha” 的考试措辞。
- [ ] 能归类 Private Capital、Real Assets、Hedge Funds 与 Digital Assets，并举出各自典型资产/策略。
- [ ] 能区分传统债券与另类实物资产，不混淆分类和相关性。
- [ ] 能解释低相关性为什么可能产生分散化效益，以及其局限性。
- [ ] 不看解析，能独立判断同类新题。
