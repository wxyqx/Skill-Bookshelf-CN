# test-results.md — 现金净流入视角（公司氧气与人人有责）（cash-net-inflow-everyones-business）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “账面利润不错但现金越来越紧、钱去哪了”逐字命中 V2；三提问＋账期与存货时间差在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “采购经理怎么帮公司改善现金”逐字命中 V2；岗位级现金映射清单在 E。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “增长很快反而越来越缺钱”命中“增长反而更缺钱”与现金机器识别。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：两家 ROA 比效率命中兄弟 skill r-m-v-return-decomposition，description 明确排除（现金口径 vs 收益率口径）。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：美元债融资方案设计，description 明确排除“融资方案设计”。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：长周期工程公司天然负现金流——B 段“现金机器模式依赖外部条件、不能硬套”在案，expected 的调整期望一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
