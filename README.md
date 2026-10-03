# skill-bookshelf 📚

把书籍蒸馏成 **AI Skills** 的总目录导航 —— 也是一个**单仓合集（monorepo）**。

> 每一本书通过 cangjie-skill（仓颉蒸馏流水线）的 RIA-TV++ 流程，
> 被蒸馏成一组**原子化、可被 AI Agent 在真实场景调用**的技能（skills）。
> 本仓库把所有已蒸馏的书集中放在一起——每本书一个子目录，内含该书的 `skills/` 与 `docs/`。

---

## 目录总览

**23 本书 · 425 个 skills**（最后更新：2026-10-03）

| 书名 | 作者 / 年份 | 主题 | Skills | 目录 |
|---|---|---:|---|---|
| 《心流》*Flow* | 米哈里·契克森米哈赖 · 1990 | 心流 / 注意力 / 意义 | 8 | [`flow/`](./flow/) |
| *Ready, Fire, Aim* | Michael Masterson · 2008 | 创业 / 销售 / 营销 | 11 | [`ready-fire-aim/`](./ready-fire-aim/) |
| 《人性的弱点》 | 戴尔·卡耐基 · 1936 | 人际关系 / 说服 | 8 | [`how-to-win-friends/`](./how-to-win-friends/) |
| 《洛克菲勒留给儿子的38封信》 | 约翰·D·洛克菲勒 · 19 世纪末–20 世纪初 | 商业哲学 / 领导 / 行动 | 15 | [`rockefeller-38-letters/`](./rockefeller-38-letters/) |
| 《刻意练习》*PEAK* | 艾利克森、普尔 · 2016 | 学习 / 技能精进 | 8 | [`peak-deliberate-practice/`](./peak-deliberate-practice/) |
| 《穷查理宝典》*Poor Charlie's Almanack* | 查理·芒格 · 2021 | 决策 / 思维模型 | 12 | [`poor-charlies-almanack/`](./poor-charlies-almanack/) |
| 《经济学原理（微观分册）》 | 曼昆 · 2020 | 经济学 / 决策分析 | 6 | [`mankiw-microeconomics/`](./mankiw-microeconomics/) |
| 《富爸爸穷爸爸系列》*Rich Dad Poor Dad* | 罗伯特·T·清崎 · 2021 | 财商 / 投资 / 创业 | 18 | [`rich-dad-poor-dad-series/`](./rich-dad-poor-dad-series/) |
| 《思考，快与慢》*Thinking, Fast and Slow* | 卡尼曼 · 2025 | 认知偏差 / 判断决策 | 28 | [`thinking-fast-and-slow/`](./thinking-fast-and-slow/) |
| 《权力的48条法则》*The 48 Laws of Power* | 罗伯特·格林 · 1998 | 权力 / 策略 / 人际 | 15 | [`power-48-laws/`](./power-48-laws/) |
| 《稀缺》*Scarcity* | 穆来纳森、沙菲尔 · 2022 | 稀缺 / 带宽 / 决策 | 7 | [`scarcity/`](./scarcity/) |
| 《影响力》*Influence* | 罗伯特·西奥迪尼 · 2016 | 说服 / 心理 / 防御 | 9 | [`influence-cialdini/`](./influence-cialdini/) |
| 《当下的力量（白金版）》*The Power of Now* | 埃克哈特·托利 · 1997 | 临在 / 当下 / 心灵成长 | 19 | [`power-of-now/`](./power-of-now/) |
| 《高效能人士的七个习惯（30周年纪念版）》*The 7 Habits of Highly Effective People* | 史蒂芬·柯维 · 1989 | 个人管理 / 领导力 / 思维方式 | 29 | [`seven-habits/`](./seven-habits/) |
| 《精益创业 2.0》*The Startup Way* | 埃里克·莱斯 · 2017 | 企业创新 / 精益方法 / 组织变革 | 36 | [`lean-startup-2/`](./lean-startup-2/) |
| 《领导梯队建设系列（共5册）》 | 拉姆·查兰 等 · 2001–2016 | 领导梯队 / 执行 / 人才培养 | 59 | [`leadership-pipeline-series/`](./leadership-pipeline-series/) |
| 《卓有成效的管理者（中英文双语珍藏版）》*The Effective Executive* | 彼得·德鲁克 · 1966 | 有效性 / 时间管理 / 决策 | 25 | [`effective-executive/`](./effective-executive/) |
| 《任天堂的体验设计——创造不知不觉打动人心的体验》*任天堂の体験設計* | 玉树真一郎 · 2021 | 体验设计 / 打动人心 / 游戏化 | 13 | [`nintendo-experience-design/`](./nintendo-experience-design/) |
| 《上瘾》*Hooked* | 尼尔·埃亚尔、瑞安·胡佛 · 2014 | 产品设计 / 习惯养成 / 增长 | 21 | [`hooked/`](./hooked/) |
| 《启示录：打造用户喜爱的产品》*INSPIRED* | Marty Cagan · 2008 | 产品管理 / 产品探索 / 用户体验 | 18 | [`inspired/`](./inspired/) |
| 《重新定义公司：谷歌是如何运营的》*How Google Works* | 埃里克·施密特、乔纳森·罗森伯格 · 2015 | 企业管理 / 赋能 / 创意精英 | 18 | [`how-google-works/`](./how-google-works/) |
| 《学会提问（原书第10版）》*Asking the Right Questions* | 尼尔·布朗、斯图尔特·基利 · 2012 | 批判性思维 / 论证审查 / 提问 | 22 | [`asking-the-right-questions/`](./asking-the-right-questions/) |
| 《简约至上：交互式设计四策略》*Simple and Usable* | Giles Colborne · 2011 | 交互设计 / 简化 / 用户体验 | 20 | [`simple-and-usable/`](./simple-and-usable/) |

