# test-results.md — 寂静与空间（silence-and-space）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程自测（fallback）** — 无独立 sub-agent 能力，主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判，判完对答案；混淆题用 19 个 skill 的 name+description 全量列表做选择。fallback 结果，可信度低于独立盲测。
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | 每天两小时地铁又挤又吵全程烦躁=description 首场景（verified.md V2 novel_question）；动作=寂静→空间轮换方案（E6 场景打包）。 |
| should-trigger-02 | 会激活 | ✓ 通过 | open office 声音没法思考、耳机堵不住=description 首场景之二；注意力从声音移到声音之下的寂静（E2），并保留降噪等环境调整建议。 |
| should-trigger-03 | 会激活 | ✓ 通过 | "安静得难受，越安静越难受"=description 反向 trigger（对"无"本身的对抗性注意）；同时确认冲突情绪是否需先处理，与 A2 区分（已成情绪浪潮→pain-body-awareness）衔接。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 会议纪要需要精确听取每个发言——B 段反场景（分注意力给字句间隙会丢信息）直接生效，应给普通速记/录音建议。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 主诉对象是思维声音（内部对象），"想学会观察念头"是 observe-the-thinker 的 trigger；本 skill 处理感官环境（外部对象），description 的 trigger 信号（太吵/过载/安静难受）均不存在。 |
| edge-01 | 边界调用 | ✓ 通过 | 判定为"不作为耳鸣干预手段：先确认已就医评估；前提下可尝试注意力调整，但明确不治疗耳鸣、以'不与耳鸣对抗'为前提"——与 E3 判停条件一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: should-trigger-01 与 waiting-state-exit 的 should-trigger-03（通勤无聊心累）是通勤场景的两个分岔，判据是主诉形态（感官对抗 vs 候场式无聊），双方 A2 已覆盖。
- 回炉记录: 无。
