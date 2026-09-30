# test-results.md — 一次只做一件事（one-thing-at-a-time）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "三个项目全延期，先砍哪个先救哪个"命中 description 主 trigger 与 verified V2 原始问题；预期（问题在并行本身 + 保留唯一要事 + 提示搁置≈取消）与 I/E3 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "日程排满、晚上十点才有空，最重要的方案一个字没写"命中"重要的事一直没时间"信号；E2 判停（碎片化是主因则衔接 consolidate-free-time）与预期一致，"修正估算不足/赶工"在 E5。 |
| should-trigger-03 | 会激活 | ✓ 通过 | "三个'公司最高优先级'项目，哪个都推进不下去"命中 A2 第 3 条（组织把多个最高优先级同时压来）；预期（全优先=没优先、要求搁置声明）与 I 段及 ce24 交叉一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "想先记录两周时间，看看时间花哪了，然后清理浪费"是时间资源侧（记录+清理），description"不适用于：时间记录与合并整块（用 consolidate-free-time）"明示分流；25 列表下 consolidate-free-time / know-thy-time 均更贴近。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "老产品线微利占着两个骨干，该不该关掉、人手从哪来"是存量放弃，description 未列但 A2 区分段明确"f14 是删掉不该继续的过去（减存量）；本 skill 是串行"；25 列表下 abandon-yesterday 描述（旧产品没前途还舍不得停）命中。 |
| edge-01 | 边界调用 | ✓ 通过 | 急诊科当班："根本不可能一次只做一件事"——B 段"值守型/响应型岗位……本质上要求并行响应，'一次只做一件事'只适用于其中的'要事'"与预期（事务队列不适用、要事层仍可用、不得指责一线不专注）逐条一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 近邻边界备注：与 consolidate-free-time 的"任务侧 vs 时间侧"分工经两向诱饵互测（本 skill snt-01 对倒 CFT snt-02）正确分流；与 abandon-yesterday / priority-and-posterior 的"减存量 / 排序 / 串行"三分工明确。
- 回炉记录：无。
