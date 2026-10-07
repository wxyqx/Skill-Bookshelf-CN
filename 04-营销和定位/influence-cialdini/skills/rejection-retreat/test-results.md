# test-results.md — rejection-retreat

> 测试方式: 独立 sub-agent 盲测
> 测试时间: 2026-09-22

## 测试结果

| ID | 类型 | 预期 | 盲测结果 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | rejection-retreat | rejection-retreat ✅ | PASS |
| should-trigger-02 | should_trigger | rejection-retreat | rejection-retreat ✅ | PASS |
| should-trigger-03 | should_trigger | rejection-retreat | rejection-retreat ✅ | PASS |
| should-not-trigger-01 | should_not_trigger | 不触发(讨价还价) | none ✅ | PASS |
| should-not-trigger-02 | should_not_trigger | reciprocity-defense | reciprocity-defense ✅ | PASS |
| edge-01 | edge_case | 对比或拒绝退让 | rejection-retreat | PASS — agent 触发了，合理 |

## 通过率: 6/6 = 100% ✅

## 关键发现

- should-not-trigger-01 (讨价还价从200到150): agent 正确识别为正常议价而非拒绝退让
- should-not-trigger-02 (送水后推销): agent 正确识别为 reciprocity-defense
- edge-01 (先说500万再看350万): agent 触发了 rejection-retreat，这是合理的——中介先报高价（被拒）再推荐低价房，符合"先大后小"模式

## 审计信息

- **通过率**: 100%
- **修复**: 无需修复
