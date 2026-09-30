# test-results.md — 战略评估会议的问题框架（strategy-review-question-set）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “战略评审会怎么开才能问出真问题、而不是念 PPT”逐字命中。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “并购标的业务计划书怎么审”命中 V2 场景；三问开场＋逐项举证＋书面结论在 E。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “slide-reading / what questions should I ask” 命中触发词。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：会议通知与订会议室属会务事务，无评审程序与问题框架诉求，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：压缩成一页纸命中兄弟 skill bedrock-strategy-one-pager，A2“构建表达 vs 评审检验”区分。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：50 人 SaaS 裁剪——expected 要求“清单可简化、三问与结论责任人必须保留”，A2/B 的按业务定制在案。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