---

## 逐本详情

### 1. 《心流：最优体验心理学》 — *Flow: The Psychology of Optimal Experience* · [`flow/`](./flow/)

- **作者**：米哈里·契克森米哈赖（Mihaly Csikszentmihalyi）· 1990
- **一句话**：幸福不能直接追求——它是你全身心投入一件有挑战性的活动时，作为副产品自然涌现的最优体验。
- **Skills**：`flow-channel-trigger` · `pleasure-vs-enjoyment` · `flow-activity-designer` · `attention-audit` · `adversity-converter` · `life-theme-builder` · `meaning-spiral-assessor` · `action-reflection-balance`

### 2. *Ready, Fire, Aim* · [`ready-fire-aim/`](./ready-fire-aim/)

- **作者**：Michael Masterson · 2008
- **一句话**：创业先开枪再瞄准——用快速试错替代"准备完美再开始"的瘫痪，覆盖从获客、定价、销售到组织诊断的一整套增长方法。
- **Skills**：`ready-fire-aim` · `allowable-acquisition-cost` · `bottleneck-diagnosis` · `four-stages-of-growth` · `free-market-management` · `front-end-back-end-marketing` · `incremental-degradation` · `marketing-four-legged-stool` · `optimum-selling-strategy` · `tipping-point-innovation` · `unique-selling-proposition`

### 3. 《人性的弱点》 — *How to Win Friends and Influence People* · [`how-to-win-friends/`](./how-to-win-friends/)

- **作者**：戴尔·卡耐基（Dale Carnegie）· 1936
- **一句话**：人是被「重要感」驱动的生物——你能让别人感到自己重要，就能赢得合作；你打击别人的自尊，就永远树敌。
- **Skills**：`listening-as-persuasion` · `bait-the-fish-thinking` · `argument-avoidance` · `yes-ladder-socratic` · `preemptive-self-criticism` · `face-saving-feedback` · `micro-progress-praise` · `reputation-anchoring`

### 4. 《洛克菲勒留给儿子的38封信》 · [`rockefeller-38-letters/`](./rockefeller-38-letters/)

- **作者**：约翰·D·洛克菲勒（John D. Rockefeller）· 原信写于 19 世纪末至 20 世纪初
- **一句话**：一个白手起家者如何通过态度、行动、谋略、合作与责任，持续创造财富并掌控命运的完整心智体系。
- **Skills**：`attitude-reframe` · `deliberate-hardship` · `impulse-control` · `low-profile-wisdom` · `no-excuse-action` · `action-first` · `time-money-planning` · `planned-luck` · `calculated-risk` · `negotiation-preparation` · `competitive-weakness-strike` · `purpose-driven-leadership` · `no-blame-leadership` · `strength-based-management` · `employees-first`

