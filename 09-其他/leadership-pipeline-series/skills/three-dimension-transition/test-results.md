# test-results.md — 阶段转型三维度：技能 / 时间 / 理念（three-dimension-transition）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “技术大牛升总监仍写 60% 代码、培训也上了行为不变”逐字命中 V2；三把尺子＋日程表硬证据在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “写一份新岗位到底要求什么变了的说明”命中三维度用于岗位转型说明与培养计划。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “口头说自己是管理者、关键项目还是自己上”命中四条证据通道（教训复盘/日程表/如何评价下属/计划立场，已核在文内）。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：系统排查整条梯队堵在哪一层命中兄弟 skill diagnosis-five-steps，description 明确排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：销售冠军转经理失败要不要换掉属人事处置——description/ 边界不产出解雇建议，expected 一致（边界判定）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：扁平组织时间被打散——B 段“时间证据在非科层组织中的适用性受限、须结合决策层级”，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
