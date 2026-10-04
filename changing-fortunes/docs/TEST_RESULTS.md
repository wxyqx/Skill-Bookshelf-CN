# TEST_RESULTS — 阶段 4 压力测试结果

> 测试方式：独立 sub-agent 盲测——盲测员未参与蒸馏，仅见全部 14 个 skill 的 name + description 与测试用例的 prompt 字面，做"14 选 1（含都不激活）"的判断；不参考 type / expected_behavior / notes。主流程再对照 test-prompts.json 判卷；每条用例的逐条判定见各 skill 的 test-results（判定理由存档于流水线 stage4/blind-A|B|C.md）。

## 总体结果

- **14 / 14 skill 通过**（minimum_pass_rate = 0.8，实际全部 100%）
- 84 条用例全部通过：should_trigger 42/42，should_not_trigger 28/28，edge_case 14/14
- **诱饵容错为 0**：should_not_trigger 无一误激活，全部正确拒答或正确指向兄弟 skill
- **同书兄弟混淆诱饵 24 条**（每条 should_not_trigger 中至少 1 条为"应触发兄弟 skill"的场景），全部正确指向兄弟 skill

## 兄弟混淆诱饵一览（24 条，全部通过）

| 本 skill | 混淆诱饵场景 | 正确指向 |
|---|---|---|
| commitment-device-design | 对手手握退路拖延谈判，如何逼其上桌 | eliminate-exit-leverage |
| commitment-device-design | 红线怕被试探，纠结精确公布还是模糊 | soft-commitment-ambiguity |
| confidence-fragility-check | 信心已动摇，设计一揽子联合干预 | strong-commitment-intervention |
| crisis-diagnosis-first | 已定性，问处置顺序对不对 | crisis-management-sequence |
| crisis-diagnosis-first | 以暂停偿付姿态逼对手打折 | unilateral-default-trap |
| crisis-management-sequence | 分不清缺现金还是还不起，先想怎么判断 | crisis-diagnosis-first |
| crisis-management-sequence | 暂停付息逼银行减值 | unilateral-default-trap |
| devaluation-accounting | 汇率高估，设计联合干预 | strong-commitment-intervention |
| eliminate-exit-leverage | 先联合老二老三再压老大的顺序 | negotiation-structure-design |
| eliminate-exit-leverage | 资金链紧张还威胁集体拖欠 | unilateral-default-trap |
| incentive-symmetry-check | 既要输出流动性又要维持信心 | triffin-dilemma-diagnosis |
| incentive-symmetry-check | 以停付威胁压价 | unilateral-default-trap |
| multilateral-coordination-assessment | 对方说没获授权不能拍板 | negotiation-structure-design |
| multilateral-coordination-assessment | 五国联合压低汇率的公报与规模设计 | strong-commitment-intervention |
| negotiation-structure-design | 撤掉免费维护逼对手回桌 | eliminate-exit-leverage |
| negotiation-structure-design | 评估协调机制有无实质成效 | multilateral-coordination-assessment |
| paradigm-failure-discipline | 设计一个让大家没法回头的机制 | commitment-device-design |
| soft-commitment-ambiguity | 喊话没人信，怎么让大家真信 | commitment-device-design |
| soft-commitment-ambiguity | 联合基金+同日声明的托底 | strong-commitment-intervention |
| strong-commitment-intervention | 说了没人信，怎么让大家相信决心 | commitment-device-design |
| strong-commitment-intervention | 汇率目标区怕精确数字被当靶子 | soft-commitment-ambiguity |
| triffin-dilemma-diagnosis | 改操作框架让自己没有退路 | commitment-device-design |
| triffin-dilemma-diagnosis | 单主体现金流断裂，先判流动性还是偿付能力 | crisis-diagnosis-first |
| unilateral-default-trap | 危机已爆发，问止血/重组/减债顺序 | crisis-management-sequence |

## 边界用例（14 条，全部给出符合预期的判定）

盲测员对 edge_case 的判断与 test-prompts.json 的 expectation 逐条核对一致，包括：应触发并执行判停纪律（eliminate-exit-leverage、commitment-device-design、incentive-symmetry-check、negotiation-structure-design、triffin-dilemma-diagnosis）、两个 skill 串联且顺序正确（strong-commitment-intervention → 先诊断；multilateral-coordination-assessment → 机制评估先行）、应先做前置检查再下结论（unilateral-default-trap 的依赖检查、soft-commitment-ambiguity 的敏感型判定）。
