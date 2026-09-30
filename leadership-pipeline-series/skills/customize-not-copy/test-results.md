# test-results.md — 模型必须按组织定制，严禁机械照搬（customize-not-copy）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “网上找到头部公司领导力模型能直接抄吗”逐字命中 V2；定制三项操作在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “引进咨询公司体系但推不动、与实际不是一回事”命中“已经引入一套通用模型却发现水土不服”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “five-layer company but the model has six stages / force-fit” 命中触发词。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：讲解六阶段是什么属概念查询，description 明确排除“只需要理解模型概念本身”。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：把继任变成覆盖所有层级的制度命中兄弟 skill succession-five-steps，A2 明确（定制是其第一步而非全流程）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：20 人初创公司要不要搭模型——expected“建议不做或大幅裁剪（作者明确极小企业不获益）”，B 段适用门槛支撑。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
