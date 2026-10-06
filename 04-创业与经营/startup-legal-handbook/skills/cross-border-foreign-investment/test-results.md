# test-results — cross-border-foreign-investment

- 盲测方式:集中盲测(终轮),独立评审代理仅依据 16 个 skill 的 name+description 菜单做选择题(2026-10-06)
- 全书 105 条用例同批判卷;两处真交界场景已标为 edge_case 并注明双 skill 协作

| 用例 | 类型 | 评审选择 | 结论 |
|---|---|---|---|
| should-trigger-01 | should_trigger | cross-border-foreign-investment | ✓ 触发本 skill |
| should-trigger-02 | should_trigger | cross-border-foreign-investment | ✓ 触发本 skill |
| should-trigger-03 | should_trigger | cross-border-foreign-investment | ✓ 触发本 skill |
| should-trigger-04 | should_trigger | cross-border-foreign-investment | ✓ 触发本 skill |
| should-not-trigger-01 | should_not_trigger | nominee-shareholding-risk | ✓ 未触发(判给 nominee-shareholding-risk) |
| should-not-trigger-02 | should_not_trigger | equity-transfer-pricing | ✓ 未触发(判给 equity-transfer-pricing) |
| edge-01 | edge_case | cross-border-foreign-investment | edge → cross-border-foreign-investment(均可接受) |
