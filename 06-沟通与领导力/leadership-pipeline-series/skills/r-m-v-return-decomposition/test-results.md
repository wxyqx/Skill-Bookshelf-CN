# test-results.md — R=M×V：资产收益率＝利润率×周转率（r-m-v-return-decomposition）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “两家 ROE 都是 15%、奢侈品 vs 超市”逐字命中 V2；M×V 结构判别在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “利润率很薄、老板想砍、我觉得还能救”命中“业务值不值得继续做”的门槛判断。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “老板要压库存、销售反对，怎么用听得懂的方式说明”命中用 V 解释周转改善收益率的说明动作。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：系统搞懂公司怎么赚钱命中兄弟 skill business-acumen-six-elements，description 明确排除（单要素拆解 vs 总框架）。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：有利润没现金命中兄弟 skill cash-net-inflow-everyones-business，description 明确排除（收益率口径 vs 现金口径）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：生物科技无形投入——B 段适用性限制（资产/存货为核心的口径对研发投入解释力弱），expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
