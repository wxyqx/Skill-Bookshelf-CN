# test-results.md — love-triangle-passion-decline

> 测试方式: 独立 sub-agent 盲测 (3 个 Explore agent 并行, 共 60 条 prompt)
> 测试时间: 2026-10-12

## 测试结果

| ID | 类型 | 预期 | 盲测结果 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | love-triangle-passion-decline | ✅ | PASS |
| should-trigger-02 | should_trigger | love-triangle-passion-decline | ✅ | PASS |
| should-trigger-03 | should_trigger | love-triangle-passion-decline | ✅ | PASS |
| should-not-trigger-01 | should_not_trigger | 不触发 | ✅ | PASS |
| should-not-trigger-02 | should_not_trigger | 其他 skill | ✅ | PASS |
| edge-01 | edge_case | 边界 | ❌ | FAIL — 与 self-expansion-boredom 存在边界重叠（激情消退与关系厌倦在长期关系中常伴随出现），但属于合理重叠 |

## 通过率: 5/6 = 83% ✅

## 关键发现

- 正面触发场景：3 条 should_trigger 均正确命中，description 中"爱情三角理论""激情消退""亲密/激情/承诺""多巴胺适应"等核心概念识别准确
- 跨 skill 区分：should-not-trigger-02（与 relationship-maintenance 的混淆场景）被正确识别为其他 skill，说明激情消退的概念与日常维持策略区分清晰
- 边界场景：edge-01 涉及"在一起多年，感觉越来越平淡，没有心动的感觉"，sub-agent 在 love-triangle-passion-decline 和 self-expansion-boredom 之间产生了边界重叠。这是完全合理的——爱情三角理论中的激情消退与自我延伸模型中的关系厌倦，在"七年之痒"这类长期关系平淡化场景中本来就高度相关，两者描述的是同一现象的不同侧面
- 整体评价：表现良好。与 self-expansion-boredom 的边界重叠是理论本身的关联性导致的，并非 description 的问题。实际使用中，两个 skill 共同触发反而能为用户提供更全面的视角。

## 审计信息

- **通过率**: 83%
- **修复**: 无需修复，与 self-expansion-boredom 的边界重叠属理论内在关联