### 5. 《刻意练习：如何从新手到大师》 — *PEAK* · [`peak-deliberate-practice/`](./peak-deliberate-practice/)

- **作者**：安德斯·艾利克森（Anders Ericsson）、罗伯特·普尔（Robert Pool）· 2016
- **一句话**：杰出表现并非依赖天生才华，而是通过走出舒适区、获得即时反馈、持续构建高质量心理表征的刻意练习被系统地塑造出来。
- **Skills**：`build-mental-representation` · `design-deliberate-practice-plan` · `self-practice-3f-method` · `sustain-long-term-motivation` · `break-through-plateau` · `identify-true-experts` · `workplace-deliberate-practice` · `deliberate-practice-in-teaching`

### 6. 《穷查理宝典》 — *Poor Charlie's Almanack* · [`poor-charlies-almanack/`](./poor-charlies-almanack/)

- **作者**：查理·芒格（Charles T. Munger）/ 编：彼得·考夫曼 · 2021
- **一句话**：通过跨学科的重要思维模型、诚实面对自身局限、在能力圈内保持纪律与耐心，从而少犯愚蠢的错误并抓住少数关键机会。
- **Skills**：`circle-of-competence` · `multi-disciplinary-thinking` · `two-track-analysis` · `psychology-of-misjudgment` · `inversion-thinking` · `stop-doing-list` · `checklist-method` · `opportunity-cost` · `margin-of-safety` · `patience-and-action` · `lollapalooza-effect` · `destroy-favorite-idea`

### 7. 《经济学原理（微观分册）》 — *Principles of Economics: Microeconomics* · [`mankiw-microeconomics/`](./mankiw-microeconomics/)

- **作者**：N. Gregory Mankiw（曼昆）· 2020
- **一句话**：把经济学的基础思维工具——权衡取舍、机会成本、边际分析、供需均衡、市场效率与失灵——提炼成可调用的决策分析框架。
- **Skills**：`econ-ten-principles` · `comparative-advantage` · `supply-demand-analysis` · `welfare-cost-benefit` · `market-failure-diagnosis` · `market-structure-analysis`

### 8. 《富爸爸穷爸爸系列》 — *Rich Dad Poor Dad* · [`rich-dad-poor-dad-series/`](./rich-dad-poor-dad-series/)

- **作者**：罗伯特·T·清崎（Robert T. Kiyosaki）· 2021 套装（1997–2020）
- **一句话**：通过转变金钱观、持续买入「能把钱放进口袋的资产」、从 E/S 象限迁往 B/I 象限，普通人可以跳出「为钱工作」的老鼠赛跑，实现不依赖工资的财务自由。
- **Skills**：`asset-liability-filter` · `cashflow-quadrant` · `rat-race-detector` · `pay-yourself-first` · `mind-your-own-business` · `good-debt-bad-debt` · `five-financial-iqs` · `opm-opt-leverage` · `put-money-to-work` · `four-pillars-investing` · `real-estate-cashflow` · `bi-triangle` · `startup-ten-lessons` · `sales-dogs` · `code-of-honor` · `retirement-ark` · `second-chance` · `kids-financial-iq`

### 9. 《思考，快与慢》 — *Thinking, Fast and Slow* · [`thinking-fast-and-slow/`](./thinking-fast-and-slow/)

- **作者**：丹尼尔·卡尼曼（Daniel Kahneman）· 中信 2025（原书 2011）
- **一句话**：判断与选择由爱编故事的快速直觉（系统1）主导，负责怀疑与统计的慢思考（系统2）天性懒惰，因此错误是系统性、可预测的——本书提供诊断词汇与程序性纠偏工具。
- **Skills**：`substitution-check` · `wysiati-check` · `base-rate-first` · `availability-check` · `scenario-scrutiny` · `rare-events-check` · `anti-anchoring` · `high-stakes-slow-thinking` · `small-sample-rules` · `regression-to-mean` · `outside-view` · `four-step-prediction` · `interval-calibration` · `expert-intuition-precheck` · `formula-over-intuition` · `premortem` · `bias-proof-review` · `frame-check` · `fourfold-risk-locator` · `wide-frame-trader` · `risk-policy` · `zero-base-rethink` · `two-selves-check` · `peak-end-design` · `focusing-illusion` · `dual-ledger` · `independent-judgment` · `decision-factory`

