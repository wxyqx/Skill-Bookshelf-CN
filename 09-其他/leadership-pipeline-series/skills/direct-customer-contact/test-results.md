# test-results.md — 顾客直接接触法（未经过滤的第一手观察）（direct-customer-contact）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “B2B 满意度分数高但续约率在掉”逐字命中 V2 与 description“满意度高却留不住客户”。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “保不住原价、分销商与终端说法不一致”命中触发信号“毛利守不住”与过滤机制识别。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “问卷与焦点小组几轮结论都模糊”命中 description 的“问卷等间接信息”归因，安排现场接触。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：一线主管学会追问与落实计划命中兄弟 skill question-to-reality，A2 明确“同属未过滤信息家族但对象不同”。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：用年报做经营体检命中兄弟 skill company-panorama-seven-questions，description 明确区分（数字侧 vs 顾客现场侧）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：纯线上 SaaS 无门店——B 段“无法接触终端时须设计替代证据链”，expected 的改造形态一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
