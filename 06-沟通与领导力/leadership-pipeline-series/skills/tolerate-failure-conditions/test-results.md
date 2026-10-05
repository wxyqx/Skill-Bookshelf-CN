# test-results.md — 宽容失败三条件（给人才自由，把失败当信号）（tolerate-failure-conditions）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “想派高潜接手烂摊子但怕搞砸”逐字命中 V2；三条件体检＋失败预算在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “新岗位没做成是不是该放弃培养”命中失败归因三分类与调整路径（而非终止）。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “how much freedom should I give” 命中触发词；三项自由的边界与协商定指标在 E。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：连续两季不达标按什么流程处理——description 明确排除“常规绩效问题的追责”，指向绩效管理程序。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：给业务三年投入期、牺牲当期利润是否合理属业务投资决策，与培养性授权不同域，不激活。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：做砸一单但成长快是否不追究——B 段“允许失败≠豁免责任（合规/客户损失/诚信按制度）”，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