### 10. 《权力的48条法则》 — *The 48 Laws of Power* · [`power-48-laws/`](./power-48-laws/)

- **作者**：罗伯特·格林（Robert Greene）· 1998
- **一句话**：权力是一场文明化的战争——你必须学会用迂回、隐蔽、耐心的手段操控人心与局势，而非依赖暴力或直白的力量对抗。
- **Skills**：`indirect-approach` · `emotion-mastery` · `conceal-intent` · `silence-power` · `reputation-strategy` · `enemy-to-ally` · `manage-superior` · `result-judgment` · `patience-shield` · `people-reading` · `strategic-surrender` · `detect-deception` · `command-attention` · `selective-honesty` · `cost-assessment`

### 11. 《稀缺：我们是如何陷入贫穷与忙碌的》 — *Scarcity* · [`scarcity/`](./scarcity/)

- **作者**：塞德希尔·穆来纳森（Sendhil Mullainathan）、埃尔德·沙菲尔（Eldar Shafir）· 2022（原版约 2013）
- **一句话**：稀缺会俘获大脑，造成管窥心态与带宽负担，通过借用、杂耍等行为自我强化成难以逃脱的陷阱——应对之道不是靠意志力，而是靠设计环境与系统。
- **Skills**：`bandwidth-management` · `tunneling-decision-check` · `borrowing-vigilance-checklist` · `pull-into-tunnel` · `slack-building-strategy` · `abundance-planning` · `scarcity-trap-escape`

### 12. 《影响力：你为什么说"是"》 — *Influence: The Psychology of Persuasion* · [`influence-cialdini/`](./influence-cialdini/)

- **作者**：罗伯特·西奥迪尼（Robert B. Cialdini）· 2016（初版 1984）
- **一句话**：六大心理原理（互惠、承诺一致、社会认同、喜好、权威、短缺）如何自动触发人类的「卡嗒，哗」依从反应，以及如何识别与防御。
- **Skills**：`click-whirr` · `contrast-principle` · `reciprocity-defense` · `commitment-consistency` · `social-proof` · `liking` · `authority` · `scarcity` · `rejection-retreat`

### 13. 《当下的力量（白金版）》 — *The Power of Now* · [`power-of-now/`](./power-of-now/)

- **作者**：埃克哈特·托利（Eckhart Tolle），译者 曹植 · 1997（白金版 2009 中文版）
- **一句话**：痛苦不来自发生了什么，而来自对思维与时间的两个认同——把注意力从思维中撤回、完全接纳当下时刻（临在），痛苦之身便失去燃料；当下是你唯一拥有、也唯一能借力的东西。
- **Skills**：`observe-the-thinker` · `inner-body-connection` · `silence-and-space` · `pain-body-awareness` · `unconsciousness-levels` · `clock-time-vs-psychological-time` · `no-problem-in-now` · `pressure-here-wanting-there` · `emotion-as-truth-check` · `accept-then-act` · `two-surrender-chances` · `non-reactive-no` · `fake-acceptance-alert` · `waiting-state-exit` · `inner-purpose-vs-outer-purpose` · `no-understanding-the-past` · `present-forgiveness` · `fully-accept-your-partner` · `relationship-as-awareness-dojo`

### 14. 《高效能人士的七个习惯（30周年纪念版）》 — *The 7 Habits of Highly Effective People* · [`seven-habits/`](./seven-habits/)

