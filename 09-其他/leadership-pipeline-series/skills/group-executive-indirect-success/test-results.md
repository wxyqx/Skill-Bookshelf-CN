# test-results.md — 集团高管：间接成功与组合管理（group-executive-indirect-success）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “管着三个事业部、比总经理们还忙、替他们做决策”逐字命中 V2；理念三问＋越俎代庖在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “集团高管考核只有收入利润指标”命中“考核标准不含育人会把他逼回事业部总经理行为”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “高管远离总部跑业务、说总部是象牙塔”命中“与总部对立”触发词与时间基准（已核“行业地位”“新业务”）。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：事业部总经理太爱当超人命中兄弟 skill business-manager-complexity-triangle，description 明确排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：接任 CEO 前 90 天做什么命中兄弟 skill ceo-five-challenges，description 明确排除。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：控股型集团只投钱不经营——expected“核心理念保留、技能与时间要求调整＋声明 GE 式原型”，A2/B 支撑。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
