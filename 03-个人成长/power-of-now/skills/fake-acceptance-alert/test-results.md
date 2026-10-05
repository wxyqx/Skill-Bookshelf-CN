# test-results.md — 假接纳警报（fake-acceptance-alert）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程自测（fallback）** — 无独立 sub-agent 能力，主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判，判完对答案；混淆题用 19 个 skill 的 name+description 全量列表做选择。fallback 结果，可信度低于独立盲测。
- **测试对象**: test-prompts.json v0.1.0，共 7 条（should_trigger 3 / should_not_trigger 3 / edge_case 1）
- **最低通过率**: 0.8

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "正念冥想一年，堵车还暴怒，是不是白练了"=description 首 trigger（mindfulness plateau / 练了这么久怎么还是这样），verified.md V2 场景；动作=三行对照→判定阶段→拆堵车暴怒机制→"不再创造"动作（E1-E4）。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "朋友圈全是允许一切发生，越修越苦，关系越来越远"=话术与实况分裂+徽章化分离感（ce15 信号）；识别+引导进入第二阶段与 I 段机制一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 以"随缘、不执着"回避跟老板谈涨薪=用修行话术替代行动（A2 场景 3 原文）；动作=把回避事项具体化并定行动时点（E4）。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 急性事件现场（项目黄了当晚、情绪特别大）需要 two-surrender-chances 的两级程序；description 不适用清单明示"急性情绪事件现场"——元诊断在此是二次伤害。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 对具体伤害事件的怨恨清库→present-forgiveness 优先；本 skill 需要长期修炼平台期语境（练了很久+话术与情绪不符），prompt 中不存在。 |
| should-not-trigger-03 | 边界判定：不支持指责 | ✓ 通过 | 朋友用"假接纳"否定用户对裁员方案的愤怒——B 段明示"不得用本 skill 否定正当愤怒"，对不公安排的愤怒可能是健康反应，应先评估情境合理性。预期行为即"不激活去支持该指责"，判定吻合，计为通过。 |
| edge-01 | 边界调用 | ✓ 通过 | 判定为"先用步骤 1-2 判定是真接纳的坚持期还是精神标记（看频率强度有无变化）；若焦虑呈持续临床特征（影响睡眠、工作、躯体症状），明确建议专业评估，不替代治疗"——与预期的分界点（持续时间与功能损害）一致。 |

## 通过率与结论

- **通过 7/7 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: should-not-trigger-03 与 present-forgiveness 的 should-not-trigger-03 同型（都是"第三方用本框架施压"的误用诱饵），两个 skill 的 B 段均须可见且判定一致——实测均通过。
- 回炉记录: 无。
