# INDEX — 《从报表看企业：数字背后的秘密（第5版）》 skill 总览

> 来源：张新民"八看"体系（人大社 2024-01）。共 **17 个 skills**，覆盖总纲、基础能力与"八看"全部视角。
> 每个 skill 目录内含 `SKILL.md`（R/I/A1/A2/E/B 六段）+ `test-prompts.json` + `test-results.md`。

## 总纲与基础能力

| Skill | 一句话定位 |
|---|---|
| [eight-lens-statement-analysis](../skills/eight-lens-statement-analysis/SKILL.md) | 拿到全套报表做系统分析的总纲：四阶段流程+八步清单+单点问题调度 |
| [business-to-statements-deduction](../skills/business-to-statements-deduction/SKILL.md) | 业务逐笔过三表推演教学：底子/面子/日子、实力/能力/活力 |
| [parent-vs-consolidated-statements](../skills/parent-vs-consolidated-statements/SKILL.md) | 母公司报表与合并报表对照技术：控制性投资、扩张效应差额、"越合并越小" |
| [ratio-analysis-pitfalls](../skills/ratio-analysis-pitfalls/SKILL.md) | 财务比率七大误用纠错：经验值、口径、公式、前提，逐条给替代动作 |
| [financial-fraud-detection](../skills/financial-fraud-detection/SKILL.md) | 审计意见五类型+关键审计事项+造假/粉饰信号清单（常识反查法） |

## 看战略

| Skill | 一句话定位 |
|---|---|
| [strategy-from-asset-structure](../skills/strategy-from-asset-structure/SKILL.md) | 从母公司资产结构判战略类型：经营/投资/并重型，扩张路径与表外资源 |
| [capital-source-four-drives](../skills/capital-source-four-drives/SKILL.md) | 钱从哪来：资本引入四来源、发展四大动力、分红政策与降杠杆 |
| [governance-stance-analysis](../skills/governance-stance-analysis/SKILL.md) | 大股东占款报表指纹链、治理结构风险、"不信人品信治理" |

## 看经营资产与效益质量

| Skill | 一句话定位 |
|---|---|
| [two-end-eating-working-capital](../skills/two-end-eating-working-capital/SKILL.md) | "两头吃"与上下游占款能力、营运资产竞争力、产品是否卖不动 |
| [asset-quality-triage](../skills/asset-quality-triage/SKILL.md) | 逐项资产体检：三层面、其他应收款 1% 界限、不良资产区域定位 |
| [income-statement-structure-analysis](../skills/income-statement-structure-analysis/SKILL.md) | 利润从哪来：三支柱两减值、三个净利润分工、收入质量三问 |
| [core-profit-cash-conversion](../skills/core-profit-cash-conversion/SKILL.md) | 核心利润获现率 1.2~1.5 倍：利润是不是纸面的现金检验 |

## 看价值与成本

| Skill | 一句话定位 |
|---|---|
| [valuation-ma-equity-pricing](../skills/valuation-ma-equity-pricing/SKILL.md) | 并购/股权交易定价四步、成本法收益法边界、高商誉/零商誉正反面 |
| [cost-determinants-impairment-attribution](../skills/cost-determinants-impairment-attribution/SKILL.md) | 成本四层决定机制、减值归因决策 vs 管理、减值择机调节识别 |

## 看风险与前景

| Skill | 一句话定位 |
|---|---|
| [financial-risk-debt-quality](../skills/financial-risk-debt-quality/SKILL.md) | 偿债能力评估：金融负债率拆解、70% 界限语境化、利息保障倍数纠偏 |
| [overexpansion-risk-signals](../skills/overexpansion-risk-signals/SKILL.md) | 过度融资/投资"撑死"五信号、存贷双高判别、投资补偿机制 |
| [prospect-forecast-growth-options](../skills/prospect-forecast-growth-options/SKILL.md) | 前景预测三步法、增长五途径盘点、保壳重组识别、可研报告审阅 |

## 引用图（related_skills 摘要）

- **调度关系**：eight-lens（总纲）在四个阶段分别调度 parent-vs-consolidated（对照）、各专项（单点深挖）、prospect-forecast（前景）。
- **depends-on**：strategy-from-asset-structure ← parent-vs-consolidated-statements（母公司口径）；core-profit-cash-conversion ← income-statement-structure-analysis（先结构后现金）。
- **contrasts-with**：strategy-from-asset-structure ↔ capital-source-four-drives（资产投向 vs 资金来源）；financial-risk-debt-quality ↔ overexpansion-risk-signals（存量负债 vs 扩张流量）。
- **composes-with**：asset-quality-triage + cost-determinants（先体检后归因）；governance-stance + financial-fraud-detection（治理侵占 vs 报表粉饰两面）。

## 推荐阅读顺序

1. 入门：business-to-statements-deduction → ratio-analysis-pitfalls
2. 实战主线：strategy-from-asset-structure → income-statement-structure-analysis → core-profit-cash-conversion → financial-risk-debt-quality
3. 避坑：financial-fraud-detection → governance-stance-analysis → overexpansion-risk-signals
4. 进阶：parent-vs-consolidated-statements → valuation-ma-equity-pricing → prospect-forecast-growth-options
