# test-results — equity-rights-design

- 盲测方式:集中盲测(终轮),独立评审代理仅依据 16 个 skill 的 name+description 菜单做选择题(2026-10-06)
- 全书 105 条用例同批判卷;两处真交界场景已标为 edge_case 并注明双 skill 协作

| 用例 | 类型 | 评审选择 | 结论 |
|---|---|---|---|
| should-trigger-01 | should_trigger | equity-rights-design | ✓ 触发本 skill |
| should-trigger-02 | should_trigger | equity-rights-design | ✓ 触发本 skill |
| should-trigger-03 | should_trigger | equity-rights-design | ✓ 触发本 skill |
| should-not-trigger-01 | should_not_trigger | charter-governance-design | ✓ 未触发(判给 charter-governance-design) |
| should-not-trigger-02 | should_not_trigger | capital-contribution-compliance | ✓ 未触发(判给 capital-contribution-compliance) |
| edge-01 | edge_case | employee-equity-incentive | edge → employee-equity-incentive(均可接受) |
