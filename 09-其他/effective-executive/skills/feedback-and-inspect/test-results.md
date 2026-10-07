# test-results.md — 反馈制度与亲自视察（feedback-and-inspect）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "去年定的战略今天还成立吗？前提是不是已经变了"命中 description 与 verified V2 原始问题；预期（决策前反馈检验衡量方法 + 亲自查看 + 前提已变则抛弃/重做）与 I/E1–E5 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "考核指标用了好多年，总觉得哪里不对，是不是该换了"命中 description 的"衡量指标是不是失效了"；预期（决策前反馈、传统衡量方法反映昨天的决策、平均数/每公里事故率判例）与 I 段第 1 点一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 "The dashboards all look green, but I don't trust them. Should I get out and see for myself"命中 description 英文 trigger（get out and see / reports vs reality）；预期（安排亲自视察 / 指定独立现场检查人 + 报告不一定靠得住）与 I 段第 2 点一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "做月度项目进度看板、任务状态自动刷新"是运营跟踪与工具制作，description"日常执行进度跟踪与项目状态汇报"与 B 段同款排除逐字覆盖。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "双方都说自己有数据，怎么破"是见解与衡量标准的争论，A2 区分段"与 opinions-first 的区别：后者要求把见解当假设并先回答'相关标准是什么'"明确分流；25 列表下 opinions-first 描述逐字命中。 |
| edge-01 | 边界调用 | ✓ 通过 | "管内容策略，没有食堂可以去看，怎么亲自视察"：B 段"无现场可到的知识型决策（如内容策略、算法指标）：改用其他直接证据渠道，不要硬套'营长尝菜'"与 E3 判停（与使用者对话/走一遍用户路径/抽查原始样本）覆盖预期。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 近邻边界备注：与 boundary-conditions 的"前提检验机制 vs 抛弃条件"分工、与 opinions-first 的"衡量方法检验机制 vs 标准之争规则"分工均已互引并经双向诱饵互测。
- 回炉记录：无。
