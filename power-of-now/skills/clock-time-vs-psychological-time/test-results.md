# test-results.md — 钟表时间 vs 心理时间判别（clock-time-vs-psychological-time）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程自测（fallback）** — 无独立 sub-agent 能力，主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判，判完对答案；混淆题用 19 个 skill 的 name+description 全量列表做选择。fallback 结果，可信度低于独立盲测。
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | "要不要公开检讨自己那次失误"=对过去处理方式的判别请求，description 的复盘场景与 verified.md V2 novel_question 直接对应；预期动作（教训=钟表时间应该做，自我清算=心理时间停止）与 E2 两栏拆分一致。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "要是当初……这个错误我放不下"命中过去向心理时间的列明信号（要是当初/guilt）；动作=两栏拆分+归档话术。 |
| should-trigger-03 | 会激活（附风险备注） | ✓ 通过 | "这样对吗？"是评估型提问，与 description"需要判断'这样用过去/未来正不正常'时调用"逐字对应；目标至上=description 列明的 trigger 变体（"等我……就好了"）。**风险备注**：waiting-state-exit 的"生活才开始"句式也命中本 prompt，属全批最模糊的双匹配边界；按 A2 定稿规则（评估型提问→判别器；已在途等待的煎熬→那边撤离程序）判归本 skill，且两者可先后接力，无论激活哪个都导出一致处理。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 日程安排是工具问题，无悔恨/自责/认同信号；B 段反场景（单纯的日程管理不适用）生效。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | prompt 自带诊断句"此刻我到底有什么问题？"——no-problem-in-now 的招牌装置逐字命中；本 skill 是长期判别器，不做当场存在性检查。 |
| edge-01 | 边界调用 | ✓ 通过 | 判定为"本 skill 只处理'使用过去的方式'，不处理'是否探究过去原因'（那是 no-understanding-the-past 的领域）；涉及创伤场景先提示专业支持"——与预期边界理由一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: should-trigger-03 是本次盲测中唯一的双匹配高危 case（本 skill vs waiting-state-exit）。处置：A2 的接力边界已在阶段 3 定稿时补强（"评估型提问走判别器；已在途等待走撤离；两者可接力"），未触发回炉。若接入 darwin-skill 后该 case 出现实测摇摆，优先复核此条。
- 回炉记录: 无。
