# test-results.md — 企业/集团职能主管：六关系点与角色重定义（corporate-function-six-relations）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “刚接任集团 HR 负责人、集团高管与公司 HR 双线、还要面对事业部总经理”逐字命中 V2；六关系点在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “职能主管天天救火、对谁都不敢说不、价值说不清”命中未尽职三标志与角色重定义。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 英文 “matrix reporting / business GM and functional boss want opposite things” 命中关键信号。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：HR 共享服务中心的流程与编制属职能内部运营设计，无多关系点定位诉求，不激活。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：架构师不想做管理、想留人命中兄弟 skill dual-track-management-technical，description 明确排除。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：150 人无矩阵结构——expected“退化为直接上司＋内部客户＋下属的三关系简化版”，A2/B 的裁剪主张支撑。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
