# PIPELINE_STATE — xiaomi-startup-thinking（小米创业思考）

- 书源：小米创业思考.epub（正文约 20.5 万字，14 章 + 前言/后记/附录五篇演讲与公开信）
- 蒸馏日期：2026-10-05，全自动模式（阶段 0/1.5 确认点不打断，最终统一汇报）
- 入库分类：04-创业与经营

- [x] 准备：EPUB 解压 + spine 32 项提取（26 个正文文件）
- [x] 阶段 0：整书理解 → docs/BOOK_OVERVIEW.md + docs/stage0-chapter-notes.md（14 份章节精读，8 组子代理）
- [x] 阶段 1：5 提取器 → docs/candidates/{frameworks 22, principles 20, cases 18, counter-examples 17, glossary 20}.md（共 97 条候选）
- [x] 阶段 1.5：三重验证 → docs/verified.md（42 条候选去重为 31 单元，通过 28，通过率 90%，3 条 V3 淘汰；28 单元按主题聚类为 17 个 skill）+ docs/rejected/REJECTED.md
- [x] 阶段 2：RIA++ 构造 → skills/<slug>/SKILL.md ×17（六段完整，引用 ≤150 字，引文均经 grep 核实）
- [x] 阶段 3：docs/INDEX.md + docs/GLOSSARY.md + 17 个 SKILL.md 的 related_skills 回填（引用图 34 条边）
- [x] 阶段 4：压力测试 → 各 skill test-prompts.json（102 条用例）+ docs/TEST_RESULTS.md（独立 sub-agent 盲测 101/102 → 修补 minority-stake-empowerment 边界排除条款 → 复测 102/102，诱饵容错 0，24 条兄弟混淆诱饵全对）
- [x] 阶段 5：docs/DIGEST.md（约 8000 字精华长文）+ 入库推送
