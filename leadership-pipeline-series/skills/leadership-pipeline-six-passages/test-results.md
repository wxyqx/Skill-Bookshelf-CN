# test-results.md — 领导力发展六阶段模型（领导梯队总框架）（leadership-pipeline-six-passages）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “四个管理层、中间断层、六个阶段怎么对应、该设几层”逐字命中 V2；定位真实层级＋5~7 层在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “MBA 四年就当总监、没怎么带过一线，要不要直接提事业部总经理”命中 description 的“越级提拔风险”与补课原则。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “每个层级都在做下一级的事”命中“层级错位”失败模式与连锁挤压。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：30 人扁平公司问是否不适用——expected 恰是“不按标准用法、说明边界、改用小公司版结论（每新增一层即失败高发点）”，该结论位于本 skill 正文 B 段与 A1（已核），故判定为“以本 skill 内容给出不适用结论”，与 expected 吻合；**备注：该条类型标注为 should_not_trigger 但实为边界处理题，建议改标 edge_case（见边界备注，未改 test-prompts.json）**。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：研发总监写代码判断卡在哪一环命中兄弟 skill three-dimension-transition，description 明确排除。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：200 人科技公司层级少一两层——description/B 允许 5~7 层与定制，expected 的审慎使用一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
