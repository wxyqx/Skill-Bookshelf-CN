# test-results.md — authority

> 测试方式: 独立 sub-agent 盲测
> 测试时间: 2026-09-22

## 测试结果

| ID | 类型 | 预期 | 盲测结果 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | authority | authority ✅ | PASS |
| should-trigger-02 | should_trigger | authority | authority ✅ | PASS |
| should-trigger-03 | should_trigger | authority | authority ✅ | PASS |
| should-not-trigger-01 | should_not_trigger | 不触发 | none ✅ | PASS |
| should-not-trigger-02 | should_not_trigger | social-proof | social-proof ✅ | PASS |
| edge-01 | edge_case | 边界 | authority | PASS — agent 触发了，合理 |

## 通过率: 6/6 = 100% ✅

## 关键发现

- should-not-trigger-02 (10万人下载): agent 正确识别为 social-proof 而非 authority
- edge-01 (医生让做手术有疑问): agent 触发了 authority，合理——医生是相关领域专家但用户有疑问，skill 激活后可引导两问法和寻求第二意见

## 审计信息

- **通过率**: 100%
- **修复**: 无需修复
