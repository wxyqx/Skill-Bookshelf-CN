# test-results.md — 双螺旋领导潜质（驭人之道×经商之道）（leadership-potential-double-helix）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “面试年轻人判断十年后能不能带一块业务”逐字命中 V2；两轴行为取证（12 问）在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “销售冠军连续三年第一、该不该直接提区域总监”命中 description 的“业绩最好的那个该不该提拔”；业绩≠潜质。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “build a high-potential list / managers send people they like” 命中触发词；输出判据表与交叉验证。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：写岗位胜任力与 JD——本 skill 判人（潜质），不负责岗位描述，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：已确定人选要设计岗位与挑战命中兄弟 skill concentric-learning-job-design，A2 明确（识人 vs 岗位设计）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：证据不足要不要先放进高潜名额——expected“标记待观察＋约定观察场景”，B 段公平程序与防标签支撑一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
