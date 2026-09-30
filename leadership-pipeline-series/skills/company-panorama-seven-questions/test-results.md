# test-results.md — 公司全景诊断七问（用年报数据做全局体检）（company-panorama-seven-questions）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “第一次尽调怎么快速上手、看经营全貌”逐字命中 V2；七问＋只用公开数据＋店主式全景在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “技术出身总监看财报像天书、销售和财务各说各话”命中“看不懂财报/没有共同语言”。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “对公司管理层提几个尖锐问题、不知问到点上”命中“不知道该向管理层问什么”；输出追问方向。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 诱饵：保不住原价、渠道与终端说法不一——症结在顾客/消费者二分与现场取证，兄弟 skill direct-customer-contact 的描述含“毛利守不住”，对标下本 skill 不激活（紧诱饵，见边界备注）。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：200 个指标里挑最重要的几个命中兄弟 skill priority-focus-three-to-four（取舍纪律而非体检清单）。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：未上市粗数据——E 段判停“关键数据不可得时用替代指标并声明”，expected 一致。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。
