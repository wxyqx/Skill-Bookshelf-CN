# test-results.md — 与内在身体联结（inner-body-connection）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程自测（fallback）** — 无独立 sub-agent 能力，主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判，判完对答案；混淆题用 19 个 skill 的 name+description 全量列表做选择。fallback 结果，可信度低于独立盲测。
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "失眠，脑子停不下来，越告诉自己别想了反而越清醒"逐字命中 description 首个 trigger；区分规则（无重播具体内容→非 observe-the-thinker 的反刍）支持本 skill；动作=不搏斗、注意力进身体能量场（E5 失眠应用）。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "一被当众否定就血冲脑门，要临场方法"=挑战来临头几秒立即回体内的触发场景（p20 并入规则）；E3 挑战挂钩对应。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 in my head / shoulders tense 命中"活 fully 在头脑里+长期躯体紧绷"场景；基础带练+日常挂载点即 E1/E4。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 右下腹隐痛=不明躯体症状，必须先建议就医排查；B 段医疗边界（胸痛/持续头痛/麻木必须就医，练习不替代检查）生效。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 已成型的情绪浪潮（熟悉的委屈压不住、胸口堵一晚）需要 pain-body-awareness 的完整觉察流程；本 skill 是一般性扎根，双方 A2 分界（成型情绪→那边）明确。 |
| edge-01 | 边界调用 | ✓ 通过 | 判定为"按书中机制这是被压抑情绪浮出水面，属可解释现象：先允许其存在并观察（转 pain-body-awareness 处理）；强烈到失控或反复出现则建议专业支持，不硬扛继续深入"——与 E2 判停 A 一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: should-trigger-01 与 observe-the-thinker 的 should-trigger-01 为近邻场景，区分规则已在阶段 3 定稿写入双方 A2（内容反刍 vs 清醒状态/躯体紧绷），判定无冲突。
- 回炉记录: 无。
