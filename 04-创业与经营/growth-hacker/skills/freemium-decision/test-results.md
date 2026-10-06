# 测试结果 — freemium-decision

- 盲测方式：2026-10-06 独立盲测代理判定——只看 21 个 skill 的 name+description 菜单，对 159 条用例做 21 选 1 选择题，未见 expected/notes。
- 本 skill 结果：**7/7 全通过（100%）**（should_trigger 3/3、should_not_trigger 2/2、edge_case 2/2）。
- 同书兄弟诱饵（should_not_trigger）48/48 全部正确转介或回避，0 跷跷板；判停/双归属/转介差异的用例见下表注脚。
- 详见：[docs/TEST_RESULTS.md](../../docs/TEST_RESULTS.md)

| 用例 | 类型 | 盲测归类 | 结果 |
|---|---|---|---|
| t01 | should_trigger | freemium-decision | ✅ |
| t02 | should_trigger | freemium-decision | ✅ |
| t03 | should_trigger | freemium-decision | ✅ |
| t04 | should_not_trigger | → subsidy-ladder（兄弟 skill 流转） | ✅ |
| t05 | should_not_trigger | → turn-penalty-into-reward（兄弟 skill 流转） | ✅ |
| t06 | edge_case | → mvp-validator（兄弟 skill 流转） * | ✅ |
| t07 | edge_case | freemium-decision | ✅ |

注脚：
- \*t06：转介：假门页面测付费意愿命中 mvp-validator 的 fake door 触发词，验证载体设计移交 mvp-validator。
