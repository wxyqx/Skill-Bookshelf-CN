# test-results.md — 控制机制三时点与免疫系统（control-three-points-immune-system）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “每天审批到深夜、越忙公司越乱”逐字命中 description 与 V2；审批量=控制缺位的反向指标在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “大授权后心里没底、怎么放权后仍知道底下在发生什么”命中“授权后怎么不出事”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “招聘失误＋报表瞒报”命中免疫系统的“病毒”清单（虚假汇报/压住事实，已核在文内）。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：视察行程与现场问什么命中兄弟 skill field-visit-protocol，description 明确“一线视察方法（用 field-visit-protocol）”。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：月度业绩讨论会命中兄弟 skill performance-dialogue-evidence，description 明确排除。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：强监管银行的刚性审批——B 段“不替代合规/监管要求”＋expected 的“剥离法定审批后再用框架”一致（记录：description 的“审批量即缺位”宜加行业限定语，见边界备注）。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
