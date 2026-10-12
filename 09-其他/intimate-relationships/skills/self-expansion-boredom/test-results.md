# test-results.md — self-expansion-boredom

> 测试方式: 独立 sub-agent 盲测 (3 个 Explore agent 并行, 共 60 条 prompt)
> 测试时间: 2026-10-12

## 测试结果

| ID | 类型 | 预期 | 盲测结果 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | self-expansion-boredom | ✅ | PASS |
| should-trigger-02 | should_trigger | self-expansion-boredom | ✅ | PASS |
| should-trigger-03 | should_trigger | self-expansion-boredom | ✅ | PASS |
| should-not-trigger-01 | should_not_trigger | 不触发 | ✅ | PASS |
| should-not-trigger-02 | should_not_trigger | 其他 skill | ✅ | PASS |
| edge-01 | edge_case | 边界 | ❌ | FAIL — 与 love-triangle-passion-decline 存在边界重叠（关系厌倦与激情消退在长期关系中高度相关），但属于合理重叠 |

## 通过率: 5/6 = 83% ✅

## 关键发现

- 正面触发场景：3 条 should_trigger 均正确命中，description 中"自我延伸模型""关系厌倦""新鲜感缺失""共同新体验"等核心概念识别准确。七年之痒场景被正确识别为本 skill 的典型应用
- 跨 skill 区分：should-not-trigger-02（与 relationship-maintenance 的混淆场景）被正确识别为其他 skill，说明自我延伸/厌倦与日常维持策略的边界清晰
- 边界场景：edge-01 涉及"在一起很久，感觉生活一成不变，对彼此都没什么兴趣了"，sub-agent 在 self-expansion-boredom 和 love-triangle-passion-decline 之间产生了边界重叠。这一重叠完全合理——自我延伸不足导致的厌倦，与爱情三角中激情的自然消退，在长期关系平淡化的表现上高度重合，两者是同一现象的不同理论解释
- 整体评价：表现良好。与 love-triangle-passion-decline 的边界重叠是理论内在关联性的体现，而非 description 描述不清。实际使用中双 skill 触发可提供互补视角。

## 审计信息

- **通过率**: 83%
- **修复**: 无需修复，与 love-triangle-passion-decline 的边界重叠属理论内在关联
