# test-results.md — 事业部副总经理四项关键业绩与四条警示（functional-vp-four-results）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “技术出身的营销副总怎么证明配得上头衔”逐字命中 V2；四项业绩逐项验收在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “工程副总泡实验室、不来往、销售有意见”命中“自我孤立”与“只重技术”两条警示。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “职能副总考核标准必须包含哪些业绩、要不要写培养接班人”命中高绩效组织含“至少一位本岗位接班人”。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：评估职能主管成熟度命中兄弟 skill functional-manager-maturity，description 明确排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：两岗位是否同一工作命中兄弟 skill job-essence-two-factors，A2 明确（业绩清单 vs 岗位本质）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：技术驱动公司高参与度——B 段“偶尔帮助并教会方法可取 vs 亲自解决大多数问题”限定语在案，expected 的审慎判定一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
