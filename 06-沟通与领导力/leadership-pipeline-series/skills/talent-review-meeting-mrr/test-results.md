# test-results.md — 人才评估会议机制（MRR）（talent-review-meeting-mrr）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “盘点做完没人看、没人动”逐字命中 description；MRR 要件（会前重写、会中举证、会后信件）在 I/E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “评价都是『表现不错』这种话”命中本 skill 的证据纪律（组织多人开诚布公收集行为证据，已核在文内）；结论与 expected 一致（注：与 succession-five-steps 存在语境重叠，因本 skill 以评价证据缺陷为核心信号而判激活）。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “honest evidence instead of impressions” 命中核心差异；会前/会中/会后三段程序在 E。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：满意度问卷属调研采集工具，description 与 B 段明确批评问卷式诊断且本机制是人才决策会议，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：老员工处置命中兄弟 skill underperformer-tiered-handling（A2“会上判断→处置落地”分工），不激活本 skill。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：40 人公司轻量化——A2/B“两天会期是大公司原型，要件保留、规模可轻量”，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
