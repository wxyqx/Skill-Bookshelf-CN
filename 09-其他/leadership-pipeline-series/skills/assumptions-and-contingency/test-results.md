# test-results.md — 前提假设显性化与应急计划（assumptions-and-contingency）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “海外建厂提案怎么做压力测试”逐字命中 V2；不超过六个前提＋取证＋最坏情形起点在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “预算会上数字对不上、谁也不说自己的假设”逐字命中 description。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “worst-case / stress-test this plan” 命中触发词；输出前提清单与应急触发条件。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：竞品价格监测表属数据采集与报表工具，description 排除（“纯财务核算”与工具需求），不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：预算会整体怎么开命中兄弟 skill operations-plan-three-step，A2 明确本 skill 是其第一步的放大处理。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：取证受限——E 段“无法核实的假设显式标注＋条件句/多情景＋不得当事实使用”，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
