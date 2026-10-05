# candidates/counter-examples.md — 《繁荣与衰退》阶段 1 反例提取

```yaml
- id: ce01
  title: MFP 残差的循环论证
  type: counter-example
  source_chapter: 引言（作者方法的自反风险）
  source_quote: |
    MFP 是核算残差——把一切不可解释的增长归因"创新"，再以"创新"解释增长；19 世纪数据精度远不足以支撑 0.26 个百分点级别的结论。
  failure_mode: 用核算残差定义创新后，反过来以创新解释增长——循环论证；早期数据精度不足以支撑精细结论。
  mechanism: 残差包含一切未建模因素（结构变化、测量误差）；叙事连贯性被误认为因果识别。
  warning_signs: [关键概念由残差定义, 数据精度与结论精度不匹配, 反例被再解释吸收]
  bound_to: ["所有本源skill的Boundary"]
  tags: [counter-example, meta]

- id: ce02
  title: 奴隶制与资本主义的共生被悬置
  type: counter-example
  source_chapter: 第一、二章
  source_quote: |
    大通银行前身曾以逾 13000 名奴隶为抵押放贷；纽约银行与雷曼兄弟皆靠棉花牟利——奴隶制嵌入全球资本主义而非外在于它。
  failure_mode: "进步史"定调把奴隶制定性为"落后于时代的体制"，回避资本主义与奴隶制的共生关系与北方共谋。
  mechanism: 史观的道德重心决定哪些事实进入主叙事。
  warning_signs: [系统性暴力退为背景, 赢家史观, 道德成本被数据化悬置]
  bound_to: ["创造性破坏框架", "市场缔造的制度设计"]
  tags: [counter-example, history]

- id: ce03
  title: 翻案论证的不对等
  type: counter-example
  source_chapter: 第四章
  source_quote: |
    用油价下跌证明"没有欺骗公众"，却回避塔贝尔指控的回扣、情报贿赂等竞争手段——油价下跌与掠夺性手段并不互斥。
  failure_mode: 为翻案而选择有利证据（降价证据），忽略竞争手段的阴暗面；翻案与指控并不互斥却被处理成二选一。
  mechanism: 辩护性论证只收集己方证据。
  warning_signs: [只举证一方的证据, 对手指控被贴标签而非检验, 结论先于证据]
  bound_to: ["垄断的语境评估"]
  tags: [counter-example, evidence]

- id: ce04
  title: 权益挤出的恒等式嫌疑
  type: counter-example
  source_chapter: 第十二章
  source_quote: |
    权益支出与国内储蓄之和"惊人的统计稳定性"更可能是恒等式式的相关而非因果；用经常账户赤字融资的投资被轻描淡写。
  failure_mode: 把统计恒等式或强相关呈现为因果机制（福利挤出储蓄）。
  mechanism: 国民账户恒等式使两变量机械负相关；对照组缺失。
  warning_signs: [相关性接近完美, 忽略外部融资渠道, 结论服务于政策立场]
  bound_to: ["活力衰退诊断"]
  tags: [counter-example, causal-inference]

- id: ce05
  title: 美联储主席的自证回避
  type: counter-example
  source_chapter: 第十一章
  source_quote: |
    为格林斯潘任内低利率辩护过重（英国利率更紧房价照涨），回避自身监管责任——作者即前主席，利益相关。
  failure_mode: 当事人评估自身政策责任时选择性举证，把危机根源外包给"全球储蓄过剩"。
  mechanism: 角色立场决定归因方向；自证需求压倒对称检验。
  warning_signs: [作者与被评估政策直接相关, 对照案例挑选偏粗, 自身责任以外部因素解释]
  bound_to: ["所有本源skill的Boundary"]
  tags: [counter-example, meta]
```
