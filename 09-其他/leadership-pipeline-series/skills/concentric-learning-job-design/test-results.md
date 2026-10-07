# test-results.md — 同心圆学习与以人定岗（岗位路径设计）（concentric-learning-job-design）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “研发负责人想转管理线、下一步放哪”逐字命中 V2；步骤（目标→评估→现岗证据→下一站→载体→风险）在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “平调到大区级别不变、他觉得自己被降职”命中 description 的“平调是不是倒退”与平行调动学习设计。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “stretch / creating a role adds a layer” 命中触发词；增设层级的失败模式在 B（b4-ce15）。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：覆盖 200 人的培养体系设计命中兄弟 skill apprenticeship-model，description 明确排除“批量校招的培养体系设计”。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：劳动合同与社保手续，description 明确排除“岗位调整涉及劳动法程序时的合规判断”。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：现岗业绩中等能否先上——expected“先判现岗是否有战胜挑战证据＋风险承受力”，E 段同心圆判据支持。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
