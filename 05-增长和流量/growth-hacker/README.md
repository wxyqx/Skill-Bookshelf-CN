# 增长黑客：创业公司的用户与收入增长秘籍

由范冰《增长黑客》（电子工业出版社 2015）蒸馏出的一组**可被 AI Agent 调用的技能**（Skills）。

> 初创公司没钱买流量：先确认产品已达成 PMF——"任何增长黑客都无法挽回一个无药可救的垃圾产品"——再用数据驱动的实验沿 AARRR 漏斗（获客→激活→留存→收入→传播）逐环找出转化率最低的卡点，做低成本、可测量的增长实验，替代砸钱投放。21 个技能覆盖 PMF 验证、获客冷启动、激活与补贴、留存与度量、免费/收费决策、病毒传播、AARRR 元层诊断与增长职业道德的完整链路。

---

## 来源

| | |
|---|---|
| **书名** | 增长黑客 Growth Hacker |
| **作者** | 范冰 |
| **出版** | 电子工业出版社 2015 |
| **蒸馏工具** | cangjie-skill（仓颉：把长内容蒸馏成可调用技能的流水线） |
| **蒸馏方法** | RIA-TV++：EPUB 提取约 20.9 万字（8 章+序+后记+附录A）→ 原始候选 140 条 → 三重验证 21 单元通过 → 聚类 21 个 skill |
| **质量验证** | 集中盲测 159 题 100%：should/should_not 全绿、同书兄弟诱饵 48 条 0 跷跷板；1 处 description 边界按跷跷板法修复+干净复测 6/6、3 处边界用例双路径修正留痕（详见 [docs/TEST_RESULTS.md](docs/TEST_RESULTS.md)） |

> **时效提示：本包基于 2015 年快照**——开放平台红利、O2O 补贴环境、SEO/ASO 权重、各平台规则均已生变。各 skill 的 B 段（背景与案例）已内嵌时代警示：**只取判断逻辑层，参数层（具体渠道、阈值、玩法）请按当期平台规则与法规重查。**

---

## 21 个技能

**一、PMF 验证**
- [`demand-four-questions`](skills/demand-four-questions/SKILL.md) — **需求四问**：立项前纸面过筛单个需求的"真伪/刚性/量与肥/变现"四问，任何一问不过即出局；依据是 68~200 倍需求成本定律——全书最便宜的一道质量关。
- [`pmf-gate`](skills/pmf-gate/SKILL.md) — **PMF 决策门**：推广/扩招/烧钱扩张前无"留存曲线走平 + 自发口碑 + 复购"硬证据则三禁止。
- [`mvp-validator`](skills/mvp-validator/SKILL.md) — **MVP 验证器**：按验证目标选形态（视频/假门/手工服务/公众号），第一天就带反馈/公告/升级三大必备模块；MVP ≠ 便宜难看残破。
- [`actions-over-words`](skills/actions-over-words/SKILL.md) — **行为重于言辞**：解读调研时用"行为 > 口头"校准可信度，付费意愿是意见权重的最佳标尺。

**二、获客**
- [`seed-user-selection`](skills/seed-user-selection/SKILL.md) — **种子用户筛选**：贵精不贵多，用筛选机制定调产品氛围，用数据日志排除"产品蝗虫"。
- [`do-things-that-dont-scale`](skills/do-things-that-dont-scale/SKILL.md) — **不可扩展的事**：零预算冷启动的人工补课选型（人肉内容/一对一陪聊/手工供给），规模化后制度化退出。
- [`content-marketing-engine`](skills/content-marketing-engine/SKILL.md) — **内容营销引擎**：先定位内容三作用，再建选题—生产—分发—复盘的固定循环，而非赌单篇爆款。

