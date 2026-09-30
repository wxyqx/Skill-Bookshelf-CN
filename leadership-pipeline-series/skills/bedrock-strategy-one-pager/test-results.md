# test-results.md — 基石式战略表达法（bedrock-strategy-one-pager）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “董事会只给 10 分钟”逐字命中 description；动作=先找基石并给可证伪承诺。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “40 页还是讲不清、团队复述不出来”命中“越写越厚、越讲越糊”；禁止删 PPT 替代思考在 A2/B。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “too complex to explain in one page” 命中触发词；输出一页纸结构。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：翻译任务属语言转换，description 的适用对象是战略的构建与表达，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：战略评审会该问什么命中兄弟 skill strategy-review-question-set（写 vs 审），A2 明确为表里，不激活本 skill。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：探索期一页纸——A2/B“过早压缩会把战略变成口号、可写假设式一页纸并转前提假设”，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
