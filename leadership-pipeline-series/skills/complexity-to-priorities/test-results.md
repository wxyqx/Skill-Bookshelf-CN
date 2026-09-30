# test-results.md — 化繁为简的决策路径（因素→关系→基本行为→优先事项）（complexity-to-priorities）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “原材料涨价 30%、该涨价/换供应商/改配方”逐字命中 V2；四步推理与“停止做”清单在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “研究进入智能家居新市场、要做五年预测”命中“团队在臆想新市场”与“未来从已有世界产生”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “政策＋汇率＋新对手一起上、战略会开成信息汇报会”命中组织化用法与韦尔奇案例路径。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：已想清楚但不敢定、总说再等等命中兄弟 skill not-betting-is-betting，description 明确为先后步骤，不激活本 skill。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：并购标的市盈率与现金流质量命中兄弟 skill pe-multiple-wealth-mechanism，A2 明确（估值 vs 决策路径）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：20 人小公司汇率波动——E 段判停（信息缺失无法补齐转 not-betting）＋简化；expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
