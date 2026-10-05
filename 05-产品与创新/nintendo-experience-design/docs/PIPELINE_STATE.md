# PIPELINE_STATE — 《任天堂的体验设计》

> cangjie-skill RIA-TV++ 流水线状态。每完成一个阶段更新本文件（断点续跑依据）。

## 元信息

- **book-slug**: `nintendo-experience-design`
- **书名**: 《任天堂的体验设计——创造不知不觉打动人心的体验》
- **作者**: 玉树真一郎（前言/第1-3章拆解 Wii、马里奥、DQ、最后生还者、风之旅人）
- **来源**: E:\download\任天堂的体验设计 _ 创造不知不觉打动人心的体验(Wx-Library).epub
- **全文文本**: `_source/book_full.txt`（66,495 字，2 个 spine HTML 转出，含附录，无缺章）
- **执行模式**: 无人值守（用户要求一次完成"蒸馏 + 上传 GitHub"）；阶段 0/1.5 的用户确认点改为在最终交付报告中事后展示
- **降级记录**: 阶段 1 五提取器因并发配额限制由 5 路并行降为 2 路并行+1 串行，产出格式不变；阶段 1.5 验证代理在写出 verified.md 后配额超限终止，rejected/ 由主流程按其结论补齐

## 阶段状态

| 阶段 | 状态 | 产出 |
|---|---|---|
| 0 整书理解 (Adler) | ✅ 完成 | BOOK_OVERVIEW.md（骨架5论点/术语14条/批判4类/应用潜力） |
| 1 并行提取 | ✅ 完成 | candidates/：frameworks 46 · principles 91 · cases 62 · counter-examples 39 · glossary 20 |
| 1.5 三重验证 | ✅ 完成 | verified.md（合并17单元→通过13/淘汰4）；rejected/ 12 文件（45 条未录取候选全部有去向） |
| 2 RIA++ 构造 | ✅ 完成 | 13 个 `<skill-slug>/SKILL.md`（R/I/A1/A2/E/B 六段齐全，引用均 ≤150 字） |
| 3 Zettelkasten 链接 | ✅ 完成 | INDEX.md（13 skills + 13 条真实关系 + 学习顺序）+ GLOSSARY.md（20 条升格 + 术语→skill 映射） |
| 4 压力测试 | ✅ 完成 | 各 skill `test-prompts.json`（含跨 skill 混淆诱饵）+ `test-results.md`（fallback 主流程自测 100% 通过，已标注可信度限制）；安装后建议接入 darwin-skill 独立盲测 |
| 5 交付 | ✅ 完成 | DIGEST.md（约 7000 字精华长文）；产出已按书架规范发布到 GitHub `wxyqx/skill-bookshelf-CN` 的 `nintendo-experience-design/` 目录（按用户要求**不安装**到本地 skills 目录） |

## 录取的 13 个 skill（slug 定稿）

1. `intuition-design-loop` 直觉设计三步循环（假设→尝试→高兴）
2. `comprehension-first-affordance` "了解"优先与示能/能指取舍
3. `primacy-frontload-first-timers` 初始效应双律（学习前置/优先第一次的用户）
4. `fatigue-timing-management` 疲劳厌倦时机管理
5. `surprise-design-two-beliefs` 惊喜设计（误解→尝试→惊讶 + 两种坚信）
6. `taboo-theme-toolkit` 禁忌主题工具箱（10种+4问）
7. `psychological-context-redesign` 心理脉络重设计
8. `foreshadow-payoff-homecoming` 伏笔与回到起点
9. `story-design-user-growth` 故事设计（虚构是手段，用户成长是目的）
10. `gap-collection-engine` 空缺驱动（整体→空缺→收集重复→成长）
11. `risk-reward-choice-feedback` 风险回报选项与反馈闭环
12. `engineered-empathy-companion` 工程化共鸣（麻烦的同行者）
13. `stop-design-graceful-endings` 让体验停止的设计

## 用户事后确认点（无人值守模式的替代安排）

- 阶段 0 确认：BOOK_OVERVIEW.md 随最终报告展示，可要求修改骨架/批判后再拆。
- 阶段 1.5 确认：通过 13 / 淘汰 4 名单见 verified.md；若要捞回，优先候选为 rejected/03（从记忆出发）与 rejected/04（分诊规则，已转 INDEX 导航）。
