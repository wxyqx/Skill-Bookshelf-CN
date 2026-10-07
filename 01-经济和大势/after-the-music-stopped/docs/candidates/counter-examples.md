# candidates/counter-examples.md — 《当音乐停止之后》阶段 1 反例提取

```yaml
- id: ce01
  title: 雷曼周末的规则突变
  type: counter-example
  source_chapter: 第五、六章
  source_quote: |
    救贝尔斯登而弃雷曼——市场可在任何清晰规则下运行，不可承受的是规则被突然改写；雷曼破产当天美林转售美国银行。
  failure_mode: 在一致规则未建立时选择性救助：救贝尔斯登（牵连太多）弃雷曼（划底线），撕碎市场预期，把可控的机构倒闭放大为全面恐慌。
  mechanism: 市场参与者按"预期规则"定价；规则突变使一切对手方敞口不可定价，冻结所有交易。
  warning_signs: [救助标准前后不一, 官员公开划资金底线, 临近倒闭机构被区别对待]
  bound_to: ["救助决策框架"]
  tags: [counter-example, inconsistency]

- id: ce02
  title: WaMu 式恐慌期市场约束
  type: counter-example
  source_chapter: 第六章
  source_quote: |
    贝尔让 WaMu 债权人受损引发美联银行挤兑——十日债券从 73 美分跌至 29 美分。
  failure_mode: 在恐慌未平息时让债权人受损以示惩戒，引发相邻机构挤兑，惩戒变成传染加速器。
  mechanism: 恐慌期无法区分惩戒对象与无辜同类，市场约束的溢出远超设计者意图。
  warning_signs: [让债权人减损的新先例, 相邻同类机构融资成本跳升, 无事先规则预告]
  bound_to: ["恐慌与传染机制"]
  tags: [counter-example, market-discipline]

- id: ce03
  title: 8% 失业率承诺
  type: counter-example
  source_chapter: 第八章
  source_quote: |
    罗默-伯恩斯坦报告高估成效（失业率不超 8%），实际峰值 10%——"反事实论证（否则更差）无法说服公众"。
  failure_mode: 用最乐观模型做公开承诺，不及预期时整个政策被定性为失败，纵然反事实更差也无人听。
  mechanism: 公众只对照承诺与结果，不执行反事实推演。
  warning_signs: [承诺基于单一乐观模型, 未留误差区间, 对手可轻易证伪]
  bound_to: ["财政刺激设计", "政策的悖论与沟通"]
  tags: [counter-example, forecast]

- id: ce04
  title: 止赎政策的三位一体退缩
  type: counter-example
  source_chapter: 第十二章
  source_quote: |
    政府在巨额资金、产权变动、"救助失败者"政治污名这三位一体障碍前退缩，用廉价、复杂的计划敷衍——酿成经济复苏的最大瓶颈。
  failure_mode: 用小规模复杂计划敷衍本需大规模简单方案的问题（房主希望计划仅帮 1 人）。
  mechanism: 三重障碍叠加时，政治最优解是敷衍；但敷衍的经济成本（止赎螺旋拖复苏）远超正面解决。
  warning_signs: [计划规模与问题规模差数量级, 设计复杂化, 产出个位数]
  bound_to: ["政策失败三位一体"]
  tags: [counter-example, policy-failure]

- id: ce05
  title: 政策的悖论反噬
  type: counter-example
  source_chapter: 第十三章
  source_quote: |
    干预成功→施救者失去公众善意→政治反弹→削弱未来干预能力；佩尤民调仅 15% 知道 TARP 的钱基本收回（72% 认为大部分没还）。
  failure_mode: 成功的政策因解释失败被污名化，导致下一次危机"就现在来说，答案是否定的"——干预能力自毁。
  mechanism: 公众记忆保留愤怒、遗忘救助收回；政治激励惩罚解释者而非奖励成功。
  warning_signs: [救助认知与事实严重背离, 反救市候选人当选, 危机工具立法被威胁废除]
  bound_to: ["政策的悖论与沟通"]
  tags: [counter-example, political]

- id: ce06
  title: 技术官僚辩护的对称性缺陷
  type: counter-example
  source_chapter: 全书（作者方法的自反风险）
  source_quote: |
    作者身兼政策设计者与评分者：反事实推断（GDP+6%、就业+480 万）依赖模型假设无对照组；"可以原谅的错误"标准过宽——事后宽容＋事前无规则＝系统性道德风险。
  failure_mode: 亲历者用模型反事实自证成功，用"沟通失败"解释一切政治反弹，回避救助的分配后果与法治代价（强制注资、法卡斯式惩罚错位）。
  mechanism: 角色立场决定评估框架；技术成功标准（GDP/就业）遮蔽分配与程序维度。
  warning_signs: [评估者与被评估者同一, 反事实无对照, 批评被归为"沟通问题"]
  bound_to: ["所有本源skill的Boundary"]
  tags: [counter-example, meta]
```
