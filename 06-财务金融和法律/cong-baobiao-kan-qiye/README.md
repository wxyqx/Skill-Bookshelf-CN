# 从报表看企业：数字背后的秘密（第5版）

由张新民《从报表看企业：数字背后的秘密（第5版）》（中国人民大学出版社，2024 年 1 月）蒸馏出的一组**可被 AI Agent 调用的技能**（Skills）。

> 把三张报表从"会计数字"还原成"企业故事"：以母公司报表为基础，先从资产结构看战略（经营/投资主导判型），再看效益质量与现金含量（核心利润获现率 1.2~1.5 倍）、看成本与价值，最后落到风险（金融负债率、占款指纹、撑死五信号）与前景（增长五途径）。17 个技能覆盖"八看"全视角、总纲流程与两件基础工具（母子报表对照、业务进三表推演）。

---

## 来源

| | |
|---|---|
| **书名** | 从报表看企业：数字背后的秘密（第5版） |
| **作者** | 张新民（中国人民大学教授，"财务状况质量分析理论"创立者） |
| **出版** | 中国人民大学出版社，2024-01，ISBN 9787300324166；第 1 版 2012 年源自 EMBA 课堂实录 |
| **蒸馏工具** | cangjie-skill（仓颉：把长内容蒸馏成可调用技能的流水线） |
| **蒸馏方法** | RIA-TV++：整书理解 → 并行提取（334 条原始候选）→ 去重合并（291 单元）→ 三重验证（76+31 通过）→ RIA++ 构造 → 集中盲测 → 交付 |
| **文本来源** | EPUB 提取全文约 21 万字，13 章切分 |
| **质量验证** | 结构终检 17/17 通过；集中盲测 119 题：硬性题 101/102，同书兄弟诱饵 34 条 0 失误 |

---

## 17 个技能

**总纲与基础能力**
- [`eight-lens-statement-analysis`](skills/eight-lens-statement-analysis/SKILL.md) — **八看总纲**：拿到全套报表做系统分析的四阶段流程+八步清单，单点问题调度到专项
- [`business-to-statements-deduction`](skills/business-to-statements-deduction/SKILL.md) — **业务进三表推演**：底子/面子/日子、实力/能力/活力、利润现金背离机理
- [`parent-vs-consolidated-statements`](skills/parent-vs-consolidated-statements/SKILL.md) — **母子报表对照**：控制性投资扩张效应差额、越合并越小、集团管理模式判别
- [`ratio-analysis-pitfalls`](skills/ratio-analysis-pitfalls/SKILL.md) — **比率七坑纠错**：经验值/口径/公式/前提逐条给替代动作
- [`financial-fraud-detection`](skills/financial-fraud-detection/SKILL.md) — **审计意见与造假信号**：五种审计意见烈度、常识反查法、六大红旗清单

**看战略**
- [`strategy-from-asset-structure`](skills/strategy-from-asset-structure/SKILL.md) — **从资产结构看战略**：母公司口径二分经营/投资资产，判型经营主导/投资主导/并重
- [`capital-source-four-drives`](skills/capital-source-four-drives/SKILL.md) — **资本引入与四大动力**：钱从哪来、分红政策、降杠杆路径
- [`governance-stance-analysis`](skills/governance-stance-analysis/SKILL.md) — **治理立场与占款识别**：大股东占款报表指纹链、不信人品信治理

**看经营资产与效益质量**
- [`two-end-eating-working-capital`](skills/two-end-eating-working-capital/SKILL.md) — **两头吃与营运资产**：上下游占款能力、流动比率<1 的正确解读、产品是否卖不动
- [`asset-quality-triage`](skills/asset-quality-triage/SKILL.md) — **逐项资产体检**：三层面质量观、其他应收款 1% 界限、不良资产区域定位
- [`income-statement-structure-analysis`](skills/income-statement-structure-analysis/SKILL.md) — **利润结构**：三支柱两减值、三个净利润分工、收入质量三问
- [`core-profit-cash-conversion`](skills/core-profit-cash-conversion/SKILL.md) — **核心利润获现率 1.2~1.5 倍**：利润是不是纸面利润的现金检验

**看价值与成本**
- [`valuation-ma-equity-pricing`](skills/valuation-ma-equity-pricing/SKILL.md) — **估值与并购定价**：入资三重效应、成本法/收益法边界、高商誉/零商誉正反面
- [`cost-determinants-impairment-attribution`](skills/cost-determinants-impairment-attribution/SKILL.md) — **成本决定与减值归因**：四层决定机制、减值归因决策 vs 管理、择机计提识别

**看风险与前景**
- [`financial-risk-debt-quality`](skills/financial-risk-debt-quality/SKILL.md) — **财务风险与负债质量**：金融负债率拆解、70% 界限语境化、利息保障倍数纠偏
- [`overexpansion-risk-signals`](skills/overexpansion-risk-signals/SKILL.md) — **过度扩张五信号**：存贷双高判别、投资补偿机制、企业不是饿死而是撑死
- [`prospect-forecast-growth-options`](skills/prospect-forecast-growth-options/SKILL.md) — **前景预测**：三步法、增长五途径、保壳重组识别、可研报告审阅

---

## 测试

每技能目录内含 `test-prompts.json`（3 正例 + 3 反例（含同书兄弟混淆诱饵）+ 1 边界例）与 `test-results.md`（集中盲测逐题记录）。

## docs

- `docs/BOOK_OVERVIEW.md` — 阶段 0 整书理解
- `docs/INDEX.md` — 技能总览与引用图
- `docs/GLOSSARY.md` — 65 条共享术语词典
- `docs/DIGEST.md` — 面向读者的精华长文
- `docs/verified.md` / `verified-cases.md` — 三重验证逐条判定与通过池
- `docs/candidates/` — 291 条去重后候选池（框架 54 / 原则 57 / 案例 80 / 反例 35 / 术语 65）+ 4 个扫描器原始产出
- `docs/rejected/` — 淘汰单元与原因
- `docs/PIPELINE_STATE.md` — 流水线状态
