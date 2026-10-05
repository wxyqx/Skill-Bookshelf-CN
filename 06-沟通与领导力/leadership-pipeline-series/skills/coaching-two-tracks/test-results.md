# test-results.md — 教练辅导双轨框架（业务轨＋行为轨）（coaching-two-tracks）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “刚被提拔、业绩还行但团队怨声载道”逐字命中 V2；业务轨/行为轨切割在 I/E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “总需要别人告诉他该做什么”命中 description 的“总等指令”信号；反馈太晚的预防用法在 A1。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “只有年度绩效评估一个正式谈话场合”命中 description 的“想反馈却只有年度评估一个场合”。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：启动绩效改进/考虑让人离开命中兄弟 skill underperformer-tiered-handling，description 明确排除“处分辞退程序”。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：信息变味、跨部门协调靠堆会议要做机制设计命中兄弟 skill social-operating-mechanism，A2 明确（机制 vs 个人辅导）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：外部顾问做高管教练——B 段/expected 的“外部教练观察位置局限＋上级为主教练＋三纪律”在案。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
