# test-results.md — 成果在组织之外（results-outside-the-organization）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "内部指标越来越好，客户投诉却越来越多"命中 description 与 verified V2 原始问题；预期（内/外定律诊断、注意力检查、质变追问）与 I/E1–E3 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "组织越来越大，整天开内部会批流程，几乎没时间见客户"命中 description 的"组织越大越高层越被内部事务困住"与 L370 判据；预期（结构性趋势 + 特殊努力与制度化安排）与 I 段第 2 点及 A1 案例 2（麦克纳马拉）一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 "internal dashboards look great but customers keep complaining. Are we too inside-out"命中 description 英文 trigger（inside-out）；预期（外部定向体检：界定外部是谁、接触占比、质变而非趋势）与 E 段一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "内部审批流程提效 20%，减少签批节点"是内部流程优化任务，B 段"纯内部职能岗位的日常优化任务：不涉及定向诊断时，用内部流程类工具即可"排除；description"把内部工作一概斥为浪费"反面使用亦已封死。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "反思自己岗位上贡献了什么、该怎样问自己"是可操作的自问句场景，A2 区分段"与 contribution-question 的区别：后者是可操作的自觉问句"明确分流；25 列表下 contribution-question 描述命中。 |
| edge-01 | 边界调用 | ✓ 通过 | "公立学校外部到底是谁：学生、家长还是纳税人"：B 段"'外部'界定不清的公共/非营利组织直接套用……必须先与用户界定口径"+E1 判停（多重委托方排优先级）与预期逐字一致（并说明书中未给可操作判据）。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 回炉记录：无。
