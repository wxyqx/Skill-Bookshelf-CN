# test-results.md — 先"正确"后折中（correct-before-compromise）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "跨部门谈判，对方要求各让一步先落地，我该怎么让"命中 description 与 verified V2 原始问题；预期（先算正确方案 + 两类折中筛让步）与 I/E 段一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "写提案老想领导会不会反对，越改越软"命中 description 的自我审查型失败模式；预期（指出"一开头就问别人肯不接受"会阻止提出最重要的结论 + 恢复正确版本 + 核对担心的具体后果）与 I 段第 3 点及 E4 一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 "conceded three rounds... which concessions are still half a loaf"命中 description 的英文 trigger（half a loaf）；预期（边界条件逐条筛）与 I 段第 2 点一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "两家供应商互相压价、不图长期合作，怎么拿最低价"是零和立场博弈，B 段"双方没有共同目标、纯立场争夺的场合：本方法预设'存在一个满足边界条件的正确解'，利益零和的博弈要用谈判与联盟方法"逐字排除。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "产品数据报告没人看、同事说看不懂，怎么改交付方式"是交付形式设计，A2 区分段"本 skill 不是改形式，而是拒绝在目标上预支折中"明确分流；25 列表下 make-output-usable 描述逐字命中。 |
| edge-01 | 边界调用 | ✓ 通过 | "乙方算出正确方案又怎样，甲方根本不会听"：B 段"对无权者（基层、乙方）而言，算出'正确'之后仍可能被迫接受错误折中，方法只完成了'辨别'，没有提供'守住'的杠杆"与预期（写进内部记录与报价依据、区分可让与不可让、评估 BATNA）一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 近邻边界备注：与 make-output-usable 的"改形式 vs 改目标"分工经双向诱饵互测（本 skill snt-02 对倒 MOU snt-01）正确分流。
- 回炉记录：无。
