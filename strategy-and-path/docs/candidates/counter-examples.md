# candidates/counter-examples.md — 反例提取器产出（阶段 1）

> 来源：《战略与路径》十二章。黄奇帆式警告多为"不能……""不是……而是……"与自认局限，是 B 段核心素材。

```yaml
- id: ce01
  title: 把结构性拐点当周期性波动硬扛
  type: counter-example
  source_chapter: 第六章
  source_quote: |
    "我们就知道当前房产商面临的困难并非短期的、周期性的，而是结构性、基础性的调整"——房企过去靠"房价只涨"思维定式盲目扩张。
  failure_mode: |
    把边界条件已触顶的结构性拐点误判为周期性回调，继续用老模式（加杠杆、囤地、赌涨价）硬扛，最终资金链断裂。
  mechanism: |
    周期波动可逆、会自我修复，扛过去就是机会；结构性拐点不可逆，扛的代价是清算。
    区分两者的工具（边界条件清单）缺失时，人会用最近一轮周期的经验外推。
  warning_signs:
    - "熬过这轮就好了"式的经验外推
    - 靠加杠杆维持旧模式
    - 说不清这次回调与上次周期的区别
  bound_to:
    - "边界条件分析法"
  tags: [counter-example, real-estate, misjudgment]

- id: ce02
  title: 激进去产能——"一夜之间淘汰旧系统"
  type: counter-example
  source_chapter: 第三章
  source_quote: |
    明言"中国不可能一夜之间把煤电机组全淘汰"，金融不能"谈煤色变"；清洁替代节奏"不能太激进"，否则电网与经济运行有风险。
  failure_mode: |
    转型期目标导向一刀切：为达减碳/升级目标同步拆旧建新，结果新系统未立稳、旧系统已拆除，系统崩溃（拉闸限电式后果）。
  mechanism: |
    大系统有惯性依赖，替代能力（调峰、备胎、供应链）的建设速度远慢于政治意愿。
    没有安全冗余的转型把可管理的风险变成系统性风险。
  warning_signs:
    - 以目标日期倒排退出时间表
    - 拿不出新系统容量的建成证据
    - 把"决心大"当"可行性"
  bound_to:
    - "先立后破节奏控制"
  tags: [counter-example, energy, transition]

- id: ce03
  title: 低估对手"损人不利己"的疯狂度
  type: counter-example
  source_chapter: 第十二章
  source_quote: |
    作者自认：低风险项指"全面发生的可能性"而非危害度——低风险项一旦发生危害反而最大（"金融核弹"）；SWIFT 对特定企业的精准打击现实存在、易成美方首选工具。
  failure_mode: |
    用"对方按成本收益行事"的理性假设排除极端情景，不做备胎（CIPS、自主芯片），极端情景真发生时被一剑封喉。
  mechanism: |
    成本收益分析在安全政治逻辑面前会失效——对手可能接受自损三千。
    低概率高危害项的防御不能靠概率论证取消，只能靠备份与威慑。
  warning_signs:
    - "对方不可能这么干，因为对他们也没好处"
    - 备胎系统长期停留在 PPT 阶段
    - 把概率低当成不用准备
  bound_to:
    - "兵棋推演式对抗分析"
    - "先立后破节奏控制"
  tags: [counter-example, geopolitics, tail-risk]

- id: ce04
  title: 以"倒逼改革"美化所有开放冲击
  type: counter-example
  source_chapter: 第九章
  source_quote: |
    作者自认：RCEP 可能加速低端产业向东盟转移；加入高水平协定面临六方面挑战（产业冲击、竞争加剧等）。
  failure_mode: |
    宣传口径把开放冲击一律说成"倒逼升级的动力"，不做受损群体与调整成本的分配分析，导致政策落地时遭遇真实阻力。
  mechanism: |
    自由贸易有净收益但分配不对称：受益者分散沉默、受损者集中有声。
    只算总账不算分配账的开放方案会在政治上翻车。
  warning_signs:
    - 论证只有收益没有受损方
    - 说不清谁承担调整成本、怎么补偿
  bound_to:
    - "滚雪球战略"
    - "源头治理思维"
  tags: [counter-example, trade, distribution]

- id: ce05
  title: 补贴驱动误当技术成熟
  type: counter-example
  source_chapter: 第三章
  source_quote: |
    200 万亿绿色投资被默认必然拉动增长，未讨论回报率与产能过剩（光伏、风电此前已两轮过剩）；"一拥而上、同质竞争、产能过剩"（第五章对地方产业政策的批评）。
  failure_mode: |
    把政府补贴/风口带来的繁荣当成技术与商业模式的成熟，一拥而上投资，产能过剩后一地鸡毛。
  mechanism: |
    补贴改变短期价格信号，使实际成本曲线与市场感知脱节；
    地方政府竞争进一步放大同质化投资。
  warning_signs:
    - 项目测算依赖补贴存续
    - 全行业都在扩产且产品同质
    - 度电成本/单位成本尚未越过在位方案
  bound_to:
    - "判断政策转向看相对成本而非财政动机"
    - "超大规模市场三效应"
  tags: [counter-example, subsidy, overcapacity]

- id: ce06
  title: 追求 100% 自给的"小而全"
  type: counter-example
  source_chapter: 第九章
  source_quote: |
    反"小而全"：绝不追求任何技术 100% 自给；日用消费品"并不一定要追求大包大揽、完全国产"。
  failure_mode: |
    安全焦虑驱动下追求全链条国产化，把有限资源撒在所有环节，关键环节反而投入不足，同时丧失国际分工收益与朋友圈。
  mechanism: |
    自给率是成本函数：越接近 100%，边际成本指数上升；
    而"被一剑封喉"的环节通常只占少数（高/中/低风险分级的价值）。
  warning_signs:
    - "全部国产化"式的口号
    - 自给清单不分关键与一般
  bound_to:
    - "绝不追求任何技术 100% 自给"
    - "兵棋推演式对抗分析"
  tags: [counter-example, self-reliance]

- id: ce07
  title: 线性外推式预测
  type: counter-example
  source_chapter: 第一章、第十一章
  source_quote: |
    80 万亿市值测算用"比例不变"线性外推，与自引的股市市值/GDP 50%-300% 波动区间自相矛盾；三大台阶时间表未预见增速中枢下移。
  failure_mode: |
    用单一比例关系或趋势线外推长期目标（股市市值、GDP 超越时点、收入占比），忽视均值回归与结构性变化。
  mechanism: |
    比例关系不是常数而是状态变量（作者自己引过 50%-300% 的波动区间），
    外推把"某一时点的快照"当成了"永恒规律"。
  warning_signs:
    - "若比例不变，则……"句式
    - 单点预测没有区间与情景
    - 10 年以上预测无敏感性分析
  bound_to:
    - "增速倍率法"
    - "长周期不会变判断法"
  tags: [counter-example, forecasting]

- id: ce08
  title: 用总量口号替代机制测算
  type: counter-example
  source_chapter: 第八章
  source_quote: |
    "每个要素市场一年产生 1 万亿红利、一年就多 5 万亿"是量级口号而非测算；国资划转 10-15 万亿实现 10% 年化回报过于理想化。
  failure_mode: |
    用"一年 N 万亿"的量级口号论证政策收益，不做分项测算，掩盖了落地阻力、市场容量与退出成本。
  mechanism: |
    量级口号把"理论上限"包装成"可兑现收益"；
    大数效应使听众失去校验能力（谁也无法直观感受 5 万亿意味着什么）。
  warning_signs:
    - 收益论证只有乘法没有分项
    - 回报率假设显著高于市场长期均值
    - 说不清红利的实现路径与时间表
  bound_to:
    - "黄奇帆五步分析法"
    - "改革三类型分类法"
  tags: [counter-example, quantification]

- id: ce09
  title: 遗产税式"重税出逃"
  type: counter-example
  source_chapter: 第七章
  source_quote: |
    遗产税等税率设计须统筹国际竞争，不能只看国内调节功能（法国 70% 遗产税致富豪外迁案例）。
  failure_mode: |
    在要素可跨境流动的条件下单边重税，结果是税基外逃——既没收到税，又赶走了税源。
  mechanism: |
    资本与人才的流动弹性远高于土地劳动；
    单边重税把"分配问题"变成了"外流问题"。
  warning_signs:
    - 税率/管制强度显著高于主要竞争辖区
    - 未评估要素外流的替代去向
  bound_to:
    - "征税面从窄、税负从轻"
    - "三次分配次序原则"
  tags: [counter-example, tax, capital-flight]

- id: ce10
  title: 官员诠释者的确定性口吻
  type: counter-example
  source_chapter: 全书（批判性提醒）
  source_quote: |
    "漂漂亮亮地完成""一定能做到"等确定性口吻淡化风险情景；"企业家听市场不听政客"近乎信仰，未考虑补贴、安全审查对企业激励结构的改写。
  failure_mode: |
    身处体制内诠释者位置时，把政策目标当预测结论，用确定性语言替代概率思维，读者若照单全收会误判风险。
  mechanism: |
    角色决定话语：背书者不能公开给目标打折；
    但市场决策需要的是概率分布而非目标函数。
  warning_signs:
    - 结论的确定性与论据的不确定性不匹配
    - 没有反事实检验（"如果错了会怎样"）
    - 引用者不加转换直接采信
  bound_to:
    - 所有本源 skill 的 Boundary 段
  tags: [counter-example, meta, bias]
```