- **作者**：史蒂芬·柯维（Stephen R. Covey）· 1989（本批以 30 周年纪念版为底本）
- **一句话**：高效能不是技巧的叠加，而是把普遍永恒的原则内化为习惯、由内而外（先个人领域成功、后公众领域成功）地实现「产出/产能平衡」的持续过程。
- **Skills**：`paradigm-shift-first` · `habit-knowledge-skill-desire` · `maturity-continuum` · `ppc-balance` · `influence-circle` · `stimulus-response-gap` · `proactive-language` · `make-and-keep-promises` · `two-creations` · `leadership-before-management` · `personal-mission-statement` · `life-center-diagnosis` · `funeral-exercise` · `transition-person` · `fourth-gen-time-management` · `stewardship-delegation` · `effectiveness-not-efficiency-with-people` · `emotional-bank-account` · `clarify-expectations` · `honor-the-absent` · `win-win-five-dimensions` · `six-interaction-modes` · `win-win-or-no-deal` · `no-involvement-no-commitment` · `seek-first-to-understand` · `diagnose-before-prescribe` · `synergy-third-alternative` · `affirm-potential` · `sharpen-the-saw-four-dimensions`

### 15. 《精益创业 2.0》 — *The Startup Way* · [`lean-startup-2/`](./lean-startup-2/)

- **作者**：埃里克·莱斯（Eric Ries）· 2017（中文版中信 2020）
- **一句话**：创业管理应当成为成熟企业的第二套核心管理体制——像设立财务部一样设立「创业部」，用创新核算与里程碑式拨款问责，分三个阶段完成一场可以反复进行的「二次创业」。
- **Skills**：`organizational-experiment-loop` · `leap-of-faith-assumption-audit` · `value-and-growth-hypotheses` · `good-experiment-four-traits` · `mvp-trio-and-scorecard` · `mvp-for-learning-not-scale` · `prfaq-working-backwards` · `business-model-six-questions` · `lean-for-non-startup-work` · `innovation-accounting-three-levels` · `audit-against-past-not-plan` · `bingo-card-diagnostic` · `growth-board-design` · `milestone-based-funding` · `innovation-needs-constraints` · `wield-the-sword` · `one-page-preapproval` · `one-team-success-is-enough` · `startup-team-basic-unit` · `dedicated-cross-functional-teams` · `three-tier-support-structure` · `train-the-veto-holders` · `gatekeeper-to-enabler` · `unified-entrepreneurial-theory` · `internal-change-owner` · `three-stage-transformation` · `pivot-persevere-cadence` · `leaders-two-questions` · `coach-assume-they-are-right` · `coach-not-leader-not-spy` · `reward-useful-failure` · `innovate-in-the-open` · `accountability-method-culture` · `behavior-before-tools` · `voluntary-adoption-indicator` · `localize-dont-copy`

### 16. 《领导梯队建设系列（共 5 册）》 · [`leadership-pipeline-series/`](./leadership-pipeline-series/)

- **作者**：拉姆·查兰（Ram Charan）、斯蒂芬·德罗特（Stephen Drotter）、詹姆斯·诺埃尔（James Noel）、拉里·博西迪（Larry Bossidy）等 · 2001–2016 系列（系列 5 册合并蒸馏）
- **一句话**：公司的成败很大程度上取决于能否成批量、可预见地从内部培养出各层级领导者——五册合并给出层级标准（领导梯队）、业绩契约（业绩梯队）、轮岗培养（高管路径）、商业语言（CEO说）与执行系统（执行）的完整操作系统。
- **Skills**：`leadership-pipeline-six-passages` · `three-dimension-transition` · `first-manager-three-transitions` · `manager-transition-tactics-three-steps` · `managing-managers-role` · `functional-manager-maturity` · `business-manager-complexity-triangle` · `group-executive-indirect-success` · `ceo-five-challenges` · `diagnosis-five-steps` · `role-clarity-gaps-overlaps` · `performance-gap-circle` · `succession-five-steps` · `potential-three-types` · `nine-box-actions` · `leadership-deficit-four-causes` · `corporate-function-six-relations` · `dual-track-management-technical` · `promotion-due-diligence` · `customize-not-copy` · `performance-pipeline-interview-build` · `job-essence-two-factors` · `control-three-points-immune-system` · `functional-vp-four-results` · `environment-three-variables` · `mealer-transition-six-steps` · `performance-dialogue-evidence` · `apprenticeship-model` · `concentric-learning-job-design` · `deliberate-practice-feedback-loop` · `leadership-potential-double-helix` · `ceo-selection-process` · `tolerate-failure-conditions` · `developing-talent-is-every-leaders-job` · `assessment-dual-track` · `leadership-is-work-not-honor` · `business-acumen-six-elements` · `r-m-v-return-decomposition` · `cash-net-inflow-everyones-business` · `direct-customer-contact` · `complexity-to-priorities` · `priority-focus-three-to-four` · `pe-multiple-wealth-mechanism` · `company-panorama-seven-questions` · `coaching-two-tracks` · `social-operating-mechanism` · `profitable-sustainable-growth` · `not-betting-is-betting` · `execution-system-architecture` · `question-to-reality` · `field-visit-protocol` · `culture-performance-linkage` · `talent-review-meeting-mrr` · `underperformer-tiered-handling` · `bedrock-strategy-one-pager` · `strategy-review-question-set` · `operations-plan-three-step` · `assumptions-and-contingency` · `follow-through-discipline`

