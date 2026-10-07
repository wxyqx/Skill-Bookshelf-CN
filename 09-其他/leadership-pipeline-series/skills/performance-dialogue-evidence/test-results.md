# test-results.md — 业绩讨论与证据法（performance-dialogue-evidence）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “季度复盘变念数据走过场”逐字命中 V2；证据二因素＋月度节奏＋活动陈述排除在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “下属汇报全是访问了多少客户”命中活动陈述排除清单与追问方式。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “担心被问凭什么这么评、怎么让年终等级自然显现”命中 description 的实录设计。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：从零建标准命中兄弟 skill performance-pipeline-interview-build，description 明确“没有标准先回建队流程”。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：员工状态差疑似心理问题——description 排除薪酬升降职，B 段亦要求转介专业资源；不激活本业绩方法。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：市场整体下滑三成而个人达标——expected 要求按“业绩＋环境背景”重判，I 段证据二因素原文支持。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
