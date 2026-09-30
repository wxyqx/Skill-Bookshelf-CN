# test-results.md — 优先次序与"优后"（priority-and-posterior）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "老板要求五个重点项目都保持第一优先"命中 description 与 verified V2 原始问题；预期（全面优先=没有优先、四原则重排、逼出优后、压力偏差论据）与 I/E2–E3 一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "被紧急的事追着跑，季度最重要的事六周没动"命中 A2 第 2 条与 ce23 预警信号（重要不紧急连续多周被推迟）；预期（压力偏差识别 + 书面化优后 + 衔接 f13/f05）与 I 段机制及 E4 一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | "给团队定下半年重点，十二项都删不下去"命中 A2 第 3 条与 ce24；预期（困难在'优后'并需坚持 + 逐项四原则检验 + 时机代价）与 I 段操作要点一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "老产品线占着两个骨干、五年没增长，该不该关掉"是存量放弃判断，description"不适用于：某业务该不该放弃（用 abandon-yesterday）"明示分流；25 列表下 abandon-yesterday 描述命中。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "已确定死磕客户留存，但被打断拿不到连续时间，怎么保住整块时间"取舍已完成，问题在时间集中与防守；description 未列但 A2 区分（"f15 定次序、执行与防守走时间类 skill"）与 25 列表下 consolidate-free-time / one-thing-at-a-time 描述命中；本 skill 不激活。 |
| edge-01 | 边界调用 | ✓ 通过 | "没有资源调配权的产品经理能否自己定优后、宣布跨部门需求暂缓"：B 段"无权限的排序：'优后'决定须由有权限者做出——本 skill 可提供论据与压力偏差分析，但不假装用户能单方面暂缓组织级项目"与预期逐字一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 通用"优先级排序"误接核对（用户重点提醒项）：本 skill 的边界是"排序之后不再上排序 skill"（snt-02 正确让位于时间/串行类），且与 abandon-yesterday 的"该不该继续 vs 都值得做怎么排"经双向诱饵互测正确分流。
- 回炉记录：无。
