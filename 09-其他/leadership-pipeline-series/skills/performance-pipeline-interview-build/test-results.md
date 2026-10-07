# test-results.md — 业绩梯队建队六步骤（含名词提取与标准双栏）（performance-pipeline-interview-build）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “层级职责乱、从零建立每层该交什么业绩的标准”逐字命中 description 与 V2 场景。 |
| should-trigger-02 | 会激活 | ✓ 通过 | 英文 “build a performance pipeline / clarification interviews / job standards by level” 命中触发词。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “新战略把 KPI 与岗位描述都作废了，怎么翻译成各层该交的结果”命中“各层领导该交什么结果”；20~25 项与宁少而高在文内。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：JD 润色属单岗位文书，description 明确排除（“给单个岗位写职位说明书”转 job-essence-two-factors）。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：已有标准要做月度复盘命中兄弟 skill performance-dialogue-evidence，description 明确“建标准 vs 用标准”。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：五层无集团高管层——expected 要求本地化重分配；description/A2 的“留灵活性”与按组织定制在案。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
