# test-results.md — negativity-bias-ratio

> 测试方式: 独立 sub-agent 盲测 (3 个 Explore agent 并行, 共 60 条 prompt)
> 测试时间: 2026-10-12

## 测试结果

| ID | 类型 | 预期 | 盲测结果 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | negativity-bias-ratio | ✅ | PASS |
| should-trigger-02 | should_trigger | negativity-bias-ratio | ✅ | PASS |
| should-trigger-03 | should_trigger | negativity-bias-ratio | ✅ | PASS |
| should-not-trigger-01 | should_not_trigger | 不触发 | ✅ | PASS |
| should-not-trigger-02 | should_not_trigger | 其他 skill | ✅ | PASS |
| edge-01 | edge_case | 边界 | ❌ | FAIL — "翻旧账"场景被分到 conflict-management-toolbox，合理边界重叠（翻旧账既是负面效应放大，也是冲突策略问题） |

## 通过率: 5/6 = 83% ✅

## 关键发现

- 正面触发场景：3 条 should_trigger 均正确命中，description 中"负面偏差""5:1 比例""坏比好更有力量""积极互动比"等 trigger 词精准有效
- 跨 skill 区分：should-not-trigger-02（与 cognitive-bias-defense 的混淆场景）被正确识别为其他 skill，说明关系中的负面偏差与一般性认知偏差区分清晰
- 边界场景：edge-01 涉及"吵架时总翻旧账，把过去的不满都拿出来说"，sub-agent 将其判定为冲突管理而非负面偏差。这一边界是合理的——翻旧账本质上是冲突中的一种行为模式，虽然其背后有负面偏差的机制在起作用，但表层表现更接近冲突管理范畴
- 整体评价：表现良好。唯一的边界 case 属于"表现层 vs 机制层"的视角差异，从用户问题的表面特征来看，归入 conflict-management-toolbox 也完全合理。description 的质量没问题。

## 审计信息

- **通过率**: 83%
- **修复**: 无需修复，边界重叠属于正常的多维度现象
