# test-results.md — social-proof

> 测试方式: 独立 sub-agent 盲测
> 测试时间: 2026-09-22

## 测试结果

| ID | 类型 | 预期 | 盲测结果 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | social-proof | social-proof ✅ | PASS |
| should-trigger-02 | should_trigger | social-proof | social-proof ✅ | PASS |
| should-trigger-03 | should_trigger | social-proof | social-proof ✅ | PASS |
| should-not-trigger-01 | should_not_trigger | 不触发 | none ✅ | PASS |
| should-not-trigger-02 | should_not_trigger | scarcity | scarcity ✅ | PASS |
| edge-01 | edge_case | 边界 | social-proof | PASS — agent 触发了，合理 |

## 通过率: 6/6 = 100% ✅

## 关键发现

- should-not-trigger-02 ("仅剩3件"想买): agent 正确识别为 scarcity 而非 social-proof
- edge-01 (朋友圈转发=好文章): agent 触发了 social-proof，合理——"好多人转发"确实触发社会认同。skill 激活后可引导验证转发动机

## 审计信息

- **通过率**: 100%
- **修复**: 无需修复
