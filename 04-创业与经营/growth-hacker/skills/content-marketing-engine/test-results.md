# 测试结果 — content-marketing-engine

- 盲测方式：2026-10-06 独立盲测代理判定——只看 21 个 skill 的 name+description 菜单，对 159 条用例做 21 选 1 选择题，未见 expected/notes。
- 本 skill 结果：**8/8 全通过（100%）**（should_trigger 3/3、should_not_trigger 3/3、edge_case 2/2）。
- 同书兄弟诱饵（should_not_trigger）48/48 全部正确转介或回避，0 跷跷板；判停/双归属/转介差异的用例见下表注脚。
- 详见：[docs/TEST_RESULTS.md](../../docs/TEST_RESULTS.md)

| 用例 | 类型 | 盲测归类 | 结果 |
|---|---|---|---|
| t01 | should_trigger | content-marketing-engine | ✅ |
| t02 | should_trigger | content-marketing-engine | ✅ |
| t03 | should_trigger | content-marketing-engine | ✅ |
| t04 | should_not_trigger | → moment-marketing（兄弟 skill 流转） | ✅ |
| t05 | should_not_trigger | → do-things-that-dont-scale（兄弟 skill 流转） | ✅ |
| t06 | should_not_trigger | → seed-user-selection（兄弟 skill 流转） | ✅ |
| t07 | edge_case | → ab-testing-protocol（兄弟 skill 流转） * | ✅ |
| t08 | edge_case | → none（判停，正确回避） * | ✅ |

注脚：
- \*t07：转介：问题焦点在 A/B 实验设计规范本身，按 description 分工转介 ab-testing-protocol。
- \*t08：判停：description 明确排除付费投放与渠道选型问题，21 个 skill 中无承接者，如实记 none，判停正确。
