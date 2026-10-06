# 测试结果 — investment-advice-discipline

- 盲测方式：2026-10-06 独立盲测代理判定——只看 20 个 skill 的 name+description 菜单，对 180 条用例做 20 选 1 选择题，未见 expected/notes。
- 本 skill 结果：**9/9 全通过（100%）**（should_trigger 4/4、should_not_trigger 3/3、edge_case 2/2）。
- 同书兄弟诱饵（should_not_trigger）59/59 全归类正确，0 跷跷板；2 对触发冲突已按跷跷板法修复并干净复测 18/18。
- 详见：[../docs/TEST_RESULTS.md](../docs/TEST_RESULTS.md)

| 用例 | 类型 | 盲测归类 | 结果 |
|---|---|---|---|
| t01 | should_trigger | investment-advice-discipline | ✅ |
| t02 | should_trigger | investment-advice-discipline | ✅ |
| t03 | should_trigger | investment-advice-discipline | ✅ |
| t04 | should_trigger | investment-advice-discipline | ✅ |
| n01 | should_not_trigger | → protection-over-forecast（兄弟 skill 流转） | ✅ |
| n02 | should_not_trigger | → rule-reliability-trend-skepticism（兄弟 skill 流转） | ✅ |
| n03 | should_not_trigger | → invest-vs-speculation-filter（兄弟 skill 流转） | ✅ |
| e01 | edge_case | investment-advice-discipline | ✅ |
| e02 | edge_case | investment-advice-discipline | ✅ |
