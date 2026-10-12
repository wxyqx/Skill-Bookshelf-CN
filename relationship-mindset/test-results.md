# test-results.md — relationship-mindset

> 测试方式: 独立 sub-agent 盲测 (3 个 Explore agent 并行, 共 60 条 prompt)
> 测试时间: 2026-10-12

## 测试结果

| ID | 类型 | 预期 | 盲测结果 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | relationship-mindset | ✅ | PASS |
| should-trigger-02 | should_trigger | relationship-mindset | ✅ | PASS |
| should-trigger-03 | should_trigger | relationship-mindset | ✅ | PASS |
| should-not-trigger-01 | should_not_trigger | 不触发 | ✅ | PASS |
| should-not-trigger-02 | should_not_trigger | 其他 skill | ✅ | PASS |
| edge-01 | edge_case | 边界 | ✅ | PASS — 宿命型与成长型边界场景被正确区分 |

## 通过率: 6/6 = 100% ✅

## 关键发现

- 正面触发场景：3 条 should_trigger 均正确命中，说明 description 中"宿命型 vs 成长型""关系信念""天生一对 vs 努力经营"等 trigger 词精准有效
- 跨 skill 区分：should-not-trigger-02（跨 skill 混淆诱饵）被正确识别为其他 skill，说明关系信念这一核心概念边界清晰，不易与冲突管理、依恋类型等邻近概念混淆
- 边界场景：edge-01 涉及"伴侣认为关系问题是性格不合导致的"，同时带有冲突和信念色彩，sub-agent 仍正确判定为 relationship-mindset，说明核心触发逻辑稳定
- 整体评价：表现最优的 skill 之一。description 质量高，触发条件明确，与其他 skill 的区分度好，无需任何调整。

## 审计信息

- **通过率**: 100%
- **修复**: 无需修复
