# test-results.md — P-E 值：财富创造机制与管理纪律（pe-multiple-wealth-mechanism）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “收购一家公司、怎么判断贵不贵”逐字命中 V2；倍数拆成质量×可预见性在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “同样一年赚 10 亿、市值只有同行一半”命中“同样利润为何财富差很多”与可口可乐/百事对照。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “季度目标与长期研发投入打架、CFO 要求每股收益达标”——expected 要求激活并携带短期主义与合规 Boundary；本 skill 已内置 b3-ce08 risk_note（已核），判定一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：行业未来两年会怎样、该抓哪几个重点命中兄弟 skill complexity-to-priorities，description 明确排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：快速看公司经营状况命中兄弟 skill company-panorama-seven-questions，description 明确排除。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：未上市家族企业不打算卖——description 明确排除“未上市且无出售/上市计划”，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
