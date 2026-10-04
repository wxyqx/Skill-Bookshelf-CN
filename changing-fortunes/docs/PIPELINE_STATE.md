# PIPELINE_STATE — changing-fortunes（时运变迁）

- 书源：时运变迁.epub（约 28.3 万字，10 章 + 3 附录 + 词汇表 + 年表）
- 蒸馏日期：2026-10-05，全自动模式（阶段 0/1.5 确认点不打断，最终统一汇报）

- [x] 准备：EPUB 解压 + spine 顺序文本提取（16 个 spine 项）
- [x] 阶段 0：整书理解 → docs/BOOK_OVERVIEW.md + docs/stage0-chapter-notes.md（14 份章节精读笔记，并行子代理按批次降级）
- [x] 阶段 1：5 提取器 → docs/candidates/{frameworks 20, principles 20, cases 18, counter-examples 18, glossary 19}.md（共 95 条候选）
- [x] 阶段 1.5：三重验证 → docs/verified.md（通过 14/23，通过率 61%，淘汰 9 条均为 V3 常识淘汰）+ docs/rejected/REJECTED.md
- [x] 阶段 2：RIA++ 构造 → skills/<slug>/SKILL.md ×14（六段完整，引用 ≤150 字，引文均经 grep 核实）
- [x] 阶段 3：docs/INDEX.md + docs/GLOSSARY.md + 14 个 SKILL.md 的 related_skills 回填（引用图 20 条边）
- [x] 阶段 4：压力测试 → 各 skill test-prompts.json（84 条用例）+ docs/TEST_RESULTS.md（独立 sub-agent 盲测，14/14 通过，诱饵容错 0）
- [x] 阶段 5：docs/DIGEST.md（约 8800 字精华长文）+ 入库推送
