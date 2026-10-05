# test-results.md — 反面意见（dissent-as-resource）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "团队里没人反对我的方案，可以直接推进吗"命中 description 与 verified V2 原始问题；预期（一致当警号、俘虏风险自查、制造异议、要求另一方案成型）与 E1–E3 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "投决会开成走过场，每次一致通过"命中 description 与 A2 第 5 条（评审流程化走过场）；预期（制造异议具体做法 + 先理解后判是非）与 E2/E4 一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 "Should I still get a devil's advocate"命中 description 英文 trigger（devil's advocate）；预期（一致往往是没人思考或不敢说话 + 制造反面意见与备好替代方案）与 I 段一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "生产线突然停了，先别讨论，赶紧告诉我谁去处理"是危机处置现场，description"需要执行纪律的危机现场"与 B 段"先行动，事后复盘"双重排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "双方都说自己有数据，谁也不服谁"是见解与标准之争，A2 区分段"与 opinions-first 的区别：后者处理见解与事实/标准的关系……先有后者确立的规则"明确分流；25 列表下 opinions-first 描述逐字命中。 |
| edge-01 | 边界调用 | ✓ 通过 | "提反对意见的人上次被穿小鞋，现在谁都不肯说话，还怎么制造异议"：B 段"人身攻击、恶意拆台、派系斗争已明面化的场合……必须先有防操纵判停与主持规则"+E1 判停"若组织存在明确的人身攻击、恶意拆台或威胁信号，先跳到步骤 5 的防操纵判停"覆盖预期（外部/匿名渠道、决策者先示弱、不追责规则、书中无保护机制、文化未改善前不强推）。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 防操纵边界核对：BOOK_OVERVIEW 强制要求"异议机制防操纵"已写入 B 段并在 E5 补判停；本次 snt-01（危机）与 edge-01（政治化）两个高风险场景均按边界正确处理。
- 回炉记录：无。
