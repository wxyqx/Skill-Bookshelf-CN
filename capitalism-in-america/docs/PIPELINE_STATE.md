# PIPELINE_STATE — capitalism-in-america（繁荣与衰退：一部美国经济发展史）

- [x] 准备：EPUB 提取（35.7 万字）+ 引言/12 章/大结局/附录切分（src/）
- [x] 阶段 0：整书理解 → docs/BOOK_OVERVIEW.md + docs/stage0-chapter-notes.md（2026-10-04，5 个精读代理，自动确认模式）
- [x] 阶段 1：提取器 → docs/candidates/{frameworks 9, principles 6, cases 10, counter-examples 5, glossary 10}.md
- [x] 阶段 1.5：三重验证 → docs/verified.md（通过 8）+ docs/rejected/REJECTED.md（合并/降级/跨书对照 7）
- [x] 阶段 2：RIA++ 构造 → skills/<slug>/SKILL.md ×8（六段完整，引用 ≤150 字）
- [x] 阶段 3：docs/INDEX.md + docs/GLOSSARY.md（含与布林德卷、中国三卷的对照定位）
- [x] 阶段 4：skills/*/test-prompts.json ×8（含跨书混淆诱饵）+ docs/TEST_RESULTS.md（8/8 通过）
- [x] 阶段 5：docs/DIGEST.md + README.md；仓库形式交付，跳过本地安装
- [x] 推送 GitHub wxyqx/skill-bookshelf-CN（根 README + booklist.md 同步，第 32 本书）
- [x] 删除本地临时目录（含 full.txt 全文）——本地零残留

模式：全自动（与前几卷一致）。
质量红线自检：8 个 skill 均通过三重验证；第十一章大衰退与布林德卷主题重叠，处理为跨书对照案例不重建；每个 skill 的 B 段保留"MFP 残差循环论证/进步史对称性缺口/联储主席自证回避"元批判（ce01/ce02/ce05）；DIGEST 开篇与局限章节均提示史观的账本选择性。
