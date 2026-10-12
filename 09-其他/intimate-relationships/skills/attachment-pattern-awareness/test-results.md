# test-results.md — attachment-pattern-awareness

> 测试方式: 独立 sub-agent 盲测 (3 个 Explore agent 并行, 共 60 条 prompt)
> 测试时间: 2026-10-12

## 测试结果

| ID | 类型 | 预期 | 盲测结果 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | attachment-pattern-awareness | ✅ | PASS |
| should-trigger-02 | should_trigger | attachment-pattern-awareness | ✅ | PASS |
| should-trigger-03 | should_trigger | attachment-pattern-awareness | ✅ | PASS |
| should-not-trigger-01 | should_not_trigger | 不触发 | ✅ | PASS |
| should-not-trigger-02 | should_not_trigger | 其他 skill | ✅ | PASS |
| edge-01 | edge_case | 边界 | ✅ | PASS — 焦虑型依恋与认知偏差的边界被正确区分 |

## 通过率: 6/6 = 100% ✅

## 关键发现

- 正面触发场景：3 条 should_trigger 均正确命中，description 中"依恋类型""安全型/焦虑型/回避型""早期经历""亲密关系模式"等 trigger 词识别度高
- 跨 skill 区分：should-not-trigger-02 设计为与 cognitive-bias-defense 的混淆场景（对伴侣行为的过度解读），sub-agent 正确判断为认知偏差而非依恋模式，说明两者边界清晰
- 边界场景：edge-01 涉及"伴侣总是担心我不爱他，反复需要确认"，同时带有焦虑依恋和认知偏差色彩，sub-agent 准确识别为依恋模式问题，核心判定逻辑稳固
- 整体评价：表现最优的 skill 之一。依恋类型作为亲密关系中辨识度极高的概念，description 的质量进一步确保了精准触发，与其他 skill 的区分度极佳。

## 审计信息

- **通过率**: 100%
- **修复**: 无需修复
