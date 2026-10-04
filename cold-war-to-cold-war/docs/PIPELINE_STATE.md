# PIPELINE_STATE — cold-war-to-cold-war（从"老冷战"到"新冷战"）

- [x] 准备：PDF 提取（PyMuPDF，51 页 / 正文 5.7 万字）+ 5 章切分（src/）
- [x] 阶段 0：整书理解 → docs/BOOK_OVERVIEW.md + docs/stage0-chapter-notes.md（2026-10-04，作者本人通读无子代理；自动确认模式）
- [x] 阶段 1：提取器 → docs/candidates/{frameworks 10, principles 7, cases 8, counter-examples 6, glossary 11}.md
- [x] 阶段 1.5：三重验证 → docs/verified.md（通过 9）+ docs/rejected/REJECTED.md（合并/淘汰 8；f02 并入 f01）
- [x] 阶段 2：RIA++ 构造 → skills/<slug>/SKILL.md ×9（六段完整，引用 ≤150 字）
- [x] 阶段 3：docs/INDEX.md + docs/GLOSSARY.md（含与姊妹卷互补对照）
- [x] 阶段 4：skills/*/test-prompts.json ×9（含跨书混淆诱饵）+ docs/TEST_RESULTS.md（9/9 通过）
- [x] 阶段 5：docs/DIGEST.md + README.md；仓库形式交付，跳过本地安装
- [x] 推送 GitHub wxyqx/skill-bookshelf-CN（根 README + booklist.md 同步，第 29 本书）
- [x] 删除本地临时目录（含 full.txt 全文）——本地零残留

模式：全自动（与前几卷一致）。
质量红线自检：9 个 skill 均通过三重验证；与《八次危机》同作者无同族重复，与黄奇帆卷三处互补对照；每个 skill 的 B 段保留作者"单向叙事/强意图推断"的元批判（ce06）；DIGEST 开篇与局限章节均作对称性提示。
