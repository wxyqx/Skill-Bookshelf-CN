# test-results.md — 见解为先（opinions-first）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "双方都说自己有数据，怎么破"命中 description 与 verified V2 原始问题；预期（各方立场不同→认定事实不同；各自申明验证标准与所需事实；衡量方法列为议题）与 I/E3 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "老板说先别带观点，把事实收集齐再决策，可我们连要收集什么都不定"命中 description 的"先收集事实再决策"反教科书主张；预期（事件本身并非事实 → 见解转可证伪假设 + 先定衡量标准）与 I 段一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 "Which metric should we use... nobody agrees on the standard"命中 description 英文 trigger（which metric is right）；预期（衡量标准为核心议题、多方案并测）与 I 段第 3 点/E5 一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "查上季度营收和毛利率"是可由数据直接回答的事实查询，description"纯事实核查、可由数据直接回答的查询"逐字排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "团队里没人反对我的方案，可以直接推进吗"是异议机制问题，A2 区分段"与 dissent-as-resource 的区别：后者主动制造互相冲突的见解并给出处理纪律"明确分流；25 列表下 dissent-as-resource 描述逐字命中。 |
| edge-01 | 边界调用 | ✓ 通过 | "两边都把见解写得能验证，结果互相矛盾，听谁的"：B 段"两个都'经得起验证'的见解如何裁决，书中无程序……实践中需补充决策责任人裁定或引入外部判据"与预期（检查标准可比性 + 第三方标准/责任人裁定 + 说明书中缺口）一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 防操纵设计核对：E6 的判停标准（识别"以见解为盾"与"以数据为拖"）为 BOOK_OVERVIEW 批判节要求的补强项，本次测试中 snt-01 与 st-02 均未出现与"事实查询/挡箭牌"的边界混淆。
- 回炉记录：无。
