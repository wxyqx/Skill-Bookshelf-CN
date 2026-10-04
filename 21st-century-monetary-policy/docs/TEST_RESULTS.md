# TEST_RESULTS — 阶段 4 压力测试结果

> 测试方式：独立 sub-agent 盲测——盲测员未参与蒸馏，仅见全部 16 个 skill 的 name + description 与测试用例的 prompt 字面，做"16 选 1（含都不激活）"的判断；不参考 type / expected_behavior / expectation / notes。主流程再对照 test-prompts.json 判卷；每条用例的逐条判定见各 skill 的 test-results.md（盲测原始记录存档于流水线 stage4/blind-A|B|C.md）。

## 总体结果

- **16 / 16 skill 通过**（minimum_pass_rate = 0.8，实际全部 100%）
- 96 条用例全部通过：should_trigger 48/48，should_not_trigger 32/32，edge_case 16/16
- **诱饵容错为 0**：should_not_trigger 无一误激活，全部正确拒答或正确指向兄弟 skill
- **同书兄弟混淆诱饵 30 条**（should_not_trigger 中点名兄弟 skill 的场景），全部正确指向兄弟 skill
- **edge_case 逐条核对**：盲测判断与 expectation 的精细预期全部吻合，包括"本 skill 定位后转出 announcement-as-policy"（panic-contagion-template）、"组合属性识别"（bagehot-stigma-design）、"默认不激活"（political-feasibility-engineering / stop-go-discipline）、"激活但克制使用/结论反向"（preemptive-strike-policy / signal-engineering / credibility-capital-management）

## 兄弟混淆诱饵一览（节选，全部通过）

| 本 skill | 混淆诱饵场景 | 正确指向 |
|---|---|---|
| preemptive-strike-policy | 紧缩期想松手、坚持还是放弃 | stop-go-discipline |
| credibility-capital-management | 政策行动的戏剧性形式设计 | signal-engineering |
| signal-engineering | 宣布本身的稳定效应 | announcement-as-policy |
| commitment-spectrum-design | 指引措辞的可信度支柱 | guidance-credibility-design |
| guidance-credibility-design | 门槛式承诺的日历绑架 | commitment-spectrum-design |
| policy-firepower-accounting | 尾部风险的保险性放松 | risk-management-insurance |
| panic-contagion-template | 已定性后的救助程序设计 | bailout-three-step-program |
| bailout-three-step-program | 先定位恐慌环节再谈救助 | panic-contagion-template |
| bagehot-stigma-design | 救助的逐案条件设计 | bailout-three-step-program |
| monetary-fiscal-boundary | 救助工具与条件的匹配 | bailout-three-step-program |
| stop-go-discipline | 长时滞下的提前行动 | preemptive-strike-policy |

## 边界用例要点（16 条，全部符合预期）

边界用例专门检验 skill 不被机械套用：框架"可用但结论不预设"（risk-management-insurance 核算保费后可能不买）、"结构同构但前提不成立"（commitment-spectrum-design 的个人承诺场景）、"前提被证伪的转向不是摇摆"（stop-go-discipline）、"宣布的信誉前提"（announcement-as-policy 拒绝不可兑现的承诺）、"技能组合识别"（bagehot-stigma-design 与 announcement-as-policy 的公告式工具）。
