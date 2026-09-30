# test-results.md — 绩效考评四问（appraisal-four-questions）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "下周年终绩效面谈，下属技术强但沟通差、老跟产品吵架"命中 description 的"年终面谈"与 verified V2 原始问题；预期（四问面谈提纲、沟通问题作为"限制"附带处理）与 I/E3 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "公司让我盘点高潜，HR 表格让打潜力分，总觉得哪里不对"命中 description 的"高潜盘点"与 p41 并入的"不评潜能"主张；预期（潜能不可评估、只评绩效、改为期望贡献对照）与 I 段一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | "报销做过手脚、让新人背锅，要不要继续用、要不要提主管"命中 description 的正直否决触发（第四问）；预期（资格否决 + 不进入容忍换算 + 依程序）与 I/E4 一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "招海外市场负责人，前两任都崩了，怎么重新设计职位和招聘标准"是事前择人与职位设计，description"招聘选人与职位设计（用 strengths-based-staffing）"明示分流；25 列表下 strengths-based-staffing 描述（职位连续两三人失败即重设）命中。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "自己忙却看不到成果，想盘一盘自己擅长什么、怎么调整工作方式"评估对象是自己，description"自我评估（用 use-your-own-strengths）"明示分流；25 列表下 use-your-own-strengths 的描述（"该不该争取这个岗位""我到底擅长什么"）命中。 |
| edge-01 | 边界调用 | ✓ 通过 | 明星员工"我脾气就这样"：预期要求区分"脾气/风格属短处"与"行为具体表现为不正直才升级第四问，并先要具体行为事实"。B 段"正直否决不设防滥用机制……使用时须以具体行为事实为依据"＋I 段"短处靠组织手段让短处不产生作用"共同覆盖该判断。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 近邻边界备注：与 strengths-based-staffing 的双向诱饵（本 skill snt-01 对倒 SBS st-02）互测正确分流；正直类问题在 SBS edge-01 与本 skill st-03 双侧处理一致（都指向资格否决 + 依程序）。
- 回炉记录：无。
