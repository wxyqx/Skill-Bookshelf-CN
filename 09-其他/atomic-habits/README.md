# 掌控习惯：原子习惯与行为设计四定律

由詹姆斯·克利尔《掌控习惯》（*Atomic Habits*，2019）蒸馏出的一组**可被 AI Agent 调用的技能**（Skills）。

> 问题不在你，而在你的体系；习惯是自我提升的复利——每天进步 1%，一年后你会强 37 倍。行为改变不靠拔高目标或锤炼意志力，而靠一套围绕"提示→渴求→反应→奖励"习惯回路的体系工程：四大定律正向使用养成好习惯，反向使用戒除坏习惯。16 个技能覆盖从身份哲学与元诊断，到四定律的养成/戒除技术、承诺机制与追踪问责，再到赛道选择、难度加码与精通反思的完整习惯生命周期。

---

## 来源

| | |
|---|---|
| **书名** | 掌控习惯（Atomic Habits: An Easy & Proven Way to Build Good Habits & Break Bad Ones） |
| **作者** | 詹姆斯·克利尔（James Clear，习惯研究专家、习惯学院创始人） |
| **出版** | 北京联合出版公司 2019.7（迩东晨 译）；英文原版 2018 |
| **蒸馏工具** | cangjie-skill（仓颉：把长内容蒸馏成可调用技能的流水线） |
| **蒸馏方法** | RIA-TV++：EPUB 提取约 11.4 万字（20 章+前言+结论+附录）；原始候选 129 条 → 三重验证 19 单元通过 → 聚类 16 个 skill |
| **质量验证** | 集中盲测 106 题 100%：should_trigger 与 should_not_trigger 全绿、兄弟诱饵 39 条 0 跷跷板；1 对触发冲突跷跷板修复+干净复测 15/15；详见 [docs/TEST_RESULTS.md](docs/TEST_RESULTS.md) |

> **时效提示：本书 2019 年出版，行为科学证据持续更新，重要健康/心理场景请结合专业意见（各 skill B 段已注明）。**

---

## 16 个技能

**身份哲学**
- [`identity-based-habits`](skills/identity-based-habits/SKILL.md) — **身份导向习惯**：用三层行为改变模型把结果目标改写为身份方向（想成为哪类人→这类人会做什么），投票模型给破戒一次发"多数票豁免"。
- [`identity-flexibility`](skills/identity-flexibility/SKILL.md) — **身份弹性**：角色退场或身份过紧时，把角色型身份改写为特质型身份（"我是运动员"→"我是那种精神坚强的人"），防止自我定义固化成牢笼。

**元诊断**
- [`habit-loop-four-laws`](skills/habit-loop-four-laws/SKILL.md) — **习惯回路元诊断**：用"提示→渴求→反应→奖励"四步定位行为卡在哪一环，按诊断表（记不住→一；不想开始→二；太难→三；不想坚持→四）转介对应定律的技术 skill，只诊断不教技术。

**第一定律：让它显而易见**
- [`start-new-habit`](skills/start-new-habit/SKILL.md) — **启动新习惯**：计划链三步走——习惯记分卡觉察→执行意图"我将于[时间]在[地点]做[事]"→习惯叠加，附锚点三校验。
- [`environment-design`](skills/environment-design/SKILL.md) — **环境设计**：提示显性化、一空间一用途（含数字分区）、减阻预备，把行为交给环境而非意志力。
- [`quit-bad-habit`](skills/quit-bad-habit/SKILL.md) — **戒除坏习惯**：第一定律反用——盘点提示源→逐项移除隔离→残留通道按增阻梯度加障碍，自律者只是少暴露者。

**第二定律：让它有吸引力**
- [`temptation-bundling`](skills/temptation-bundling/SKILL.md) — **诱惑捆绑**：两段式公式把"需要做的"与"想要做的"同时性绑定（特定剧只在健身车上看），让需要的习惯成为通往渴望的入口。
- [`join-the-culture`](skills/join-the-culture/SKILL.md) — **加入群体**：用双条件筛选群体（目标行为在其中是常态＋你与成员已有共同点），让"和大家一样"本身成为执行力。
- [`craving-reframing`](skills/craving-reframing/SKILL.md) — **渴望重构**："得→想"换词改写预测即改写渴望，配激励仪式随时调用状态；反用可逐条重写坏习惯的"好处"，让它失去吸引力。

**第三定律：让它简便易行**
- [`two-minute-start`](skills/two-minute-start/SKILL.md) — **两分钟启动**：把新习惯压缩成两分钟内能物理完成的门户习惯，先标准化再优化；状态好想继续的日子也在两分钟处强制停。
- [`commitment-devices`](skills/commitment-devices/SKILL.md) — **承诺机制**：第三定律反用——承诺机制（奥德修斯合约）、一次性决策与自动化把正确行为变成默认选项；频率低到养不成习惯的重要行为直接交给自动化。

**第四定律：让它令人愉悦**
- [`reward-design`](skills/reward-design/SKILL.md) — **奖励设计**：给长期有利的行为添加即时快乐（增强法），用颠倒记账法奖励"忍住了没做"，奖励须经身份一致性校验——"奖励启动习惯，身份维持习惯"。
- [`tracking-and-accountability`](skills/tracking-and-accountability/SKILL.md) — **追踪与问责**：追踪减负三原则＋"绝不错过两次"崩溃恢复协议，自我追踪不足时升级为习惯契约与问责伙伴。

**高级战术**
- [`domain-selection`](skills/domain-selection/SKILL.md) — **赛道选择**：基因适配四问定位"做什么"——乐趣的标志不是喜欢，而是能比多数人更容易承受其痛苦；找不到优势就自创交叉领域。
- [`goldilocks-difficulty`](skills/goldilocks-difficulty/SKILL.md) — **金发姑娘难度**：给稳定运转的习惯加约 4% 难度并保留成功内核，爱上厌倦——成功的最大威胁不是失败而是倦怠。
- [`mastery-reflection`](skills/mastery-reflection/SKILL.md) — **精通反思**：诊断自动化钝化（"你只是在强化，而不是在改善"），用掌握循环＋年终三问/决策日志/诚信报告重启改进。

---

## 测试

每技能目录内含 `test-prompts.json`（should-trigger / should-not-trigger（含同书兄弟混淆诱饵）/ edge-case）与 `test-results.md`（集中盲测逐例记录）。

## docs

- [docs/BOOK_OVERVIEW.md](docs/BOOK_OVERVIEW.md) — 阶段 0 整书理解
- [docs/DIGEST.md](docs/DIGEST.md) — 面向读者的精华长文（不读全书看这篇）
- [docs/INDEX.md](docs/INDEX.md) — 技能总览、引用图与推荐学习顺序
- [docs/GLOSSARY.md](docs/GLOSSARY.md) — 共享术语词典
- [docs/TEST_RESULTS.md](docs/TEST_RESULTS.md) — 集中盲测报告（106 题，终判 100%，冲突修复复测通过）
- [docs/verified.md](docs/verified.md) — 三重验证逐条判定（19 单元＋聚类总表＋时效警示）
- [docs/stage0-chapter-notes.md](docs/stage0-chapter-notes.md) — 前言+20 章+结论+附录四组精读笔记
- [docs/candidates/](docs/candidates/) — 去重后候选池 · [docs/rejected/](docs/rejected/) — 淘汰记录 · [docs/PIPELINE_STATE.md](docs/PIPELINE_STATE.md) — 流水线状态
