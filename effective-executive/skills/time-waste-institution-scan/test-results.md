# test-results.md — 时间浪费的制度检修四项（time-waste-institution-scan）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "每到季末都要爆肝冲刺，去年也是这样……业务特性还是管理病"命中 description 的"重复危机"与 A2 第 1 条；预期用"可预见却重复=疏忽懒散"定性并给例行作业化/改规则两条出路，与 I/E 段一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "会议实在太多……是不是组织结构有问题"命中 description 的"会议太多"与 1/4 判据；预期追查职责重叠、优先组织归并而非会议技巧，与 E4 一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 "Hiring more people didn't help - we spend all day aligning and mediating conflicts"命中 description 的"协调内耗/too much coordination overhead"与 1/10 判据；预期给判据 + 查"偶尔才需要"的专家，与 I 段第二项一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 台风停电三小时是真正偶发事件，description"一次性偶发事故"直接排除；B 段"真正的偶发事件……不能强行例行化，那不经济也不现实"与 E1 判停互证。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "个人日程里塞满会和应酬，逐项判断该退哪些"是个人活动取舍，description"不适用于个人活动取舍（用 time-diagnosis-questions）"明示分流；25 列表下 time-diagnosis-questions 同样逐字命中。 |
| edge-01 | 边界调用 | ✓ 通过 | 急诊高峰拥挤：B 段"服务、创意、危机响应行业的'高潮迭现'可能确是业务特性……需要区分'可预见却复发'与'本质上不可预见的波动'"直接覆盖预期（对固有波动做能力设计而非消灭）。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 与 time-diagnosis-questions 的对偶核对：本 skill snt-02（个人日程）与三问 snt-02（季末冲刺）互为镜像诱饵，两条均按"对象是个人还是组织"正确分流，无交叉误接。
- 回炉记录：无。
