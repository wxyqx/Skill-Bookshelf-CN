# test-results — speed-four-abilities

- **盲测方式**：独立 sub-agent 盲测（未参与蒸馏，仅见 17 skill 的 name+description 与 prompt 字面，做 17 选 1 + none 的判断）

| case | 类型 | 盲测判断 | 激活对象 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | yes | speed-four-abilities | ✅ |
| should-trigger-02 | should_trigger | yes | speed-four-abilities | ✅ |
| should-trigger-03 | should_trigger | yes | speed-four-abilities | ✅ |
| should-not-trigger-01 | should_not_trigger | no | sunk-cost-restart | ✅ |
| should-not-trigger-02 | should_not_trigger | no | endgame-reasoning | ✅ |
| edge-01 | edge_case | yes | speed-four-abilities | ✅ |

- **通过率**: 6/6 = 100%
- **minimum_pass_rate**: 0.8 → 通过 ✅

## 说明

edge_case 的盲测判断与 test-prompts.json 的 expectation 逐条核对一致。
