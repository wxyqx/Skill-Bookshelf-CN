# test-results.md — 两次臣服机会（two-surrender-chances）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程自测（fallback）** — 无独立 sub-agent 能力，主流程模拟"只加载本 SKILL.md 的全新 agent"逐条盲判，判完对答案；混淆题用 19 个 skill 的 name+description 全量列表做选择。fallback 结果，可信度低于独立盲测。
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | 上午突然被裁+"天塌了"+手抖="厄运落地、既成事实"首场景（verified.md V2 novel_question）；预期完整序列（定级→第一机会清单→情绪压倒转第二机会→危机判停）与 E1-E6 逐项对应。 |
| should-trigger-02 | 会激活 | ✓ 通过 | "知道该接受现实但我真的做不到"=两级程序的标志句式（判停 B：接受不了→直转第二机会，不强迫想通）；后续怨恨检查与 present-forgiveness 的交接在 A2/E 段有支撑。 |
| should-trigger-03 | 会激活 | ✓ 通过 | 丧亲+everyone tells me to accept+I feel nothing：厄运级场景命中（亲人离世在 description 清单）；"feel nothing"按 B 段/I 段识别为可能的情感切断而非臣服（"切断你的感受并不是臣服"），并说明哀伤自然进程与专业支持选项——不强行转化哀伤。 |
| should-not-trigger-01 | 不会激活 | ✓ 通过 | 日常人际冲突+"就当接受现实吧"的话术有假接纳嫌疑——既非厄运级也非真接纳；全列表下 fake-acceptance-alert / non-reactive-no 更合适（B 段"慢性日常不满不到厄运级"反场景生效）。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 事实仍可改变（提条件/申请调岗）→判停 A 转行动线（accept-then-act）；本 skill 待命不抢跑"接受"话术。 |
| edge-01 | 边界调用 | ✓ 通过 | 判定为"激活完整两级程序：第一机会承认'病已确诊'并配合治疗（医疗决策遵医嘱），第二机会向恐惧与悲伤的感受臣服；崩溃大哭是正常哀悼而非失败；情绪持续恶化建议心理支持"——与预期的三者叠加判断一致。 |

## 通过率与结论

- **通过 6/6 = 100%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- 边界备注: should-not-trigger-01 的判据（日常级+假接纳嫌疑双重排除）依赖全 skill 列表比对，是本 skill 通过的关键诱饵；与 accept-then-act 的量级分界（日常 vs 厄运）在双方 A2 均已写明。
- 回炉记录: 无。
