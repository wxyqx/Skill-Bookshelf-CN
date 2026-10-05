# test-results.md — 部门总监：四项技能与两年期杠杆机制（managing-managers-role）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “部门总监觉得在打杂、天天救火、没时间做预算与长期计划”逐字命中 V2；四项技能＋提问句式在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “一线经理被架空、员工越过他们找总监”命中“让一线经理对管理工作负责”与授权重建。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “推新流程遭整层中层抵抗”命中“混凝土层/不明确地带”的组织级归因。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：研发总监只关心自己那块研发命中兄弟 skill functional-manager-maturity，description 明确排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：两部门职责扯皮命中兄弟 skill role-clarity-gaps-overlaps，A2 明确（职责边界 vs 角色技能）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：100 人公司无正式总监层——expected“重命名该职能、不硬造层级”，E/A2 的层数定制支撑。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
