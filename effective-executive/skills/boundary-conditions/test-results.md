# test-results.md — 边界条件（boundary-conditions）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "先上线再迭代该不该同意，帮我定最低要求"命中 description 的"最低要求是什么"与 verified V2 原始问题；预期（写最低需要 + 必要性检验 + 临时措施永久化测试）与 E1–E3 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "去年定的区域策略前提前提还成立吗？什么情况下该抛弃"命中 description"什么时候该抛弃这项决策"与第三用途；预期（列出边界条件 + 抛弃触发器）与 E5 一致。**备注**：feedback-and-inspect 是近邻候选（"前提是否变了"），两 skill 的区分信号为"抛弃条件（本 skill）vs 前提检验机制（FAI）"，各自 description 均已声明；本场按"什么情况下抛弃"的措辞判给本 skill 并通过。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 "minimum must-haves and the boundary conditions before we commit"命中 description 的英文 trigger（boundary conditions / minimum requirements）；预期（最低必须达成清单 + 必要性检验 + 勉强可行风险）与 E2/E4 一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "办公室打印机选型，预算八百以内"是琐碎可逆选择，B 段"日常琐碎、可逆、后果极小的选择：为它写边界条件是过度工程（'行政长官不宜考虑鸡毛蒜皮之类的事情'）"逐字排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "十个小毛病要不要大改造，值不值得做决策"是"是否需要决策"门槛，description"还没决定要不要做决策（先用 decide-and-act-fully）"明示分流；25 列表下 decide-and-act-fully 描述命中。 |
| edge-01 | 边界调用 | ✓ 通过 | "各方对'方案必须满足什么'看法完全不同，谁的才算数"：B 段"边界条件是'充满风险的判断'，但书里没给裁决程序……实际使用中需要自行补充对齐机制（书面清单、责任人裁定）"与预期逐字一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 近邻边界备注：与 feedback-and-inspect 的"抛弃条件 vs 前提检验"分工、与 problem-classification 的"先定性后定规范"顺序均已写入相关 skills 节并经双向诱饵互测。
- 回炉记录：无。
