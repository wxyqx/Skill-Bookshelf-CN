# test-results.md — 数字导向的绩效考核不能替代领导力评估（评估双轨）（assessment-dual-track）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “销售冠军数字翻倍是不是该直接提拔”命中 description“该不该提拔业绩好的人”；两轨拆开＋追因提问在 E（注：与 leadership-potential-double-helix 的“业绩最好的该不该提拔”存在语境重叠，本条以“数字能否说明能力”的角度命中本 skill 的追因纪律）。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “一套表既决定奖金又决定谁该培养”逐字命中 description 的“年终考核和领导力评估要不要分开”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “numbers were great but the whole market was up” 命中“是不是市场好他才达标”与追因示范。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：毛利掉 5 个点做业务复盘——description 明确排除“纯业务数据复盘”，对象是业务不是人。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：反馈给了但行为没变命中兄弟 skill deliberate-practice-feedback-loop，A2 明确（组织级评估制度 vs 一对一反馈闭环）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：80 人公司一次年会——expected“证据、结论与用途必须分开，形式可合并为两个议程段落”，两轨分离原则支撑。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
