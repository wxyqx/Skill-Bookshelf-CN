# test-results.md — 决策五要素（decision-five-elements）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "重大并购要一套系统的审查框架"命中 description 与 verified V2 原始问题；预期五要素逐条审计与 I/E 段一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "组织调整方案文件发了没人动，到底哪里出了问题"是决策推行失败的回查场景，A2 第 2 条措辞与之吻合（"开会定了但推不动/执行走样，要回查哪一环漏了"）；预期（重点核对要素四，回查谁了解/步骤责任人/能力匹配/衡量激励）与 E4 一致。**备注**：decision-to-action 是近邻候选（"发了文件没人执行"在其 trigger 列表中），本 skill 与它的分工为"诊断哪一环出错（本 skill 总审计）vs 已定位到行动环节的修复（DTA 专项）"——两 skill 的 description 与 A2 均已互引；本场按"回查哪一环"的措辞判给总审计并通过。 |
| should-trigger-03 | 会激活 | ✓ 通过 | "重大投资决策当时快速一致通过，现在想系统复盘"命中 A2 第 3 条（决策复盘）；预期五步回查 + 一致通过警觉（衔接 f23）+ 要素二抛弃判断与 E 段及 B 段配套警戒一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "客服连续三个月同类投诉，每次单独处理，该怎么定性"是单一要素（问题性质）深挖，description"问题定性用 problem-classification"明示分流；25 列表下 problem-classification 描述逐字命中。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "十个小毛病要不要大改造"前置问题是"是否需要决策"，description"日常小决定（用 decide-and-act-fully 判断是否需要决策）"明示分流；25 列表下 decide-and-act-fully 描述命中。 |
| edge-01 | 边界调用 | ✓ 通过 | "工厂半夜爆裂事故，当场决定停线还是换线"：B 段"危机响应中的即时决策……不适用完整程序"（含德鲁克"宽松时间"自述）与预期（先按预案拍板、事后复盘与制度修正回到五要素/问题分类）一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 通用"决策技巧"边界核对（用户重点提醒项）：snt-02 按"是否需要决策"让位于 decide-and-act-fully；三例 should_trigger 均为重大/程序性决策，无一条是日常小决定或纯咨询话术。
- 回炉记录：无。
