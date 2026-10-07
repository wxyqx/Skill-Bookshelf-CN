# 测试结果 — ab-testing-protocol

- 盲测方式：2026-10-06 独立盲测代理判定——只看 21 个 skill 的 name+description 菜单，对 159 条用例做 21 选 1 选择题，未见 expected/notes。
- 本 skill 结果：**8/8 全通过（100%）**（should_trigger 3/3、should_not_trigger 3/3、edge_case 2/2）。
- 同书兄弟诱饵（should_not_trigger）48/48 全部正确转介或回避，0 跷跷板；判停/双归属/转介差异的用例见下表注脚。
- 详见：[docs/TEST_RESULTS.md](../../docs/TEST_RESULTS.md)

| 用例 | 类型 | 盲测归类 | 结果 |
|---|---|---|---|
| t01 | should_trigger | ab-testing-protocol | ✅ |
| t02 | should_trigger | ab-testing-protocol | ✅ |
| t03 | should_trigger | ab-testing-protocol | ✅ |
| t04 | should_not_trigger | → activation-aha-magic-number（兄弟 skill 流转） | ✅ |
| t05 | should_not_trigger | → growth-metrics-system（兄弟 skill 流转） | ✅ |
| t06 | should_not_trigger | → none（判停，正确回避） * | ✅ |
| t07 | edge_case | → freemium-decision（兄弟 skill 流转） * | ✅ |
| t08 | edge_case | ab-testing-protocol | ✅ |

注脚：
- \*t06：判停：description 明确排除方向性/模式级大改变决策（A/B 测不出跃进式创新），无其他 skill 承接，如实记 none，正确回避。
- \*t07：转介："悄悄删免费选项试验"属 freemium-decision 的静默砍免费版流程，非通用 A/B 方法问题。
