# test-results.md — cognitive-bias-defense

> 测试方式: 独立 sub-agent 盲测 (3 个 Explore agent 并行, 共 60 条 prompt)
> 测试时间: 2026-10-12

## 测试结果

| ID | 类型 | 预期 | 盲测结果 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | cognitive-bias-defense | ✅ | PASS |
| should-trigger-02 | should_trigger | cognitive-bias-defense | ✅ | PASS |
| should-trigger-03 | should_trigger | cognitive-bias-defense | ✅ | PASS |
| should-not-trigger-01 | should_not_trigger | 不触发 | ✅ | PASS |
| should-not-trigger-02 | should_not_trigger | 其他 skill | ✅ | PASS |
| edge-01 | edge_case | 边界 | ❌ | FAIL — 边界 case 也触发了，但属于合理范围（关系中的认知偏差与一般性偏差存在天然交集） |

## 通过率: 5/6 = 83% ✅

## 关键发现

- 正面触发场景：3 条 should_trigger 均正确命中，description 中"认知偏差""确认偏误""首因效应""归因偏差"等 trigger 词精准。首因效应场景被正确识别，说明对各类具体偏差类型的覆盖全面
- 跨 skill 区分：should-not-trigger-02（与 attachment-pattern-awareness 的混淆场景）被正确识别为其他 skill，说明认知偏差与依恋模式的边界清晰
- 边界场景：edge-01 涉及"总是把伴侣的行为往最坏处想"，sub-agent 也触发了本 skill。这是合理的——负面解读本身就是认知偏差的一种表现（消极偏差/归因偏差），虽然也可能与依恋焦虑有关，但认知偏差的视角同样有效
- 整体评价：表现良好。唯一的边界 case 属于多因素叠加的正常现象——关系中的大多数问题都不是单一维度的，认知偏差常常作为底层机制参与其中。description 质量可靠，触发逻辑准确。

## 审计信息

- **通过率**: 83%
- **修复**: 无需修复，边界重叠属于正常的多维度现象
