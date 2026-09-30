# test-results.md — 继任计划：新定义、四原则与五步骤（succession-five-steps）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “只有我一个人在操心接班人、怎么变成制度”逐字命中 V2；五步骤＋审核节奏在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “建了高潜人才库名单却没人可用、关键岗位靠空降”命中 description 的“人才库怎么建/纸上名单”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “succession across all levels / replacement planning for the CEO” 命中触发词。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：CTO 下月走的交接清单——description 明确排除“临到换人前 30 天的应急找人”。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：判断某个人属于哪种潜能命中兄弟 skill potential-three-types，A2 明确（制度 vs 单点判据）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：60 人三层公司——A2/B 小公司裁剪（压缩层级、保留标准＋评估＋年度审核核心），expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
