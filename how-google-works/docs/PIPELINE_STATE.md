# PIPELINE_STATE — 《重新定义公司：谷歌是如何运营的》

> cangjie-skill RIA-TV++ 流水线状态。每完成一个阶段更新本文件（断点续跑依据）。

## 元信息

- **book-slug**: `how-google-works`
- **书名**: 《重新定义公司：谷歌是如何运营的》（*How Google Works*）
- **作者**: 埃里克·施密特、乔纳森·罗森伯格（与艾伦·伊格尔合著）；中文版靳婷婷译，中信出版社 2015
- **来源**: D:\桌面\3994-重新定义公司\重新定义公司.epub
- **全文文本**: `_source/book_full.txt`（202,431 字，48 个 spine 文件合并，含前言/六章/结语/注释/词汇表/致谢，无缺章）
- **执行模式**: 无人值守（用户要求与上一本同样处理：蒸馏 + 上传 skill-bookshelf-CN，不安装本地）；阶段 0/1.5 的确认点改为在最终交付报告中事后展示
- **降级记录**: 子代理多次遭遇"Captcha verification timed out"与并发配额限制——提取器改为单只串行重试（5 只全部成功）；阶段 2+4 由主流程写出 1 个标杆 skill（hippo-resistance），其余 17 个由 4 只 builder 串行构造，主流程程序化校验 18/18 通过

## 阶段状态

| 阶段 | 状态 | 产出 |
|---|---|---|
| 0 整书理解 (Adler) | ✅ 完成 | BOOK_OVERVIEW.md（骨架 8 单元/术语 20+ 条（含原书自带词汇表锚点）/批判 4 类/应用潜力 23 主题） |
| 1 并行提取 | ✅ 完成 | candidates/：frameworks 51 · principles 227 · cases 92 · counter-examples 62 · glossary 25（合计 457） |
| 1.5 三重验证 | ✅ 完成 | verified.md（合并 25 单元 → 通过 18 / 淘汰 7，含防作弊校准声明）；rejected/：7 个淘汰文件 + 4 个依附簇文件，278 条参选候选全部有归属 |
| 2 RIA++ 构造 | ✅ 完成 | 18 个 `skills/<slug>/SKILL.md`（R/I/A1/A2/E/B 六段齐全，引文均 ≤150 字；frontmatter 含 related_skills，共 15 条真实关系） |
| 3 Zettelkasten 链接 | ✅ 完成 | INDEX.md（18 skills + 引用图 + 学习顺序）+ GLOSSARY.md（25 条升格 + 术语→skill 映射） |
| 4 压力测试 | ✅ 完成 | 各 skill `test-prompts.json`（各 6 条：3 trigger + 2 诱饵含 1 跨 skill + 1 edge）+ `test-results.md`（fallback 主流程自测 18×6/6，已标注可信度限制与回炉点） |
| 5 交付 | ✅ 完成 | DIGEST.md（精华长文）；已按书架规范发布到 `wxyqx/skill-bookshelf-CN` 的 `how-google-works/`（按用户要求**不安装**到本地 skills 目录） |

## 录取的 18 个 skill（slug 定稿）

1. `hippo-resistance` 别听河马的话（HiPPO 抗性：让数据与论据说话）
2. `org-design-rules` 组织设计三律（7 的法则+两个比萨+影响力中心）
3. `expel-villains-protect-stars` 驱逐恶棍，保护明星
4. `technical-insight-first` 计划必错，信赖技术洞见
5. `open-as-strategy` 开放为王与选择封闭的前提
6. `focus-user-think-10x` 聚焦用户，往大处想
7. `hiring-quality-bar` 招聘质量律（羊群效应/宁缺毋滥/宁"漏聘"不"误聘"）
8. `talent-portrait` 人才画像（学习型动物/机场测试/加大光圈）
9. `hiring-ops` 招聘组织化（全员出动/招聘委员会/30 分钟面试）
10. `retention-playbook` 留汰律（换出巧克力/电梯演讲/爱他就让他走）
11. `real-consensus` 共识的真正含义（共识≠人人同意）
12. `decision-timing-discipline` 决策时机与授权（响铃/80-80/马背原则/PIA）
13. `default-open-candor` 默认开放与讲真话的安全环境（最牛的路由器）
14. `resource-70-20-10` 70/20/10 资源配置原则
15. `twenty-percent-time` 20% 时间制（重点在自由，不在时间）
16. `ship-iterate-fail-well` 交付—迭代与败得漂亮
17. `innovation-chaos` 创新不可指派（缔造原始的混沌）
18. `ask-hard-questions` 把难题提出来（5 年"可能会怎样"与组织自检）

## 用户事后确认点（无人值守模式的替代安排）

- 阶段 0 确认：BOOK_OVERVIEW.md 随最终报告展示，可要求修改骨架/批判后再拆。
- 阶段 1.5 确认：通过 18 / 淘汰 7 名单见 verified.md；若要捞回，优先候选为 rejected/p14（拥挤出成绩，作者核心体验但 V3 判常识）与 rejected/cluster-okr（OKR 簇，并入 focus-user-think-10x）。
