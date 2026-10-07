# test-results.md — 从时间开始（know-thy-time）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "想记录一下时间，具体该怎么记才准"命中 description 的核心入口（时间记录规范）；预期（当时记、连续三四个星期、一年两三个时段 + 记录为被分析 + 下一步转诊断）与 R/E 段逐条对应。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "to-do list or a time log? Planning never seems to work"命中"计划 vs 记录"的起点排序，description 英文 trigger（time log / "should I plan first or log first"）逐字对应；预期回答即 I 段"不以计划为起点"。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 远程办公场景在 A2 第 4 条明列；"先测量一下我的时间到底去哪了"命中 description 主 trigger；预期（先采集 2–4 周原始记录 + 记忆不可靠提醒）与 E 段一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | App 推荐是工具选型，description"不适用于工具推荐与日程排版"直接排除；B 段同款排除（"用户要求工具选型……本 skill 给的是采样规范，不是工具清单"）。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "记录做完了"处在 description 明示的下游分流点（"记录已在手要逐项砍活动 → time-diagnosis-questions"）；25 列表下 time-diagnosis-questions 的 trigger（取消/授权）明显更贴近。 |
| edge-01 | 边界调用 | ✓ 通过 | 急诊科无记录时间：description"无时间自主权岗位可用，但须改按 B 段替代动作"；B 段强制声明给出"碎片式记录、只记录不受控时段、不做自责式结算"的降级版本，与预期一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 通用"时间管理技巧"误接核对（用户重点提醒项）：snt-01（App 推荐）为泛时间工具请求，description 与 B 段双重排除，未误接；另与 consolidate-free-time 的 snt-01（番茄钟设置）互证——时间类三个 skill 都不吃纯工具请求。
- 回炉记录：无。
