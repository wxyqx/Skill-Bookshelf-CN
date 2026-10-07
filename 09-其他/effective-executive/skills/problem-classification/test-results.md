# test-results.md — 问题四分类（problem-classification）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）** — 当前环境无独立 sub-agent 工具，按 methodology 06 降级条款由主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判（先隐藏 type / expected_behavior / notes，判完再对答案）；跨 skill 混淆题以 25 个 skill 的 name + description 全量列表做"该激活哪一个"的选择。**可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（且全部 should_not_trigger 必须通过，诱饵容错为 0）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "客服连续三个月同类投诉，每次单独赔礼道歉"命中 description 的"同类问题又来了"与 verified V2 原始问题；预期（第一类经常性问题 → 建规则根治 / 可预见重复例行作业化）与 I/E 段一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "生产线接头老是坏，修好又坏，是不是该换供应商"命中"表面各别实为经常"（书中管子接头案例原型）；预期（先假定经常性、分析根本原因、不逐起修理）与 I 段默认假设一致。 |
| should-trigger-03 | 会激活 | ✓ 通过 | "供应商合规审查规则，有人说就一次特殊情况别搞复杂，怎么判断要不要立规则"命中 description 的规则/个案选择与默认经常性假说（L1544）；预期（四分类定位 + 写明规则假定 + 预置验证复审）与 E2–E4 一致。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | "并购要完整审查框架，从问题定性到执行反馈都要"是全景五要素审计，description"定性已定后的决策程序（用 decision-five-elements）"（含"用户已明确卡在某个要素时直接用兄弟 skill"的反向引用）明示分流；25 列表下 decision-five-elements 描述命中。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | "退货规则三个月前定好、规则没问题，但门店执行不到位，怎么落地"卡点在决策后的行动承诺，description"已有明确规则只需执行"排除；25 列表下 decision-to-action 描述（"发了文件没人执行""谁来负责"）命中。 |
| edge-01 | 边界调用 | ✓ 通过 | "行业因新政策突然被整顿，算偶发还是经常"：B 段"四分类未覆盖'结构性政治问题'……可能把政治问题误判为技术问题"+ I 段"归类随证据修正的义务"覆盖预期（按第四类处理 + 明示可修正 + 承认政治维度）。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 双向诱饵核对：本 skill snt-01（并购框架）与 decision-five-elements snt-01（同类投诉）互为镜像，两条均正确分流（全景 vs 单要素）。
- 回炉记录：无。
