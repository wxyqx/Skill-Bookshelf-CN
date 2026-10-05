# test-results.md — 贡献自问法（contribution-question）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "被提名加入行业委员会秘书处，不确定该不该接受"命中 description 的"要不要接一个职位/项目/委员会"；预期（用"这里我能对谁产出什么成果"过滤 + 反向检验）与 verified V2 推出答案一致，E1 判停覆盖。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "年度总结只能说出一堆做过的事，说不出给谁带来了什么成果"命中 description 的述职场景与"重视勤奋忽略成果"失败模式（ce11）；预期（职务定义式 vs 贡献式回答、重写为受益者+成果）与 E1/E2 对应。 |
| should-trigger-03 | 会激活 | ✓ 通过 | "人际扯皮、靠和气维持、事情推不动"命中 A2 第 4 条与 R 段第三句引文（融洽 vs 成果）；预期用人际四项要求自检，与 E4 一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 涨薪话术是谈判与说服请求，description"薪酬谈判话术"明示不适用；B 段"贡献问句是自我要求与成果定向，不是邀功工具"同款排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 季度汇报"只报使用量还该报什么"已过贡献定向、要配比检查，description"要做三领域配比检查（用 three-domains-of-contribution）"明示分流；25 列表下 three-domains 描述逐字命中。 |
| edge-01 | 边界调用 | ✓ 通过 | 被边缘化两年："还谈贡献是不是自欺欺人"：B 段"处于明显被边缘化、存在结构性歧视或被挤压的环境……须先承认权力与机会分配的现实约束"覆盖预期（降为小尺度追问、不把结构挤压解释成个人不努力）。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 回炉记录：无。
