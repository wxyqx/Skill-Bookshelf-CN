# test-results — long-term-asset-quality

- 盲测方式:集中盲测,独立评审代理仅依据 18 个 skill 的 name+description 菜单做选择题(2026-10-05)
- 全书 111 条用例同批判卷,本 skill 满分通过
- 结果:**6/6**


| 用例 | 类型 | 期望 | 评审选择 |
|---|---|---|---|
| should-trigger-01 | should_trigger | 期望: 触发本 skill | ✓ long-term-asset-quality |
| should-trigger-02 | should_trigger | 期望: 触发本 skill | ✓ long-term-asset-quality |
| should-trigger-03 | should_trigger | 期望: 触发本 skill | ✓ long-term-asset-quality |
| should-not-trigger-01 | should_not_trigger | 期望: 不触发(判给 earnings-manipulation-tactics) | ✓ earnings-manipulation-tactics |
| should-not-trigger-02 | should_not_trigger | 期望: 不触发(判给 asset-allocation-strategy) | ✓ asset-allocation-strategy |
| edge-01 | edge_case | 期望: 不触发(判给 long-term-asset-quality) | ✓ long-term-asset-quality |