### 17. 《卓有成效的管理者（中英文双语珍藏版）》 — *The Effective Executive* · [`effective-executive/`](./effective-executive/)

- **作者**：彼得·德鲁克（Peter F. Drucker），译者 许是祥 · 1966
- **一句话**：有效性不是天赋而是可以学会的习惯——知识工作者通过记录时间、聚焦贡献、发挥长处、要事优先、有效决策五项实践，把自己管理成能对组织成果负责的「管理者」，让平凡人做出不平凡的事。
- **Skills**：`effectiveness-five-habits` · `results-outside-the-organization` · `know-thy-time` · `time-diagnosis-questions` · `time-waste-institution-scan` · `consolidate-free-time` · `contribution-question` · `three-domains-of-contribution` · `make-output-usable` · `strengths-based-staffing` · `appraisal-four-questions` · `manage-your-boss` · `use-your-own-strengths` · `one-thing-at-a-time` · `abandon-yesterday` · `priority-and-posterior` · `decision-five-elements` · `problem-classification` · `boundary-conditions` · `correct-before-compromise` · `decision-to-action` · `feedback-and-inspect` · `opinions-first` · `dissent-as-resource` · `decide-and-act-fully`

### 18. 《任天堂的体验设计——创造不知不觉打动人心的体验》 — *任天堂の体験設計* · [`nintendo-experience-design/`](./nintendo-experience-design/)

- **作者**：玉树真一郎（前任天堂 Wii 策划开发） · 2021（电子工业出版社中文版，王芳译；日文原版约 2020）
- **一句话**：任何人都能创造打动人心的体验——把"用户经历体验的过程"本身当设计对象，用直觉设计让人不由自主地行动、惊喜设计让人不由自主地着迷、故事设计让人不由自主地想叙述。
- **Skills**：`intuition-design-loop` · `comprehension-first-affordance` · `primacy-frontload-first-timers` · `fatigue-timing-management` · `surprise-design-two-beliefs` · `taboo-theme-toolkit` · `story-design-user-growth` · `gap-collection-engine` · `risk-reward-choice-feedback` · `engineered-empathy-companion` · `foreshadow-payoff-homecoming` · `psychological-context-redesign` · `stop-design-graceful-endings`

### 19. 《上瘾：让用户养成使用习惯的四大产品逻辑》 — *Hooked: How to Build Habit-Forming Products* · [`hooked/`](./hooked/)

- **作者**：尼尔·埃亚尔（Nir Eyal）、瑞安·胡佛（Ryan Hoover），钟莉婷、杨晓红 译 · 2014（中文版中信出版社）
- **一句话**：习惯养成类产品的引擎是「触发→行动→多变酬赏→投入」的四阶段闭环——用户的投入沉淀为储存价值并自动加载下一次触发，外部触发逐步内化为情绪绑定；设计者必须先用操纵矩阵问「该不该」，再问「能不能」。
- **Skills**：`hook-model-four-stages` · `habit-zone-frequency-first` · `vitamin-to-painkiller` · `four-opportunity-sources` · `external-triggers-four-types` · `internal-trigger-anchoring` · `five-whys-emotional-root` · `bmat-action-diagnosis` · `three-core-motivations` · `six-simplicity-elements` · `three-variable-rewards` · `finite-infinite-variability` · `investment-changes-attitude` · `five-stored-values` · `load-next-trigger` · `investment-timing-granularity` · `habit-test-three-steps` · `manipulation-matrix` · `preserve-user-autonomy` · `protect-heavy-users` · `upgrade-not-replace`

