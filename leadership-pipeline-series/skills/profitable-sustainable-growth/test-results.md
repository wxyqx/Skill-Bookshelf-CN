# test-results.md — 赢利可持续增长原则（增长必须赢利、可持续，并伴随利润与周转率的提高）（profitable-sustainable-growth）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “all-in 出海、收入翻三倍，批不批”逐字命中 V2；四项同步检查在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “销售激励按签约金额、单子越多利润率越掉”命中“设计销售激励（按金额还是按毛利）”与错误激励反例。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “先亏几年换规模、格局定了再盈利”命中“先做大再盈利”；同时要求携带模型边界声明。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：现金断粮要收缩——description 明确排除“危机生存性收缩”并指向现金视角 skill。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：收购判断贵不贵命中兄弟 skill pe-multiple-wealth-mechanism，A2 明确（增长验收 vs 估值判断）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：公益社企——B 段“非营利需改写后再用（赢利→可持续覆盖成本）”，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
