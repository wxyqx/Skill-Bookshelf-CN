# PIPELINE_STATE — 财务报表分析

- 书 slug: financial-statement-analysis
- 来源: D:\桌面\32490-财务报表分析\财务报表分析.pdf(292 页,文本层完整,非扫描版)
- 开始: 2026-10-05

| 阶段 | 状态 | 产出 |
|---|---|---|
| 提取 | ✅ | _source/book_full.txt + ch1-ch7/appendix.txt(31 万字,PDF页=书页+16) |
| 阶段 0 | ✅ | BOOK_OVERVIEW.md(6 骨架论点,13 术语,4 类批判) |
| 阶段 1 | ✅ | _digests/ 8 章 + _candidates_raw/ 7 文件 274 条 → candidates/ 五池 224 条 |
| 阶段 1.5 | ✅ | _verify/verified_A(58)+verified_B(23) → verified.md(81 单元→18 skill) + rejected/ 36 条 |
| 阶段 2 | ✅ | 标杆 strategic-analysis-path 盲测 6/6;17 个 builder skill 全部产出 |
| 阶段 3 | ✅ | INDEX.md(18 skill 六组)+ GLOSSARY.md(47 术语) |
| 阶段 4 | ✅ | 终检脚本全过;集中盲测 111/111(含全部兄弟混淆诱饵 0 误触发);test-results.md 18 份 |
| 阶段 5 | 🔄 | DIGEST.md(8165 字)已产出;书架五处同步;push;清理本地 |

## skill 清单(18)
strategic-analysis-path, project-quality-entry, cash-quality-funding-risk, receivables-and-funneling, inventory-and-margin, long-term-asset-quality, asset-allocation-strategy, capital-structure-four-forces, profit-quality-3d, revenue-quality-three-questions, non-operating-income-quality, cash-flow-three-activities, consolidation-pitfalls, differential-analysis, ratio-revision-rules, earnings-manipulation-tactics, profit-deterioration-sweep, off-statement-strategy-blindspots

## 注意事项
- 原书 PDF 文本层有零星错字(权贵发生制/历吏成本/质最/资产负侦表),产出时一律写正确字
- 版权:R 段引用 ≤60 字(比红线 150 字更严)
- 子代理并发上限 3-4,失败等 30 秒补发
