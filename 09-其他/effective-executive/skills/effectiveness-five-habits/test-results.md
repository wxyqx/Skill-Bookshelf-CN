# test-results.md — 有效性五项习惯（effectiveness-five-habits）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "每天都很忙，但总觉得没做出什么成果……从整体上看看该从哪儿查起"直接命中 description 的整体诊断与"忙而无果"信号；预期动作（先立"有效性是习惯不是天赋"、按五习惯顺序给路径、指出第一个动作）与 R/I/E 段一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | 英文提问直指 "Drucker's five habits of effectiveness"，命中 description 的英文 trigger 与总纲定位；预期（英文列五项 + 从时间记录入手）与 I 段顺序一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | "有效性自检表，覆盖时间、贡献、用人、优先次序和决策"是 description 明示的自检清单场景；A2 第 3 条（组织/自我审计清单）与 E 段五面检查对应，预期输出含"待采集"标注与数据前置说明。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 四象限排待办是通用生产力工具操作，description"不适用于纯工具操作"直接排除；全 25 列表下也无任何 skill 应接（priority-and-posterior 的 B 段明确把四象限列为"排序分析工具"而非本方法的适用对象）。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 用户只要"第一步记录时间"，description"时间记录用 know-thy-time"明示分流；25 列表下 know-thy-time 的英文 trigger（time log / 时间审计）逐字命中，判给兄弟 skill 无歧义。 |
| edge-01 | 边界调用 | ✓ 通过 | 一小时集体复盘：可激活总纲提供检查清单，但 E3 判停"不要五项平均用力"要求裁剪（挑一项深入 + 会后各自采集），与预期边界理由一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 跨 skill 混淆核对：snt-01（四象限）与 snt-02（记录时间）是两条最典型的混淆诱饵，前者靠"工具操作"排除、后者靠"单点技巧分流"排除，均无歧义。
- 回炉记录：无。
