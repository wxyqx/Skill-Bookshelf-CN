# test-results.md — 潜能-绩效九格矩阵与每格行动（nine-box-actions）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “盘点会凭印象填九宫格、填完也没动作”逐字命中 V2；先标准后填格＋每格动作在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “卓越/转型 vs 非全面/熟练分别该怎么处理”逐字命中 description 的“每个格子里的人分别该怎么处理”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “nine-box feels like a formality / slotted by gut feel” 命中触发词；输出证据纪律与逐格行动。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：Excel 九宫格模板制作属工具任务，description 明确无评估标准与证据诉求，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：只有一个人操心接班人要建制度命中兄弟 skill succession-five-steps，description 明确（矩阵只是第四步工具）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：任职三个月的经理能否填“非全面”——B/description 明确“任职未满六个月者的评价”不适用，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
