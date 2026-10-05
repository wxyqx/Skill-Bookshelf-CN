# PIPELINE_STATE — eight-crises（八次危机：中国的真实经验 1949-2009）

- [x] 准备：TXT 结构识别（UTF-8，23.2 万字）+ 7 段切分（前言/四章/展望对策/附录）
- [x] 阶段 0：整书理解 → docs/BOOK_OVERVIEW.md + docs/stage0-chapter-notes.md（2026-10-04，自动确认模式）
- [x] 阶段 1：提取器 → docs/candidates/{frameworks 11, principles 10, cases 12, counter-examples 7, glossary 12}.md
- [x] 阶段 1.5：三重验证 → docs/verified.md（通过 10）+ docs/rejected/REJECTED.md（淘汰/降级/合并 12）
- [x] 阶段 2：RIA++ 构造 → skills/<slug>/SKILL.md ×10（六段完整，引用 ≤150 字）
- [x] 阶段 3：docs/INDEX.md + docs/GLOSSARY.md（含与姊妹卷框架的互补对照）
- [x] 阶段 4：skills/*/test-prompts.json ×10（含跨书混淆诱饵）+ docs/TEST_RESULTS.md（10/10 通过）
- [x] 阶段 5：docs/DIGEST.md + README.md；仓库形式交付，跳过本地安装
- [x] 推送 GitHub wxyqx/skill-bookshelf-CN（根 README + booklist.md 同步，第 28 本书）
- [x] 删除本地临时目录（含 full.txt 全文）——本地零残留

模式：全自动（与前两卷一致）。
质量红线自检：10 个 skill 均通过三重验证；本卷无跨书同族框架（作者不同源），与姊妹卷三个 skill 建立"互补对照"关系；test-prompts 均含兄弟混淆诱饵；DIGEST 含反例陷阱与作者局限章节（含框架循环论证风险的元批判）。