**三、激活**
- [`ab-testing-protocol`](skills/ab-testing-protocol/SKILL.md) — **A/B 测试规范**：双方案并行/单变量/预设判优三铁律，"多数测试注定失败"的预期管理与微优化陷阱边界。
- [`activation-aha-magic-number`](skills/activation-aha-magic-number/SKILL.md) — **激活啊哈时刻与魔法数字**：从留存数据反推关键行为 → 注册默认引导 → A/B 校准魔法数字。
- [`subsidy-ladder`](skills/subsidy-ladder/SKILL.md) — **补贴阶梯**：返利 → 限期券 → 现金 → 红包的形态升级，并预演"停止补贴后的留存曲线"。
- [`gamification-boundary`](skills/gamification-boundary/SKILL.md) — **游戏化边界**：PBL 设计与"只能锦上添花，不能雪中送炭"红线判据，预设新鲜感衰减后的退役。

**四、留存**
- [`retention-diagnosis`](skills/retention-diagnosis/SKILL.md) — **留存诊断**：四层诊断（净增长 → 三口径基准 → 流失五分类 → 性能硬伤有损服务止血）；留存有硬伤时拉新是给漏水的桶灌水。
- [`winback-mechanisms`](skills/winback-mechanisms/SKILL.md) — **流失召回**：通道 × 内容选型矩阵；唤醒是补救手段而非留存的替代品。
- [`growth-metrics-system`](skills/growth-metrics-system/SKILL.md) — **增长指标体系**：一个 North Star + 两条分析纪律 + 带口径陷阱注解的 26 项指标字典，排除虚荣指标。

**五、收入**
- [`freemium-decision`](skills/freemium-decision/SKILL.md) — **免费/收费决策**：先过三前提，撑不起时走"静默砍免费版试验"（悄悄删 → A/B 验证 → 公开切换）。
- [`turn-penalty-into-reward`](skills/turn-penalty-into-reward/SKILL.md) — **化惩罚为奖励**：越轨用户（盗版/薅漏洞）转化三原则——绝不责备、给予补偿、提供便利，堵不如疏。

**六、传播**
- [`viral-k-factor`](skills/viral-k-factor/SKILL.md) — **病毒 K 因子**：K=感染率×转化率与病毒循环周期双指标定位瓶颈，八种心理触发器匹配分享动作。
- [`external-viral-loop`](skills/external-viral-loop/SKILL.md) — **外部病毒循环**：主产品外病毒活动（H5 小游戏/测试、Bug 营销）三大考验 + 六要点 + 付出感设计与封杀风险评估。
- [`moment-marketing`](skills/moment-marketing/SKILL.md) — **时机营销**：只在热点爆发期把推广融入用户语境，为可预测节点在研发阶段预埋卖点。

**七、AARRR 元层**
- [`aarrr-funnel-diagnosis`](skills/aarrr-funnel-diagnosis/SKILL.md) — **AARRR 漏斗诊断**：用指标链找转化率最低的卡点环节，只对该环节设计实验并转入对应专项 skill。

**八、职业道德**
- [`growth-ethics-redlines`](skills/growth-ethics-redlines/SKILL.md) — **增长道德红线**：换位思考/最小授权最大知情/契约精神三道守门闸，任何一闸不过即砍。

---

## 测试

每技能目录内含 `test-prompts.json`（should-trigger / should-not-trigger（含同书兄弟混淆诱饵）/ edge-case）与 `test-results.md`（集中盲测逐例记录，判停/双归属/转介差异已加注脚）。

## docs

- [docs/BOOK_OVERVIEW.md](docs/BOOK_OVERVIEW.md) — 阶段 0 整书理解
- [docs/DIGEST.md](docs/DIGEST.md) — 面向读者的精华长文（不读全书看这篇）
- [docs/INDEX.md](docs/INDEX.md) — 技能总览、引用图与推荐学习顺序
- [docs/GLOSSARY.md](docs/GLOSSARY.md) — 共享术语词典
- [docs/TEST_RESULTS.md](docs/TEST_RESULTS.md) — 集中盲测报告（159 题 100% 通过）
- [docs/verified.md](docs/verified.md) — 三重验证逐条判定
- [docs/stage0-chapter-notes.md](docs/stage0-chapter-notes.md) — 序+8 章+后记/附录A 四组精读笔记
- [docs/candidates/](docs/candidates/) — 去重后候选池 · [docs/rejected/](docs/rejected/) — 淘汰记录 · [docs/PIPELINE_STATE.md](docs/PIPELINE_STATE.md) — 流水线状态
