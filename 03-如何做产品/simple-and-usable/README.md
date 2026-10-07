# 简约至上：交互式设计四策略（Simple and Usable）· 技能集

由 Giles Colborne《简约至上：交互式设计四策略》蒸馏出的一组**可被 AI Agent 调用的技能**（Skills）。

> 简单不是减少功能数，而是用户的感觉——先用主流用户的视角明确"什么才是简单"，
> 再通过删除、组织、隐藏、转移四个策略，把无法消除的复杂性放到正确的位置上。
> 本项目把这套方法论提炼成 20 个原子化技能。

---

## 来源

| | |
|---|---|
| **书名** | 简约至上：交互式设计四策略 *Simple and Usable Web, Mobile, and Interaction Design* |
| **作者** | [英] Giles Colborne（cxpartners 公司总裁，曾任英国航空可用性顾问） |
| **出版** | 英文原版 2011（New Riders / Pearson）/ 中文版 人民邮电出版社 2011（李松峰、秦绪文 译） |
| **蒸馏工具** | cangjie-skill（仓颉：把长内容蒸馏成可调用技能的流水线） |
| **蒸馏方法** | RIA-TV++（整书理解 → 并行提取 → 三重验证 → RIA++ 构造 → 链接 → 压力测试 → 交付） |

---

## 20 个技能

主题分组对应 Colborne 的骨架：明确认识（第 1–2 章）→ 四策略（第 3–7 章）→ 收尾与哲学（第 8 章）。

### 认识与立场（第 1–2 章：简化之前）

- [`pseudo-simplicity-detection`](skills/pseudo-simplicity-detection/SKILL.md) — **貌似简单排查**：用三特征识别并否决说明书/向导/卡通助手类假捷径
- [`business-case-for-simplicity`](skills/business-case-for-simplicity/SKILL.md) — **简化的商业论证**：公司方程式翻译 + 重要性×可行性强制分档
- [`simplicity-baseline`](skills/simplicity-baseline/SKILL.md) — **简单基准描述**：先成文"什么算简单"，此后一切取舍拿它当自检句
- [`field-observation`](skills/field-observation/SKILL.md) — **真实环境观察**：走出办公室，让设计"在被打断的间隙生存"
- [`mainstream-user-lens`](skills/mainstream-user-lens/SKILL.md) — **主流用户立场**：三分类+六组对照，对专家噪音视而不见
- [`control-and-emotion`](skills/control-and-emotion/SKILL.md) — **掌控感与感情需求**：连问"然后呢"挖到感情需求层再出方案
- [`extreme-usability-goals`](skills/extreme-usability-goals/SKILL.md) — **极端简单目标**：把常规目标升格为不可能达成的方向舵
- [`user-story-craft`](skills/user-story-craft/SKILL.md) — **用户故事法**：环境→角色→情节的三层结构 + 四标准自检
- [`share-the-insight`](skills/share-the-insight/SKILL.md) — **分享认识**：把认识压成判据句，不在场也能做对决定

### 四策略（第 3–7 章：简化的执行）

- [`four-strategies`](skills/four-strategies/SKILL.md) — **四策略总纲**：删除→组织→隐藏→转移的穷尽式路径与选择逻辑
- [`remove-strategy`](skills/remove-strategy/SKILL.md) — **删除策略**：举证责任反转 + 需求逆向工程 + 掌控感边界
- [`declutter`](skills/declutter/SKILL.md) — **减速带清理**：感知层减负（干扰、错误、视觉、文字）
- [`organize-strategy`](skills/organize-strategy/SKILL.md) — **组织策略**：分类标准三重判定、围绕行为组织、期望路径
- [`visual-organization`](skills/visual-organization/SKILL.md) — **视觉组织**：感知分层、色标条件、网格对齐
- [`hide-strategy`](skills/hide-strategy/SKILL.md) — **隐藏策略**：三类可隐藏判断 + 渐进/适时出现 + 不做自定义
- [`transfer-strategy`](skills/transfer-strategy/SKILL.md) — **转移策略**：人机分工表 + 平台长短板 + 信任前提
- [`open-experience`](skills/open-experience/SKILL.md) — **开放式体验**：菜刀钢琴模型，让用户自己定义成功

### 收尾与哲学（第 8 章 + 全书边界）

- [`complexity-placement`](skills/complexity-placement/SKILL.md) — **复杂性放置**：Tesler 法则 + 四问——决定谁面对消不掉的复杂性
- [`details-carry-simplicity`](skills/details-carry-simplicity/SKILL.md) — **细节支撑简单**：规模乘法给小问题定价
- [`simplicity-boundaries`](skills/simplicity-boundaries/SKILL.md) — **简单的边界**：下防删光特征，上防塞满认知

---

## 文档导航

- [INDEX.md](docs/INDEX.md) — skill 总览 + 引用图 + 推荐学习顺序
- [GLOSSARY.md](docs/GLOSSARY.md) — 共享术语词典（16 条，按作者用法校准）
- [DIGEST.md](docs/DIGEST.md) — 精华长文：不读全书看这篇
- [BOOK_OVERVIEW.md](docs/BOOK_OVERVIEW.md) — 整书理解（含作者局限批判）
- [verified.md](docs/verified.md) — 三重验证记录（97 条候选 → 20 个技能）
- [PIPELINE_STATE.md](docs/PIPELINE_STATE.md) — 流水线状态
- 每个 skill 目录内含 `SKILL.md` + `test-prompts.json`（darwin 兼容）+ `test-results.md`（独立盲测记录）
