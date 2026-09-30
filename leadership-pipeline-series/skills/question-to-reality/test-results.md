# test-results.md — 追问到现实（提问式领导）（question-to-reality）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “漂亮方案的当场审查”命中 description“拿到一份漂亮的方案/计划/述职报告要当场审查”；动作=固定顺序逐层下钻，吻合。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “头头是道但心里没底”逐字命中关键信号；E 段“追问到前提暴露为止”的判停标准在案。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “probe / challenge the assumptions without rewriting” 命中触发词；与“不越位替对方改方案”的教练边界一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：采购合同法律审查属专业法务，本 skill 对象是业务方案/计划，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：去工厂视察命中兄弟 skill field-visit-protocol（现场核对 vs 会议追问），由 description 与 A2 的“两个场合”区分，不激活本 skill。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：追问过度的判停——A2/B 段“对方不掌握实情、追问只会变成审问的场合”命中，expected 的“停止连环追问、转单独沟通”与之一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
