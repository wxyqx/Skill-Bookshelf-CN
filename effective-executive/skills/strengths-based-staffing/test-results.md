# test-results.md — 用人所长四原则（strengths-based-staffing）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "产出极高的技术大牛，脾气差、不服管教，要留他吗"命中 description 的"高产出但不服管"与 verified V2 原始问题；预期（三问筛选 + 让短处不产生作用 + 查"少不了某人"信号）与 E3/E4 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "两年换三个人都做不好，是不是去外面挖更厉害的"命中"某职位连续两三人失败"与第一原则硬判据（"必须重新设计职位，不要去找天才"）。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 "we can't do without him"命中 description 的"少不了他/indispensable"trigger；预期（三种坏信号 + 尽快调职 + 合规提示）与 I/E4 及 ce18 一致。 |
| should-not-trigger-01 | 边界处理（不进入本 skill 核心路径） | ✓ 通过 | "设计培训计划补沟通短板让他胜任管理岗"方向与本 skill"短处几乎不可改变、管理者的任务不是改变人"相反；B 段"本 skill 明确……不适用于设计改变性格与缺点的培养计划"直接排除该做法，并给出正确替代（评估长处与任务匹配 / 调整职位设计）。判定为"激活纠偏而非执行补短板"，与预期"不应激活核心动作、改为评估匹配或调整职位"一致。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "年终绩效面谈除了打分还能谈什么"是考评面谈，description"面谈考评（appraisal-four-questions）"明示分流；25 列表下 appraisal-four-questions 描述逐字命中。 |
| edge-01 | 边界调用 | ✓ 通过 | 虚报报销单：E5 判停"若在任一环节出现正直问题……跳过全部'长处/短处'权衡，按资格问题处理（参见 appraisal-four-questions）"与预期（资格否决 + 处置依程序）一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 近邻边界备注：与 appraisal-four-questions 的"事前择人 vs 在岗考评"分工经两向诱饵互测无交叉误接；与 use-your-own-strengths 的"他人 vs 自己"分工同样成立。
- 回炉记录：无。
