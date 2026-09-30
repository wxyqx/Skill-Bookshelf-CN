# test-results.md — 贡献三领域（three-domains-of-contribution）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "新成立的内部平台团队，季度汇报只报使用量感觉不完整"命中 description 的"季度汇报该报什么"与 verified V2 原始问题；预期（三条线 + 权重说明）与 E1–E4 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "几十年只看营收，老员工退休没人接班"命中 description 的"无人接班"与 A2 第 2/4 条；预期（第三条线为零 + 落成具体机制而非政策文件）与 A1 案例 2 判语"仅有政策是没有用的"一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 "values in the handbook, but everyone says the standard is just 'hit the number'"命中"价值观/values"trigger 与"价值观必须像直接成果一样可被检验"的核心逻辑（I 段第二线）。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 财务 KPI 拆解表是指标分解任务，description"不适用于……财务审计与 KPI 拆解"逐字排除；B 段"把三领域当作 KPI 清单强制打分"为反面使用，进一步封死。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "迷茫，不知道能贡献什么"尚未完成贡献定向，description"不适用于：尚未完成贡献定向（用 contribution-question）"明示分流；25 列表下 contribution-question 描述逐字命中。 |
| edge-01 | 边界调用 | ✓ 通过 | 公立医院三目标："算不算三种直接成果"：E1 判停（"若一句话里混着三种互不相同的成果，先做取舍或明确主次"）+ B 段"谁的价值观未讨论"覆盖预期（区分冲突的直接成果 vs 价值观承诺、承认政治必然）。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 回炉记录：无。
