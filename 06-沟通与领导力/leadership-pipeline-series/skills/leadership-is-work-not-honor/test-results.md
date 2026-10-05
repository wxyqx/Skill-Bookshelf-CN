# test-results.md — 领导是一种工作而非荣誉；警惕自恋与诚信损耗（leadership-is-work-not-honor）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “骨干为冲业绩打擦边球怎么谈”逐字命中 V2；诚信硬门槛＋两问在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “很能干的同事要被推上管理岗但他犹豫、不知道当领导图什么”逐字命中 description 的“要不要接受这个管理岗位”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “is this what I actually want, or am I chasing the title” 命中触发词。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：同事失眠状态差命中“心理健康问题”，description 明确排除并转介。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：CEO 继任委员会与候选人面谈命中兄弟 skill ceo-selection-process，description 明确排除“组织层面的继任与选拔程序”。 |
| edge-01 | 不会激活（触发描述缺口） | ✗ 首轮不通过 → 回炉 | 首轮不通过：prompt 是“会议和和气气、决议反复推翻，我该忍还是走”的环境去留判断，正文 A2/B 已含“无效共治/环境裁决/去留判断”（已核），但 **description 未载任何环境或去留信号**——真实宿主只预载 name+description 时不会激活，属触发描述缺口。回炉：description 补入该信号（详见回炉记录）。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- **回炉记录**: 首轮通过 5/6；其中 1 条首轮不通过（见上表 ✗ 行）。
  - 根因：触发描述缺口——description 未载环境去留信号。
  - 修复（仅改 description，符合 methodology 06）：也用于判断“这个环境还值不值得留”（无效共治、决议反复、机制失灵时的个人去留选择）。
  - 复测：修后该条判定会激活/边界处理并与 expected_behavior 一致，复测通过；其余 5 条不受影响。
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
