# test-results.md — 管理上司（manage-your-boss）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "新上司当场否掉每个方案、会上打断"命中 description 与 verified V2 原始问题；预期（四问调研 → 读者型/听者型判定 → 重排陈述顺序 → 复盘）与 E1–E5 逐条对应。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "老板技术出身，在意细节和数字，我汇报先讲愿景"命中 description 的"按其接受方式（读者型/听者型）"；预期（判定接收方式、重排顺序、不唯命是从）与 I 段第二三层一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | "上司能力一般、跟着没希望，是不是该'改造'他"是 ce13 的对治场景；预期（纠正方向、只看长处、上司不升迁下属无法上升）与 I 段前提判断及 R 段引文一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "公开反对总监拍板的目标，反对意见怎么提"是异议问题，description"向上司提反对意见（用 dissent-as-resource）"明示分流；25 列表下 dissent-as-resource 描述（制造并处理不同意见、先理解后判是非）命中。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "为客户做的数据分析报告没人看"是面向平级/客户的交付设计，description"专业产出交付（用 make-output-usable）"明示分流；25 列表下 make-output-usable 描述逐字命中。 |
| edge-01 | 边界调用 | ✓ 通过 | "上司喜欢一页纸，但风险大一页纸说不清关键假设"：E4 判停（要求与"正确的事情"冲突时不唯命是从）+ B 段"适配的是方式，不是放弃判断"覆盖预期（折中设计：摘要+完整支撑/会前对齐；形式适配不等于隐瞒风险）。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 近邻边界备注：与 make-output-usable、dissent-as-resource 的三方边界经双向诱饵互测（本 skill snt-02 / MOU snt-02 / DAR 无 snt 对应但 A2 明确）正确分流。
- 回炉记录：无。
