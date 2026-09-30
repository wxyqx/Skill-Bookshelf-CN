# test-results.md — 领导缺陷四因与组织三缺失（leadership-deficit-four-causes）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “高薪空降的高管半年就不行、复盘该怪谁”逐字命中 V2；四因＋三缺失在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “连续三任同一岗位都失败”命中 description 的“公司总在同一个地方用人出错”与三缺失排查。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “set him up to fail / post-mortem” 命中触发词，输出机制修复＋合法处置边界。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：解除劳动合同的沟通与补偿测算——description 明确“不构成人力资源法律意见”，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：两部门职责扯皮命中兄弟 skill role-clarity-gaps-overlaps，A2 明确（四因之四的前半段另有专 skill）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：政策突变致市场消失——expected 先排除不可抗力；description 明确排除“不可抗的外部失败”，一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
