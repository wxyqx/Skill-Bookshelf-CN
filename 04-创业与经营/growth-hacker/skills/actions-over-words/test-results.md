# 测试结果 — actions-over-words

- 盲测方式：2026-10-06 独立盲测代理判定——只看 21 个 skill 的 name+description 菜单，对 159 条用例做 21 选 1 选择题，未见 expected/notes。
- 本 skill 结果：**6/6 全通过（100%）**（should_trigger 3/3、should_not_trigger 2/2、edge_case 1/1）。
- 同书兄弟诱饵（should_not_trigger）48/48 全部正确转介或回避，0 跷跷板；判停/双归属/转介差异的用例见下表注脚。
- 详见：[docs/TEST_RESULTS.md](../../docs/TEST_RESULTS.md)

| 用例 | 类型 | 盲测归类 | 结果 |
|---|---|---|---|
| t01 | should_trigger | actions-over-words | ✅ |
| t02 | should_trigger | actions-over-words | ✅ |
| t03 | should_trigger | actions-over-words | ✅ |
| t04 | should_not_trigger | → mvp-validator（兄弟 skill 流转） * | ✅ |
| t05 | should_not_trigger | → none（判停，正确回避） * | ✅ |
| t06 | edge_case | actions-over-words | ✅ |

注脚：
- \*t04：转介：description 修复（跷跷板法）后明确排除假门类验证载体场景并指向 mvp-validator，正确转介；干净复测 6/6。
- \*t05：判停：明确可用性问题（行为与口头一致）已被 description 排除，其余 20 个 skill 无承接者，正确回避。
