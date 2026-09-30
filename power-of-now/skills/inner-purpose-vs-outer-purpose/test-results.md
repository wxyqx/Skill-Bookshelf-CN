# test-results.md — 内在目的 vs 外在目的（inner-purpose-vs-outer-purpose）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程自测（fallback）** — 无独立 sub-agent 能力，主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判，判完对答案；混淆题用 19 个 skill 的 name+description 全量列表做选择。fallback 结果，可信度低于独立盲测。
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | 外派抉择+两边都有道理=A2 场景 1 / verified.md V2 novel_question；预期动作（外在轴两选项都是游戏、权重转到意识质量、解除赌注）与 E1/E3 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "考上编制高兴一个月现在空虚/我图什么"=description"得到了却不快乐/空心"直接命中；自检问句+改 how 即 E4。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 chasing goals / empty / waste 命中"失败后怀疑白干"；解除"白干"赌注（教训=钟表时间收获）与 E3 呼应。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 薪资结构与晋升路径对比=实务分析请求，用户要信息与工具；B 段反场景（纯职业规划咨询不适用）生效。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 手在敲代码心飞交付日="身在此心在彼"的压力分裂，pressure-here-wanting-there 优先；无意义/空虚信号。 |
| edge-01 | 边界调用 | ✓ 通过 | 判定为"不启动双轴练习：兴趣丧失+睡眠改变+持续无意义感=抑郁筛查信号，先建议专业评估，本 skill 缓行"——与 E2 判停条件一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 无特殊边界。edge-01 与 should-trigger-02 的分界（哲学性空虚 vs 抑郁性空虚）在 description 的不适用清单与 E2 判停中均已写明。
- 回炉记录: 无。
