# test-results.md — 社会化沟通执行机制的设计（social-operating-mechanism）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “转远程后信息滞后、决策慢”逐字命中 V2；五特征＋三步＋五病在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “会议多、同一议题反复上会没结论”命中无效会议五病（议而不决/没有跟进）。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “跨国团队六个国家、50 个经理同步顾客/对手/技术”命中五特征与 QMI 案例用法。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：规范汇报流程与审批链以过合规审计——description 明确排除“合规流程设计”，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：对个人的行为辅导命中兄弟 skill coaching-two-tracks，A2 明确（对象是个人不是机制）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：15 人同址团队——description 明确排除“10 人内同址团队”，expected 的“不必上完整机制”一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
