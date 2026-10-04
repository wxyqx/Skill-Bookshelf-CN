# candidates/counter-examples.md — 《分析与思考》阶段 1 反例提取

```yaml
- id: ce01
  title: 宝能式六工具叠加
  type: counter-example
  source_chapter: 第1讲
  source_quote: |
    70亿万能险经高息揽储、资金池、错配、通道、嵌套放大至450多亿购万科25%——杠杆被工具层层黏结放大。
  failure_mode: 用合规外衣的金融工具层层嵌套，把小资本放大成大杠杆，一旦底层资产波动即全线击穿。
  mechanism: 每一层工具都让资金"名实分离"，穿透监管跟不上嵌套速度；杠杆是乘法不是加法。
  warning_signs: [多层通道, 优先劣后嵌套, 收益率显著高于无风险利率]
  bound_to: ["金融乱象六工具识别"]
  tags: [counter-example, leverage]

- id: ce02
  title: 蚂蚁式 ABS 高频循环
  type: counter-example
  source_chapter: 第1讲
  source_quote: |
    30多亿资本金循环发ABS 40次形成3600多亿放贷、上百倍杠杆——资本金对风险的覆盖被循环架空。
  failure_mode: 把证券化当无限杠杆机器，循环次数失控使名义资本金与真实风险敞口脱钩。
  mechanism: 每次循环把同一信用重新包装出售，风险并未出表，只是记在了看不见的地方。
  warning_signs: [循环次数无上限, 杠杆数十倍, 资本金与放贷规模比例悬殊]
  bound_to: ["数字信贷五原则", "ABS循环纪律"]
  tags: [counter-example, fintech]

- id: ce03
  title: P2P 庞氏结构
  type: counter-example
  source_chapter: 第3讲
  source_quote: |
    P2P注册上万家、近万亿元坏账；众筹资本金、向网民高息揽储、无场景放贷、资金池——五个机制都是违规的。
  failure_mode: 无资本金、无场景、无监管的"三无放贷+资金池"必然滑向庞氏。
  mechanism: 借新还旧的流动性幻觉掩盖信用风险，规模越大崩盘越烈。
  warning_signs: [承诺高收益保本, 无明确资金用途, 线上高息揽储]
  bound_to: ["P2P式伪金融五重违规机制"]
  tags: [counter-example, ponzi]

- id: ce04
  title: 广场协议式汇率急变
  type: counter-example
  source_chapter: 第4讲（回顾）
  source_quote: |
    1971年美国单方面停止美元兑换黄金，布雷顿森林体系崩溃——无锚货币时代开启；美国债务违约方式是贬值与通胀。
  failure_mode: 货币无锚滥发+隐性违约（贬值通胀）是储备货币国转嫁债务的惯用路径，持有人承担铸币税反向收割。
  mechanism: 主权信用无硬约束时，财政压力最终由货币持有人分摊。
  warning_signs: [政府债务增速持续超收入增速, 实际利率为负, 财政货币化言论升温]
  bound_to: ["主权信用货币的刚性纪律"]
  tags: [counter-example, currency]

- id: ce05
  title: 监管同频共振
  type: counter-example
  source_chapter: 第14讲
  source_quote: |
    一个病人如果有四种病，四个外科医生同一天动手术，好人也被开刀开坏了——一刀切、层层加码、同频共振。
  failure_mode: 多部门同时收紧、各级放大强度，使本来可管理的风险调整变成系统性踩踏。
  mechanism: 每级加码看似安全边际，叠加后是矫枉过正；金融是连续系统，急刹最危险。
  warning_signs: [多部门同月发文, 基层执行强度远超文件原意, 行业流动性骤然枯竭]
  bound_to: ["监管三反模式"]
  tags: [counter-example, regulation]

- id: ce06
  title: 美国脱实就虚的教训
  type: counter-example
  source_chapter: 第13讲、第12讲
  source_quote: |
    美国GDP中85%来源于以金融为中心的服务业，制造业只占11%；金融业属于精英产业，华尔街总共才吸纳30万人就业。
  failure_mode: 制造业占比过低+金融业占比过高（7-8% 阈值）的经济体，危机通过金融放大而非吸收。
  mechanism: 金融业增加值占比超 7-8% 历史上多以危机出清回归 5-6%；就业吸纳差加剧贫富分化反噬消费。
  warning_signs: [金融业增加值占比逼近8%, 制造业占比快速下滑, 贫富分化扩大]
  bound_to: ["宏观杠杆四指标", "制造业占比红线（书架已有）"]
  tags: [counter-example, structure]

- id: ce07
  title: 散户市的波动结构
  type: counter-example
  source_chapter: 第7讲
  source_quote: |
    散户持股市值占25%却贡献80%交易量；公募13万亿中仅2万亿入市——机构也"散杂小"，2015配资踩踏、2016熔断。
  failure_mode: 无长期资金压舱石的市場高波动常态化，制度缺陷（退市、发行）被短期政策工具反复对冲。
  mechanism: 短钱主导定价→波动→监管救市→预期扭曲的闭环。
  warning_signs: [换手率畸高, 政策市预期, 年金保险占比过低]
  bound_to: ["资本市场三功能诊断", "长期资金压舱石原则"]
  tags: [counter-example, stock-market]

- id: ce08
  title: 概念泛化不可证伪
  type: counter-example
  source_chapter: 第2讲（作者方法的自反风险）
  source_quote: |
    把一切成功改革追溯性归入"供给侧结构性改革"——概念泛化到不可证伪；"十条共几万亿红利"是拉弗式推算（恰是作者批评供给学派之处）。
  failure_mode: 好框架被过度扩张后失去预测力；用自己反对的推算方式论证自己的主张。
  mechanism: 事后归因+大数口号让框架免于检验。
  warning_signs: [框架解释一切, 收益测算只有乘法, 无失败案例讨论]
  bound_to: ["所有本源skill的Boundary"]
  tags: [counter-example, meta]
```