### 20. 《启示录：打造用户喜爱的产品》 — *INSPIRED: How to Create Tech Products Customers Love* · [`inspired/`](./inspired/)

- **作者**：Marty Cagan（曾任惠普程序员、网景平台及工具部门副总裁、eBay 产品管理及设计高级副总裁） · 2008（华中科技大学出版社中文版 2011，七印部落 译）
- **一句话**：产品经理的本职是探索出**有价值的、可用的、可行的**产品——在写第一行代码之前，用高保真原型和真实用户验证这三点；因为"如果产品没有市场价值，无论开发团队多么优秀也无济于事"。
- **Skills**：`opportunity-assessment-ten-questions` · `discovery-execution-two-modes` · `product-validation-trio` · `minimal-product-definition` · `hi-fi-prototype-as-spec` · `charter-user-program` · `prototype-testing-playbook` · `user-research-limits` · `persona-driven-focus` · `irrational-user-signals` · `product-principles-priority` · `special-product-defense` · `emotion-based-demand` · `new-old-thing` · `metric-driven-improvement` · `smooth-deployment` · `rapid-response-window` · `tech-headroom-20percent`

### 21. 《重新定义公司：谷歌是如何运营的》 — *How Google Works* · [`how-google-works/`](./how-google-works/)

- **作者**：埃里克·施密特（Eric Schmidt，谷歌前 CEO）、乔纳森·罗森伯格（谷歌前产品负责人），与艾伦·伊格尔合著 · 2015（中信出版社中文版，靳婷婷译；英文原版 2014）
- **一句话**：互联网时代企业的成功之道，是聚集一群"创意精英"（smart creative）并营造让他们自由发挥的环境——**赋能而非管理**；信息、连接、计算的成本骤降让"速度定成败"，卓越产品是唯一护城河。
- **Skills**：`hippo-resistance` · `org-design-rules` · `expel-villains-protect-stars` · `technical-insight-first` · `open-as-strategy` · `focus-user-think-10x` · `hiring-quality-bar` · `talent-portrait` · `hiring-ops` · `retention-playbook` · `real-consensus` · `decision-timing-discipline` · `default-open-candor` · `resource-70-20-10` · `twenty-percent-time` · `ship-iterate-fail-well` · `innovation-chaos` · `ask-hard-questions`

### 22. 《学会提问（原书第10版）》 — *Asking the Right Questions: A Guide to Critical Thinking* · [`asking-the-right-questions/`](./asking-the-right-questions/)

- **作者**：[美] 尼尔·布朗（M. Neil Browne）、斯图尔特·基利（Stuart M. Keeley） · 2012（英文原版 10th ed.；中文版机械工业出版社 2013，吴礼敬 译）
- **一句话**：批判性思维不是"多想一下"的态度，而是一张环环相扣的关键问题清单（论题→结论→理由→歧义词→假设→谬误→证据→替代原因→数据→省略信息→备选结论）——用它逐层拆解任何想说服你的论证，同时把同一张清单对准自己的结论（强势批判性思维），否则它只会沦为护短工具。
- **Skills**：`scrutiny-worthiness-filter` · `pan-for-gold-reading` · `strong-sense-self-audit` · `critical-thinker-values` · `keep-dialogue-alive` · `wishful-feeling-check` · `critical-question-master-list` · `locate-issue-conclusion` · `identify-reasons` · `charity-before-judgment` · `ambiguity-loaded-words` · `value-assumption-mining` · `descriptive-assumption-mining` · `fallacy-three-questions` · `evidence-grade-triage` · `expert-opinion-audit` · `research-survey-audit` · `analogy-evaluation` · `rival-causes-audit` · `deceptive-data-check` · `omitted-info-probe` · `alternative-conclusions`

### 23. 《简约至上：交互式设计四策略》 — *Simple and Usable: Web, Mobile, and Interaction Design* · [`simple-and-usable/`](./simple-and-usable/)

