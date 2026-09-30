# test-results.md — 时间诊断三问（time-diagnosis-questions）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | 微信群与例行会"怎么判断哪些可以直接退出"命中 description 的逐项裁决场景；A2 第 1 条（群/会/委员会/应酬）明列；预期三问分别指向删/转/问相关人，与 I/E 段一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "delegate without it looking like I'm dumping my own work"命中 description 的"授权/delegate"trigger 与"授权正解"这一问；预期先纠正语义再逐项筛选，与 I 段第二问一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | "记录做完了，想每一条都判断一下该不该继续做"是该 skill 的标准入口（前置于 know-thy-time 之后）；预期给出三问清单 + 完成标准 + 删减风险提示，与 E 段对应。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 写拒绝邮件是执行类写作请求，description"不适用于……只差写一封拒绝邮件"逐字排除；B 段"先判据后执行"同款声明。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 季末爆肝冲刺的"业务特性还是管理病"是制度病灶问题，description"怀疑是制度病灶（用 time-waste-institution-scan）"明示分流；25 列表下 time-waste-institution-scan 的描述（重复危机/可预见却复发）逐字命中。 |
| edge-01 | 边界调用 | ✓ 通过 | 合规检查想用"不做会怎样"砍掉：B 段明确"三问的前提是'对成果无影响的非生产性活动'，法定/合规/安全义务有明确后果，不属于可取消项"；预期为守边界并引导改用第二问或改进执行方式，与 B/E 段一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 通用时间管理误接核对：本 skill 的三个 should_trigger 全部是"活动逐项裁决"（含群聊、授权、记录在手），无一条是纯工具或通用效率问题；工具类诱饵由同类 skill 承接排除。
- 回炉记录：无。
