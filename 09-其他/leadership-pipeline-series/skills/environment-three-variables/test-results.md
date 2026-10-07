# test-results.md — 大环境（土地）分析三变量（environment-three-variables）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “新任 CEO 先换人还是先改环境”逐字命中 V2；土地—种子—农民比喻与三变量在 I/E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “换两任总裁、请顾问、做培训还是老样子”命中“换了人还是老样子”与运营模式判断。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “数字化转型员工不敢说自己不会、不敢提问”命中“员工不敢承认不会”与知晓者文化。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：重建各层业绩标准命中兄弟 skill performance-pipeline-interview-build，A2“种子与土地”分工明确。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：团建活动策划，description 明确排除“团建活动策划”。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：60 人创业公司——A2/B 简化路径（收敛为文化取向＋决策方式）与 expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
