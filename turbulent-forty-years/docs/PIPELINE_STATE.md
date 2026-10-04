# PIPELINE_STATE — turbulent-forty-years（激荡四十年）

- 书源：激荡四十年.epub（正文约 77 万字，《激荡十年》+《激荡三十年》全三册，44 个年度章+两篇前言）
- 蒸馏日期：2026-10-05，全自动模式（阶段 0/1.5 确认点不打断，最终统一汇报）

- [x] 准备：EPUB 解压 + spine 62 项合并为 13 part + 按年度章拆分为 44 章
- [x] 阶段 0：整书理解 → docs/BOOK_OVERVIEW.md + docs/stage0-chapter-notes.md（44 份年度章精读，15 组×3 代理并行降级）
- [x] 阶段 1：5 提取器 → docs/candidates/{frameworks 20, principles 20, cases 18, counter-examples 18, glossary 20}.md（共 96 条候选）
- [x] 阶段 1.5：三重验证 → docs/verified.md（40 条候选去重为 27 单元，通过 16，通过率 59%，11 单元均为 V3 常识淘汰）+ docs/rejected/REJECTED.md
- [x] 阶段 2：RIA++ 构造 → skills/<slug>/SKILL.md ×16（六段完整，引用 ≤150 字，引文均经 grep 核实）
- [x] 阶段 3：docs/INDEX.md + docs/GLOSSARY.md + 16 个 SKILL.md 的 related_skills 回填（引用图 28 条边）
- [x] 阶段 4：压力测试 → 各 skill test-prompts.json（96 条用例）+ docs/TEST_RESULTS.md（独立 sub-agent 盲测 95/96 → 修补 property-rights-timing / business-government-distance 触发边界 → 复测 96/96，诱饵容错 0）
- [x] 阶段 5：docs/DIGEST.md（约 8000 字精华长文）+ 入库推送
