# test-results.md — 事业部总经理：协同三角形与整合团队（business-manager-complexity-triangle）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “接手事业部、利润与份额双降、第一刀砍哪”逐字命中 V2；三角逐角检查在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “通宵自己上、部门各干各的、团队散沙”命中“不做超人/整合团队”硬要求。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “只把成熟产品做得更高效、没人讨论这条线还要不要留”命中“从能不能做到该不该做”的里程碑转变。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：职能主管只关心自己那块研发命中兄弟 skill functional-manager-maturity，description 明确排除（第三阶段 vs 第四阶段）。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：管三个事业部比总经理还忙命中兄弟 skill group-executive-indirect-success，description 明确排除。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：平台型业务——B 段已内置“平台型/软件型取舍逻辑未覆盖、须本地化”（已核），expected 的“重构三角＋声明前提”一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
