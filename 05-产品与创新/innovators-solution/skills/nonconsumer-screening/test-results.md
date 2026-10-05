# test-results — nonconsumer-screening

- **盲测方式**：独立 sub-agent 盲测（未参与蒸馏，仅见 15 skill 的 name+description 与 prompt 字面，做 15 选 1 + none 的判断）

| case | 类型 | 盲测判断 | 激活对象 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | yes | nonconsumer-screening | ✅ |
| should-trigger-02 | should_trigger | yes | nonconsumer-screening | ✅ |
| should-trigger-03 | should_trigger | yes | nonconsumer-screening | ✅ |
| should-not-trigger-01 | should_not_trigger | no | three-stone-tests | ✅ |
| should-not-trigger-02 | should_not_trigger | no | new-market-disruption-pattern | ✅ |
| edge-01 | edge_case | yes | nonconsumer-screening | ✅ |

- **通过率**: 6/6 = 100%
- **minimum_pass_rate**: 0.8 → 通过 ✅

## 说明

edge_case 的盲测判断与 test-prompts.json 的 expectation 逐条核对一致。
