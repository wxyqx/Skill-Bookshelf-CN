# test-results.md — 潜能三分类：转型/成长/熟练（potential-three-types）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “老员工绩效一般但从不出错、怎么评价”逐字命中 V2；三类潜能＋证据规则在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “评选年度高潜名单、要更细更能说服人的分类”命中对“高潜/非高潜”二分的替换主张。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “is he promotable” 命中触发词；输出“哪类潜能＋证据＋时间窗”。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：销售提成规则设计属薪酬规则，与潜能判定无关，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：九宫格填格与每格处理命中兄弟 skill nine-box-actions，description 明确（潜能轴是输入、矩阵另有专 skill）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：错层者的潜能上报——expected“先归位再评估（绩效证据被错配污染）”，B 段“无连续绩效记录不可分类”支撑。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
