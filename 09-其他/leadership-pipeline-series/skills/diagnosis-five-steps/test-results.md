# test-results.md — 个体与组织诊断五步/四步法（diagnosis-five-steps）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “执行力差、想找出哪个人的问题”逐字命中 V2；先看工作再看人＋五步取证在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “每层都有问题、说不清卡在哪层”命中组织诊断四步与“按层汇总定位阻滞”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “高潜明星越提拔越出问题、360 反馈差、想先搞清缺什么”命中 description 的个体五步与培养计划产出；千人教练案例在 A1。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：判断卡在技能/时间/理念、要快速自检命中兄弟 skill three-dimension-transition，description 明确排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：拿诊断结论作降职劝退依据——expected 要求边界声明（仅作发展对话输入＋劳动法边界），B 段伦理边界支撑，判定一致（边界判定）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：50 人小组织简化——expected“保留三条底线、压缩为抽查”，A2/B 按组织定制在案。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
