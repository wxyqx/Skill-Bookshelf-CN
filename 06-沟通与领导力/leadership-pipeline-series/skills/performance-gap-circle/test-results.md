# test-results.md — 绩效圆圈与绩效缺口：七项内容与培养四步循环（performance-gap-circle）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “销售冠军提主管、定培养计划、不知从哪几项入手”逐字命中 V2；七项圆圈＋补缺→测试→升级四步循环在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “业务能力很强但只顾自己做业务、不带团队不管客户”命中 description 的“只会自己干活不会带团队”；定位到领导绩效/客户绩效。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “development plan for a newly promoted manager / what the gap actually is” 命中触发词。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：算 KPI 完成率与奖金系数属数据核算，description 排除（“纯 KPI 数字对账”），不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：两部门职责扯皮命中兄弟 skill role-clarity-gaps-overlaps，description 明确（先清职责再谈缺口）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：未晋升者绩效差——expected 要求调整用法（不是晋升缺口）；B 段“职责未澄清不画圈”与缺口逻辑限定于层级转换，支撑一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
