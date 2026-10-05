# test-results.md — 痛苦之身觉察（pain-body-awareness）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程自测（fallback）** — 无独立 sub-agent 能力，主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判，判完对答案；混淆题用 19 个 skill 的 name+description 全量列表做选择。fallback 结果，可信度低于独立盲测。
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "突然炸了+摔门+事后后悔+不知道自己怎么了"命中 description 的"一点就炸/事后后悔"信号；预期动作（识别激活信号→注意力放身体能量→查回放/复述供能行为）与 E1/E2/E4 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | 夜里惊醒、胸口压石头=恐惧已成型为身体能量浪潮（浪潮信号优先于纯头脑万一循环，后者归 no-problem-in-now）；与 verified.md V2 novel_question 同构。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 wave of rage / replaying / pattern 命中；预期还要求不沿用书中性别化断言——B 段"性别本质主义"警示与案例 c22 历史语境标注可支撑。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 外派利弊是价值/决策问题，无反复发作的情绪实体描述；全列表下 inner-purpose-vs-outer-purpose 的 description 更匹配。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 用户明确的问题是"这算接纳吗/是不是自我安慰"——元诊断问题，fake-acceptance-alert 的 trigger（"我都放下了，可是还是难受"）直接命中；本 skill 的觉察流程不回答真伪接纳问题。 |
| edge-01 | 边界调用 | ✓ 通过 | 持续三周低落+食欲改变=需专业评估的临床症状，不进入觉察流程、至多作治疗外辅助——与 B 段医疗转介一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: should-trigger-02 与 no-problem-in-now 的 should-trigger-02（等复查结果反复想象最坏诊断）是同一大场景的两种主诉形态：带身体能量浪潮信号（夜里惊醒/胸口压石）→ 本 skill；纯"万一……怎么办"头脑循环 → 那边。区分规则已写进双方 A2，本次盲测按规则判定，两题均通过。
- 回炉记录: 无。
