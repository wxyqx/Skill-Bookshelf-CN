# test-results — signal-engineering

- **盲测方式**：独立 sub-agent 盲测（未参与蒸馏，仅见 16 skill 的 name+description 与 prompt 字面，做 16 选 1 + none 的判断）

| case | 类型 | 盲测判断 | 激活对象 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | yes | signal-engineering | ✅ |
| should-trigger-02 | should_trigger | yes | signal-engineering | ✅ |
| should-trigger-03 | should_trigger | yes | signal-engineering | ✅ |
| should-not-trigger-01 | should_not_trigger | no | announcement-as-policy | ✅ |
| should-not-trigger-02 | should_not_trigger | no | none | ✅ |
| edge-01 | edge_case | yes | signal-engineering | ✅ |

- **通过率**: 6/6 = 100%
- **minimum_pass_rate**: 0.8 → 通过 ✅

## 说明

edge_case 的盲测判断与 test-prompts.json 的 expectation 逐条核对一致（含判停、转出、组合属性、默认不激活等精细预期）。
