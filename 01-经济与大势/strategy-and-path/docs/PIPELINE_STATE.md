# PIPELINE_STATE — strategy-and-path（战略与路径：黄奇帆的十二堂经济课）

- [x] 准备：EPUB 解压 + 12 章文本提取（src/，30.4 万字）
- [x] 阶段 0：整书理解 → docs/BOOK_OVERVIEW.md + docs/stage0-chapter-notes.md（2026-10-04，自动确认模式）
- [x] 阶段 1：5 提取器 → docs/candidates/{frameworks 19, principles 20, cases 25, counter-examples 10, glossary 15}.md
- [x] 阶段 1.5：三重验证 → docs/verified.md（通过 19）+ docs/rejected/REJECTED.md（淘汰/降级/合并 14）
- [x] 阶段 2：RIA++ 构造 → skills/<slug>/SKILL.md ×19（六段完整，引用 ≤150 字）
- [x] 阶段 3：docs/INDEX.md + docs/GLOSSARY.md
- [x] 阶段 4：skills/*/test-prompts.json ×19（含兄弟混淆诱饵）+ docs/TEST_RESULTS.md（19/19 通过）
- [x] 阶段 5：docs/DIGEST.md（精华长文）+ README.md（书目录页）；按"仓库形式交付"跳过本地安装
- [x] 推送 GitHub wxyqx/skill-bookshelf-CN + 更新书架根 README（第 20 本书）
- [x] 删除本地临时目录（含 src/ 全文文本）——本地零残留

模式：全自动（阶段 0/1.5 确认点自动通过，结论记录于 BOOK_OVERVIEW.md 与 verified.md）。
质量红线自检：19 个 skill 均通过三重验证与六段完整性检查；test-prompts.json 均含 ≥2 条诱饵（其中 1 条为同书兄弟混淆）；DIGEST 含反例陷阱与作者局限章节。
