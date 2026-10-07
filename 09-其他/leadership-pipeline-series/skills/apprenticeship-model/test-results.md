# test-results.md — 轮岗培养模式总框架（apprenticeship-model）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “招了一批校招生、想把有潜力的培养成部门负责人，路径怎么设计”逐字命中 V2；四要件在 I/E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “关键岗位空缺只能外招、想学 GE/高露洁自己造血、该抄什么”命中 description 括注；抄的是四要件与经营嵌入。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “rotation program / high potentials not growing” 命中触发词，三要件诊断轮岗失效。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：推荐领导力培训课程——description 明确排除“只想要一次培训课程”，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：销售总监退休的继任安排命中兄弟 skill succession-five-steps / ceo-selection-process，A2 明确（培养引擎 vs 岗位决策）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：45 人公司要不要照搬五岗位 25 年——expected“原则保留、周期与形式按规模折算”，A2/B 定制主张支撑。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
