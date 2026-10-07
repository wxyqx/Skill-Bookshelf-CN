# test-results.md — 管理/技术双轨发展框架（dual-track-management-technical）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “最好的工程师不想做管理、只有管理岗才能加薪”逐字命中 V2；技术轨定义在 I/E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “销售明星提成经理两年都很痛苦”命中“被硬提上管理岗后水土不服”；放回专业岗是官方出口。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “too many managers with one or two reports / titles are a joke” 命中多领导综合征。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：首席工程师 JD 与面试题属招聘执行，无通道设计诉求，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：集团财务负责人的矩阵关系命中兄弟 skill corporate-function-six-relations，description 明确排除。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：只带两人的经理岗是否砍掉——expected 谨慎区分刻意培养与伪管理岗＋合规协商提示，B 段含劳动法边界。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