- **作者**：[英] Giles Colborne（cxpartners 公司总裁，曾任英国航空可用性顾问） · 2011（英文原版 New Riders；中文版人民邮电出版社 2011，李松峰、秦绪文 译）
- **一句话**：简单不是减少功能数，而是用户的感觉——先用主流用户的视角明确"什么才是简单"，再通过删除、组织、隐藏、转移四个策略，把无法消除的复杂性（Tesler 法则：复杂性守恒，只能决定谁面对它）放到正确的位置上。
- **Skills**：`pseudo-simplicity-detection` · `business-case-for-simplicity` · `simplicity-baseline` · `field-observation` · `mainstream-user-lens` · `control-and-emotion` · `extreme-usability-goals` · `user-story-craft` · `share-the-insight` · `four-strategies` · `remove-strategy` · `declutter` · `organize-strategy` · `visual-organization` · `hide-strategy` · `transfer-strategy` · `open-experience` · `complexity-placement` · `details-carry-simplicity` · `simplicity-boundaries`

---

## 安装

一次性安装**所有书**的 skills，或只装某一本：

```bash
# 一次性安装全部 425 个 skills（用户级，所有项目可用）
for d in */skills; do cp -r "$d"/* ~/.claude/skills/; done

# 或只装某一本（以心流为例）
cp -r flow/skills/* ~/.claude/skills/
```

每本书的 `skills/` 里每个技能目录都包含 `SKILL.md`（+ `test-prompts.json` / `test-results.md` 测试产物）。

---

## 目录结构

```text
skill-bookshelf/
├── README.md                 # 总导航（你在这里）
├── flow/                     # 《心流》
│   ├── README.md             # 本书说明
│   ├── skills/               # 8 个可安装技能
│   └── docs/                 # 蒸馏文档（DIGEST/INDEX/GLOSSARY/…）
├── ready-fire-aim/           # *Ready, Fire, Aim*（11 skills）
├── how-to-win-friends/       # 《人性的弱点》（8 skills）
├── rockefeller-38-letters/   # 《洛克菲勒留给儿子的38封信》（15 skills）
├── peak-deliberate-practice/ # 《刻意练习》（8 skills）
├── poor-charlies-almanack/   # 《穷查理宝典》（12 skills）
├── mankiw-microeconomics/    # 《经济学原理（微观分册）》（6 skills）
├── rich-dad-poor-dad-series/ # 《富爸爸穷爸爸系列》（18 skills）
├── thinking-fast-and-slow/   # 《思考，快与慢》（28 skills）
├── power-48-laws/            # 《权力的48条法则》（15 skills）
├── scarcity/                 # 《稀缺》（7 skills）
├── influence-cialdini/       # 《影响力》（9 skills）
├── power-of-now/             # 《当下的力量（白金版）》（19 skills）
├── seven-habits/             # 《高效能人士的七个习惯》（29 skills）
├── lean-startup-2/           # 《精益创业 2.0》（36 skills）
├── leadership-pipeline-series/ # 《领导梯队建设系列》（59 skills）
├── effective-executive/      # 《卓有成效的管理者》（25 skills）
├── nintendo-experience-design/ # 《任天堂的体验设计》（13 skills）
├── hooked/                   # 《上瘾》（21 skills）
├── inspired/                 # 《启示录：打造用户喜爱的产品》（18 skills）
├── how-google-works/         # 《重新定义公司：谷歌是如何运营的》（18 skills）
├── asking-the-right-questions/ # 《学会提问（原书第10版）》（22 skills）
└── simple-and-usable/        # 《简约至上：交互式设计四策略》（20 skills）
```

---

## 如何添加一本新书

每蒸馏完成一本新书，把它作为新子目录加入这个合集，保持三步同步：

1. 把该书的蒸馏产物按 `<book-slug>/skills/` + `<book-slug>/docs/` 结构放进一个新子目录（命名约定：去掉 `-skills` 后缀的 slug）；
2. 在「目录总览」表格里加一行，并把「N 本书 · M 个 skills」的计数更新；
3. 在「逐本详情」里追加一个 `###` 小节，链接指向新子目录。

字段从该书的 `README.md` 顶部「来源」表格和 `docs/INDEX.md` 里直接取，不必重新总结。
