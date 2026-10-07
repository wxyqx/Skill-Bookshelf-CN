# PIPELINE_STATE — china-reform-trilogy（中国改革三部曲）

- [x] 准备：EPUB 提取（89 万字，三部曲合一）+ 29 个文件切分（12 讲 + 11 章 + 6 章 + 前言附录）
- [x] 阶段 0：整书理解 → docs/BOOK_OVERVIEW.md + docs/stage0-chapter-notes.md（2026-10-04，6 个精读代理+作者补读，自动确认模式）
- [x] 阶段 1：提取器 → docs/candidates/{frameworks 10, principles 8, cases 10, counter-examples 6, glossary 12}.md
- [x] 阶段 1.5：三重验证 → docs/verified.md（通过 10）+ docs/rejected/REJECTED.md（合并/降级 8）
- [x] 阶段 2：RIA++ 构造 → skills/<slug>/SKILL.md ×10（六段完整，引用 ≤150 字）
- [x] 阶段 3：docs/INDEX.md + docs/GLOSSARY.md（三种改革叙事的对照定位）
- [x] 阶段 4：skills/*/test-prompts.json ×10（含跨书混淆诱饵）+ docs/TEST_RESULTS.md（10/10 通过）
- [x] 阶段 5：docs/DIGEST.md + README.md；仓库形式交付，跳过本地安装
- [x] 推送 GitHub wxyqx/skill-bookshelf-CN（根 README + booklist.md 同步，第 31 本书）
- [x] 删除本地临时目录（含 full.txt 全文）——本地零残留

模式：全自动（与前几卷一致）。
质量红线自检：10 个 skill 均通过三重验证；本卷为书架"中国改革叙事"第三视角（理论/方案设计者），与黄奇帆两卷（实操）、温铁军两卷（代价）建立三角对照导航；每个 skill 的 B 段保留"规范性理论可行性论证偏弱/自反风险"元批判（ce06）；DIGEST 含反例陷阱与作者局限章节。
