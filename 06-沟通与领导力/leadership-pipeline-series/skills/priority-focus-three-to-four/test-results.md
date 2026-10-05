# test-results.md — 优先事项聚焦（少而稳定的 3~4 项）（priority-focus-three-to-four）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “同时跑 20 个改进项目、资源打架，怎么砍”逐字命中 V2；四把尺＋两栏取舍在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “老板说有十个重点、每个都排了优先级”命中“目标清单有十条『重点』”；拒绝选择也是选择。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “重点方向每季度换一轮、下面已经麻木”命中“优先事项每季度换一轮”与稳定性约束。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：外部环境突变还没想清楚为命中兄弟 skill complexity-to-priorities（先推导后收口），description 明确先后。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：要不要退出业务一直定不下来命中兄弟 skill not-betting-is-betting（选太多 vs 不敢选）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：现金快断的危机——description 明确排除“危机期单点动员”，expected 的“单点全组织动员”一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
