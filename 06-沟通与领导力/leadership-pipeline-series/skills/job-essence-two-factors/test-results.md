# test-results.md — 工作本质双因素判定：决策权＋障碍（job-essence-two-factors）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “两个同名区域总监、工资差一倍，怎么判断是不是同一种工作”逐字命中 V2 场景与双因素判定。 |
| should-trigger-02 | 会激活 | ✓ 通过 | 面试追问岗位本质：触发词表含“岗位本质/决策权/障碍”，A2 明示它是建队访谈问题 3A/3B/4 的判据；判为激活（依据信号词与 A2，非仅 description 首句）。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “同批产品经理里有维护成熟线的、有从零做新线的，能否放进同一职级”命中“职级对标”与障碍因素。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：写岗位说明书，description 明确排除“纯写职位描述”。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：重建各层业绩标准命中兄弟 skill performance-pipeline-interview-build，A2“母流程 vs 子判据”明确。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：描述相同但监管与资源约束不同——expected 判定“本质不同工作”，双因素独立性的 I 段表述支持该结论。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
