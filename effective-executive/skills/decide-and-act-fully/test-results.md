# test-results.md — 是否需要决策与做全（decide-and-act-fully）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "公司流程十个小毛病，要不要启动一次大改造"命中 description 与 verified V2 原始问题；预期（逐个测试"保持现状的后果"→ 小的不做；其余按两项原则收尾）与 E1–E3 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "方案得失都清楚，还在说再研究研究，算不算拖延"命中 description"再研究研究"trigger 与 ce34；预期（两问检验 + 拍板时限 + 略事犹豫量级）与 I 段后端一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 "Do we really need a decision here, or should we just do half of it and see"命中 description 英文 trigger（do we really need a decision / go big or not at all）；预期（过门槛 + 半截行动不符合边界条件）与 I 段两端一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "已经决定换系统，帮着理行动步骤和责任人"是已定决策的落地，description"已定决策的行动设计（用 decision-to-action）"明示分流；25 列表下 decision-to-action 描述逐字命中。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "三个项目全延期，先砍哪个先救哪个"是多线并行问题，description 未列但 A2 区分（"本 skill 管一项决策自身是否完整，不管注意力的集中"）与 25 列表下 one-thing-at-a-time 描述命中；本 skill 不激活。 |
| edge-01 | 边界调用 | ✓ 通过 | "判断必须做，但拍板权限不在我，领导一直拖"：B 段"缺少决策权限的场合……其可执行部分是把两端判据写成建议提交决策者"与预期（书面建议 + 拍板时限说明 + 说明书中无授权不足路径）一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 通用"决策技巧"边界核对（用户重点提醒项）：本 skill 的 snt-01/02 均按"决策四要素链条的下游/上游"正确分流（行动设计→DTA；并行取舍→OTAAT），无泛决策请求被误接。
- 回炉记录：无。
