# test-results.md — 选人不能只看一个绩效因素，要问"能否接受新理念"（promotion-due-diligence）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “三年业绩全优但要接的岗位完全不是一回事”逐字命中 V2；三必问逐条取证在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “CEO 想提老部下、理由只是业绩一直很好”命中 description 的“他业绩全优能不能升”；补证与旧交情风险在 A1。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “numbers are great but the new role is a different animal” 命中触发词。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：晋升材料做成汇报 PPT 属文书演示，无证据审查诉求，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：上任一年失败要复盘怪谁命中兄弟 skill leadership-deficit-four-causes，description 明确“事前尽调 vs 事后归因”。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：跨部门危机表现好——expected“部分通过（第一问成立，仍须补齐二三问）”，三必问结构支持。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
