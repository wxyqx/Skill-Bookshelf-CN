# test-results.md — 文化变革的绩效联结框架（culture-performance-linkage）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “宣讲半年没人改变行为”逐字命中 description；动作=目标—条件—奖励—教练/处置四步查断点。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “价值观挂墙上、奖励还是大锅饭”命中奖励环节硬约束（行为与回报脱钩）。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “culture change isn't landing / slogans but no behavior change” 命中触发词；顺序追问在 A2。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：企业文化节宣传稿属活动策划，description 排除（“活动策划”），不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：“整体诊断执行体系哪里断了”近逐字命中兄弟 skill execution-system-architecture 的三流程触发语；本 skill 面向文化—行为工程，不激活。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：问卷式文化诊断纠偏——B 段“问卷报告未触及行为、起点应是管理层自己”命中，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
