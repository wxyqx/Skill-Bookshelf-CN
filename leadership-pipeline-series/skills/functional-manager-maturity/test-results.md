# test-results.md — 职能主管：领导力成熟度与竞争优势使命（functional-manager-maturity）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “技专家升研发总监、怕成大号工程师”逐字命中 V2；成熟度三视角在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “HR 总监专业扎实但业务线说帮不上忙”命中“专业孤岛/对专业忠诚”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “聪明年轻人两年到总监、要不要放到事业部副总”命中“不急于任命”警告；并附反歧视提示（B 段）。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：部门总监被 12 个一线经理排队请示命中兄弟 skill managing-managers-role，description 明确排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：接手新事业部想降价砍人命中兄弟 skill business-manager-complexity-triangle，description 明确排除。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：单一业务公司双肩挑——A2 一线观察的岗位界定（L10640–L10644）支撑，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
