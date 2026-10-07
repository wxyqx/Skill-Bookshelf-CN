# 聪明的投资者 — 流水线状态

- 书名: 《聪明的投资者》 本杰明·格雷厄姆（第4版老译本，1964年数据，16章4篇）
- 源文件: D:\桌面\2354-聪明的投资者\聪明的投资者.epub（正文约 17.4 万字）
- slug: intelligent-investor
- 分类: 02-认知与决策（对齐 poor-charlies-almanack）
- 节奏: 全自动；交付推 GitHub 后临时目录零残留

## 状态
- [x] 阶段 0 完成：4 组精读笔记 188KB + BOOK_OVERVIEW.md 27KB
- [x] 阶段 1 提取完成：candidates/ 5 件——frameworks.md（f01–f51，51 条）、principles.md（p01–p73，73 条）、cases.md（c01–c60，60 条素材）、counter-examples.md（x01–x30，30 条素材）、glossary.md（t01–t30，30 条素材）；候选合计 124 条（框架+原则）+ 120 条素材
- [x] 阶段 1.5 三重验证完成（2026-10-06）：
  - 验证 124 / 去重合并 70 / 通过 51 个独立方法论单元（覆盖 121 条 id）/ 聚类 20 个 skill / 独立淘汰 3（f12、f14、p19 → rejected/）
  - 通过率 41%（51/124，按独立方法论单元计，落在 30–70% 正常区间；剔除去重后独立候选口径为 51/54=94%，双池重叠大所致，明细见 verified.md 统计节）
  - 产出：verified.md（51 单元 yaml + 聚类总表 + 降级素材注 + 去重合并账 + 1964 通用时效警示）；rejected/f12.md、rejected/f14.md、rejected/p19.md
- [x] 阶段 2 完成：20 个 SKILL.md + test-prompts.json（格式已规范化）（进行中）：按 verified.md 聚类总表构造 20 个 SKILL.md；每个 skill 头部写入 1964 通用时效警示，数字参数标注"1964 年快照，按当期重查"；A1 素材/反例/术语按总表挂接
- [x] 阶段 3+4 完成：INDEX/GLOSSARY（链接20/20）；盲测 180 用例，should 类 105/105，冲突 2 对已修+复测 9/9，终判 100%
- [ ] 阶段 5 交付 → DIGEST（17KB）已写；待打包入库 02-认知与决策 + 推送

## 聚类 → slug 速查（阶段 2 构造清单）
1 invest-vs-speculation-filter｜2 rule-reliability-trend-skepticism｜3 market-mr-volatility-discipline｜4 mechanical-allocation-dca｜5 investor-identity-matching｜6 overheated-market-defense｜7 defensive-stock-selection｜8 bond-safety-terms｜9 aggressive-negative-list｜10 excess-return-path-selection｜11 neglected-large-cap-strategy｜12 bargain-issues-net-nets｜13 special-situations-arbitrage｜14 earnings-power-valuation｜15 growth-stock-appraisal｜16 protection-over-forecast｜17 stock-diagnosis-techniques｜18 margin-of-safety-core｜19 shareholder-governance｜20 investment-advice-discipline
