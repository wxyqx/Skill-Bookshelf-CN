# test-results.md — 商业智慧：六要素＋两基础总框架（business-acumen-six-elements）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “跳槽 SaaS 做 HR 怎么快速搞懂靠什么赚钱”逐字命中 V2；六要素逐项翻译＋两基础在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “各部门各说各话、有没有共同的生意语言”命中“竖井思维/共同语言”与驾驶比喻。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “给团队做商业扫盲、要够简单又够本质的框架”命中 description 的非财务人员场景，输出最小知识地图＋岗位翻译。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：查具体财务数字，description 明确排除“查具体财务数据”。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：两家 ROA 都是 15% 比质量命中兄弟 skill r-m-v-return-decomposition，description 明确排除。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：烧钱换用户的 App——B 段已内置“六要素对平台型/软件型不直接适用，须补现金流与单位经济”（已核），expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
