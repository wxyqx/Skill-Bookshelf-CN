# PIPELINE_STATE — 21st-century-monetary-policy（21世纪货币政策）

- 书源：21世纪货币政策.epub（正文约 38.5 万字，导读+前言+15 章）
- 蒸馏日期：2026-10-05，全自动模式（阶段 0/1.5 确认点不打断，最终统一汇报）

- [x] 准备：EPUB 解压 + spine 顺序文本提取（30 个 spine 项，正文 17 节）
- [x] 阶段 0：整书理解 → docs/BOOK_OVERVIEW.md + docs/stage0-chapter-notes.md（17 份章节精读笔记，并行子代理 3 个/批降级）
- [x] 阶段 1：5 提取器 → docs/candidates/{frameworks 20, principles 20, cases 18, counter-examples 18, glossary 19}.md（共 95 条候选）
- [x] 阶段 1.5：三重验证 → docs/verified.md（40 条候选去重为 27 单元，通过 16，通过率 40%，11 单元均为 V3 常识淘汰）+ docs/rejected/REJECTED.md
- [x] 阶段 2：RIA++ 构造 → skills/<slug>/SKILL.md ×16（六段完整，引用 ≤150 字，引文均经 grep 核实）
- [x] 阶段 3：docs/INDEX.md + docs/GLOSSARY.md + 16 个 SKILL.md 的 related_skills 回填（引用图 28 条边）
- [x] 阶段 4：压力测试 → 各 skill test-prompts.json（96 条用例）+ docs/TEST_RESULTS.md（独立 sub-agent 盲测，16/16 通过，诱饵容错 0，30 条兄弟混淆诱饵全对）
- [x] 阶段 5：docs/DIGEST.md（约 8000 字精华长文）+ 入库推送
