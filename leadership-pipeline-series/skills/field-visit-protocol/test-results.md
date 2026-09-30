# test-results.md — 深入一线视察流程（field-visit-protocol）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “一年去不了两次、下属报喜不报忧”命中 description 关键信号；动作=带假设入场＋四段式程序＋书面结论。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “下周去工厂视察、不走马观花”命中；SKILL.md 内已含“尖锐问题出现率/书面化/复查期”验收标准（已核）。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “remote / unfiltered information” 命中 description 的“远程团队怎么了解”，四要素向远程迁移的动作在 A2。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：安全生产审计属合规专业审计，description 明确排除“合规审计”，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：会上追问扩张计划命中兄弟 skill question-to-reality，A2“组织内侧视察 vs 会议追问”区分，不激活。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：远程全员会替代视察的条件（四要素缺一不可）在 A2/E；expected 的“形式可替代、要素不可省”一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
