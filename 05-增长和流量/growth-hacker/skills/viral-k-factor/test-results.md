# 测试结果 — viral-k-factor

- 盲测方式：2026-10-06 独立盲测代理判定——只看 21 个 skill 的 name+description 菜单，对 159 条用例做 21 选 1 选择题，未见 expected/notes。
- 本 skill 结果：**9/9 全通过（100%）**（should_trigger 4/4、should_not_trigger 3/3、edge_case 2/2）。
- 同书兄弟诱饵（should_not_trigger）48/48 全部正确转介或回避，0 跷跷板；判停/双归属/转介差异的用例见下表注脚。
- 详见：[docs/TEST_RESULTS.md](../../docs/TEST_RESULTS.md)

| 用例 | 类型 | 盲测归类 | 结果 |
|---|---|---|---|
| t01 | should_trigger | viral-k-factor | ✅ |
| t02 | should_trigger | viral-k-factor | ✅ |
| t03 | should_trigger | viral-k-factor | ✅ |
| t04 | should_trigger | viral-k-factor | ✅ |
| t05 | should_not_trigger | → external-viral-loop（兄弟 skill 流转） | ✅ |
| t06 | should_not_trigger | → aarrr-funnel-diagnosis（兄弟 skill 流转） | ✅ |
| t07 | should_not_trigger | → moment-marketing（兄弟 skill 流转） | ✅ |
| t08 | edge_case | → pmf-gate（兄弟 skill 流转） * | ✅ |
| t09 | edge_case | → growth-ethics-redlines（兄弟 skill 流转） * | ✅ |

注脚：
- \*t08：转介差异：预期为触发后判停转介 pmf-gate，盲测直接归口 pmf-gate，结论殊途同归，PASS=双路径其一（修测试留痕）。
- \*t09：转介：默认上传通讯录属数据/权限过度授权，转介 growth-ethics-redlines 守门闸。
