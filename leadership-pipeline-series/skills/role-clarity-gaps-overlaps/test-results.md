# test-results.md — 明确职责三步法与职责断裂/重叠检查（role-clarity-gaps-overlaps）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “产品开发计划到底归谁、开会也没定论”逐字命中 V2；断裂/重叠二分与层级图在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “岗位说明书与实际干的不是一回事、好几个活没人管”命中“无人负责这块”与三步法。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “role ambiguity / two levels both give instructions” 命中关键信号。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：起草岗位说明书模板属文书，description 明确排除“单纯写招聘 JD”。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：刚提拔要定培养计划命中兄弟 skill performance-gap-circle，A2 明确顺序（先清职责再谈缺口）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：8 人无正式层级——expected“不宜套六阶段，用断裂/重叠两查法当场分工”，B 段“没有层级结构的临时项目组不适用”支持。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
