# test-results — property-rights-timing

- **盲测方式**：独立 sub-agent 盲测（未参与蒸馏，仅见 16 skill 的 name+description 与 prompt 字面，做 16 选 1 + none 的判断）

| case | 类型 | 盲测判断 | 激活对象 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | yes | property-rights-timing | ✅ |
| should-trigger-02 | should_trigger | yes | property-rights-timing | ✅ |
| should-trigger-03 | should_trigger | yes | property-rights-timing | ✅ |
| should-not-trigger-01 | should_not_trigger | no | initial-identity-pricing | ✅ |
| should-not-trigger-02 | should_not_trigger | no | red-hat-structure-decision | ✅ |
| edge-01 | edge_case | weak | property-rights-timing | ✅ |

- **通过率**: 6/6 = 100%
- **minimum_pass_rate**: 0.8 → 通过 ✅

## 说明

edge_case 的盲测判断与 test-prompts.json 的 expectation 逐条核对一致。

> 本 skill 在首轮盲测中暴露与对方 skill 的触发重叠（改制方案被媒体质疑场景），已修补 description 边界并以干净盲测代理复测，复测 6/6 通过。
