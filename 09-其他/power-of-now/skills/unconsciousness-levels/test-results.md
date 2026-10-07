# test-results.md — 无意识分层与挑战测试（unconsciousness-levels）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程自测（fallback）** — 无独立 sub-agent 能力，主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判，判完对答案；混淆题用 19 个 skill 的 name+description 全量列表做选择。fallback 结果，可信度低于独立盲测。
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "冥想半年怎么还是炸了/是不是白练了"=A2 场景 1 原文；预期动作（独处的平静不作数→转为基线数据→约定恢复时长复测；情绪本身移交 pain-body-awareness）与 E3/E4 判停一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "真进步还是自我感觉良好，有没有办法验证"逐字命中 description trigger；两级刻度+挑战测试+恢复时长指标的自测方案即 E1-E5。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 一停下刷手机就发慌必须填满=麻醉剂式回避（A2 场景 4 原文、ce11 信号）；预期"不给出停用建议、引导觉察、必要时建议专业帮助"与 E6 警示条款及 B 段一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 评估对象是他人——B 段"只用于自测、给他人打分违背原意"反场景生效。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 用户此刻需要的是处理已激活的情绪能量（胸口那团火），pain-body-awareness 优先；本 skill 的测量请求（评估进步/解释波动）在 prompt 中不存在。 |
| edge-01 | 边界调用 | ✓ 通过 | 判定为"不启动对他人的测量；可借框架自察'我为什么想改造领导'（转向自我观察），对方主动求助再另议"——与预期激活方式一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 无特殊边界；should-not-trigger-01 与 edge-01 是同一硬边界（自测工具不用于他人）的两种提问形态，判定一致。
- 回炉记录: 无。
