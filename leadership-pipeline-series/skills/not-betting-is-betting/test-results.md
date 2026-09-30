# test-results.md — 不下注本身就是一种赌博（not-betting-is-betting）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “要不要等竞品先发布、市场明朗再跟进”逐字命中 V2；把等待重新定价在 I/E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “三次会都要求再看一季度数据、怕犯错”命中“决策反复推迟要求更多数据”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “想立暂不进入却没人负责、没人写依据”逐字命中 description。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：还没搞清外部环境意味着什么命中兄弟 skill complexity-to-priorities（先想清楚再下注），description 明确先后。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：20 个改进项目砍到几个命中兄弟 skill priority-focus-three-to-four（选太多 vs 不敢选）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：成本数据两周可拿到——expected“可等（关键未知可低成本短期消除）”，E 段判停条件支撑。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
