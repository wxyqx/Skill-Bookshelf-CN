# test-results.md — 表现不佳者分层处置流程（underperformer-tiered-handling）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “老员工业绩下滑、资历深人缘好、解雇还是留着”逐字命中 V2 场景；分层＋取证＋体面程序在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “业绩达标但行为恶劣”命中“业绩好但行为差”类别；二选一谈话与行为证据准备在 A1/E。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “postponing the conversation about letting someone go” 命中“拖了很久不敢谈 / let someone go”触发词。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：补偿金测算=法律与 HR 专业测算，description 明确“不构成人力资源法律意见”，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：人才评估会命中兄弟 skill talent-review-meeting-mrr，A2“机制 vs 处置”分工，不激活。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：薪酬被压、职责不清→expected 要求先排除组织因素；B 段系列级伦理边界①在案，判定一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
