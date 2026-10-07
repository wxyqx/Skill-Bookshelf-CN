# test-results — ratio-revision-rules

- 盲测方式:集中盲测,独立评审代理仅依据 18 个 skill 的 name+description 菜单做选择题(2026-10-05)
- 全书 111 条用例同批判卷,本 skill 满分通过
- 结果:**7/7**


| 用例 | 类型 | 期望 | 评审选择 |
|---|---|---|---|
| should-trigger-01 | should_trigger | 期望: 触发本 skill | ✓ ratio-revision-rules |
| should-trigger-02 | should_trigger | 期望: 触发本 skill | ✓ ratio-revision-rules |
| should-trigger-03 | should_trigger | 期望: 触发本 skill | ✓ ratio-revision-rules |
| should-trigger-04 | should_trigger | 期望: 触发本 skill | ✓ ratio-revision-rules |
| should-not-trigger-01 | should_not_trigger | 期望: 不触发(判给 capital-structure-four-forces) | ✓ capital-structure-four-forces |
| should-not-trigger-02 | should_not_trigger | 期望: 不触发(判给 differential-analysis) | ✓ differential-analysis |
| edge-01 | edge_case | 期望: 不触发(判给 ratio-revision-rules) | ✓ ratio-revision-rules |
