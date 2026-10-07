# 测试结果 — aarrr-funnel-diagnosis

- 盲测方式：2026-10-06 独立盲测代理判定——只看 21 个 skill 的 name+description 菜单，对 159 条用例做 21 选 1 选择题，未见 expected/notes。
- 本 skill 结果：**9/9 全通过（100%）**（should_trigger 4/4、should_not_trigger 3/3、edge_case 2/2）。
- 同书兄弟诱饵（should_not_trigger）48/48 全部正确转介或回避，0 跷跷板；判停/双归属/转介差异的用例见下表注脚。
- 详见：[docs/TEST_RESULTS.md](../../docs/TEST_RESULTS.md)

| 用例 | 类型 | 盲测归类 | 结果 |
|---|---|---|---|
| t01 | should_trigger | aarrr-funnel-diagnosis | ✅ |
| t02 | should_trigger | aarrr-funnel-diagnosis | ✅ |
| t03 | should_trigger | aarrr-funnel-diagnosis | ✅ |
| t04 | should_trigger | aarrr-funnel-diagnosis | ✅ |
| t05 | should_not_trigger | → retention-diagnosis（兄弟 skill 流转） | ✅ |
| t06 | should_not_trigger | → growth-metrics-system（兄弟 skill 流转） | ✅ |
| t07 | should_not_trigger | → pmf-gate（兄弟 skill 流转） | ✅ |
| t08 | edge_case | → retention-diagnosis（兄弟 skill 流转） * | ✅ |
| t09 | edge_case | aarrr-funnel-diagnosis | ✅ |

注脚：
- \*t08：双归属边界：retention-diagnosis 的 description 明列该触发且归属更精确，PASS 条件为双侧其一（修测试留痕）。
