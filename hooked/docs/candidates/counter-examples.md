# candidates/counter-examples.md — 反例提取器产出

> 提取器: counter-example-extractor（串行降级执行，"干净视角"独立跑完：只找失败模式 / 反例 / 陷阱）
> 全书上下文: 见 BOOK_OVERVIEW.md；出处按 fulltext.txt 实际章节与行号标注。
> 本阶段不做筛选，宁错杀，交给阶段 1.5 三重验证。每条含 failure_mode 与 mechanism。引用 ≤150 字。

```yaml
- id: ce01
  title: "黑暗模式"滥用人际型触发
  type: counter-example
  source_chapter: 第2章（L616）
  source_quote: |
    "有些商家利用'黑暗模式'将人际型触发和病毒式循环应用在不道德的信息传播中。……这种
    做法一开始会带来一定的收益，但代价却是失去用户的信任与期望。"
  failure_mode: 用恶意程序引诱用户把朋友拉进社交网站，透支社交关系换短期增长。
  mechanism: 人际触发依赖信任存量；被邀请者一旦察觉自己被"套路"，愤怒与失望会同时
    摧毁邀请者与被邀请者对产品的信任，病毒循环变成负循环。
  warning_signs:
    - 邀请流程对被邀请方不透明
    - 用户分享后表达尴尬或道歉
    - 增长依赖持续加大诱导力度
  bound_to:
    - "人际型触发"
    - "保障用户自主权"
  tags: [counter-example, dark-pattern, trust]
```

```yaml
- id: ce02
  title: 回馈型触发的昙花一现
  type: counter-example
  source_chapter: 第2章（L604–606）
  source_quote: |
    "回馈型触发所引发的用户关注往往是昙花一现。要想利用回馈型触发维持用户的兴趣，
    企业必须让自己的产品永远置于聚光灯下，这无疑是一项艰巨而又前景莫测的任务。"
  failure_mode: 把媒体报道/应用商店推荐带来的流量高峰误判为习惯形成，团队随之扩张。
  mechanism: 回馈型触发的注意力来自平台分发而非用户动机，聚光灯移走即归零；且"永远
    置于聚光灯下"不可控、不可预算。
  warning_signs:
    - 增长曲线与媒体事件完全同构
    - 无媒体期留存断崖
    - 团队按峰值配置资源
  bound_to:
    - "外部触发四分类"
    - "自主型触发是习惯的必要条件"
  tags: [counter-example, trigger, growth]
```

```yaml
- id: ce03
  title: 付费型触发的长期依赖
  type: counter-example
  source_chapter: 第2章（L598–600）
  source_quote: |
    "付费型触发能够有效地拉拢用户，但是代价不菲。……假如 Facebook 或者 Twitter 要靠
    打广告来触发用户，那可能过不了多久就会资不抵债。靠花钱来拉拢回头客不是长久之计。"
  failure_mode: 用广告购买维持用户打开率，把营销预算当成产品黏性的替代品。
  mechanism: 付费触发只购买曝光不建立情绪绑定；一旦停投，行为频率回落——因为它没有
    生成内部触发，也没进入习惯循环。
  warning_signs:
    - 停投即流失
    - 获客成本长期高于用户终身价值
    - 回访高度依赖推送预算
  bound_to:
    - "外部触发四分类"
    - "外部触发的终局是被内部触发取代"
  tags: [counter-example, paid-acquisition]
```

```yaml
- id: ce04
  title: 旧习惯的回转（后进先出）
  type: counter-example
  source_chapter: 第1章（L395–399）
  source_quote: |
    "在接受过戒酒治疗的嗜酒者中，约有 2/3 的人会在一年之内重拾旧习。另有研究显示，通过
    节食减肥的人几乎无一例外地在两年之内再度发胖。……最新收获的东西往往最先失去。"
  failure_mode: 以为行为改变一次即宣告成功，忽视旧神经通路随时可能重新激活。
  mechanism: 大脑"后进先出"：新习惯在旧通路未消亡时建立，压力或情境回归时旧行为先
    复活；习惯替换是长期防御战而非一次性事件。
  warning_signs:
    - 改变后未设防复发机制
    - 情境（压力/场所）恢复原状
    - 以单次成功宣告完成
  bound_to:
    - "撼动旧习惯需要绝对优势"
    - "频率优先"
  tags: [counter-example, relapse, habit-change]
```

```yaml
- id: ce05
  title: "略胜一筹"的产品幻觉
  type: counter-example
  source_chapter: 第1章（L368–372；古维尔）
  source_quote: |
    "许多创新都以失败告终，因为用户总是过分地倚重原有产品，而商家却总是高估新产品。
    ……即便某个新产品优势显著，但如果与用户业已形成的习惯冲突太过激烈，那就注定无法
    成功。"
  failure_mode: 创业者以为功能更好 10%–20% 就能撬走竞品用户。
  mechanism: 旧产品的影响"深入骨髓"，切换意味着重学+放弃储存价值；微弱优势被切换
    成本吞没后，新产品的体验反而"感觉更差"（与 c08 Google/Bing 互证）。
  warning_signs:
    - 卖点清单全是"比对方好一点"
    - 未计算用户的储存价值损失
    - 演示惊艳但次日留存低
  bound_to:
    - "撼动旧习惯需要绝对优势"
  tags: [counter-example, innovation, competition]
```

```yaml
- id: ce06
  title: 可预见反馈回路的无效（冰箱门）
  type: counter-example
  source_chapter: 前言（L202）
  source_quote: |
    "你打开冰箱门，里面的工作灯就会亮起，这个结果在你预料之中，所以你不会没完没了地
    重复开门这个动作。假如给这个结果添加一些变量……你的渴望被点燃了。"
  failure_mode: 用稳定、可预期的奖励设计"激励"，期望产生持续使用欲。
  mechanism: 可预见结果不激活渴望回路；没有变量就没有多巴胺层面的"期待"，行为只剩
    工具性使用，用完即走。
  warning_signs:
    - 奖励固定、每次一样
    - 用户能准确说出下一次会得到什么
    - 完成任务后无"再来看看"冲动
  bound_to:
    - "多变的酬赏"
  tags: [counter-example, reward, predictability]
```

```yaml
- id: ce07
  title: 可预测后即失去魅力（婴儿与小狗）
  type: counter-example
  source_chapter: 第4章（L1211–1215）
  source_quote: |
    "几年后，小狗身上曾经让孩子兴奋不已的特点已经不再有吸引力。孩子已经能预知小狗的
    下一个动作，所以觉得没有以前那么好玩了。"
  failure_mode: 初期靠新鲜感获得增长后，以为兴趣会自然延续。
  mechanism: 大脑一旦掌握因果关系即把行为转为自动处理，意识不再投入；没有新变量注入，
    注意力流向下一个未知对象。
  warning_signs:
    - 核心体验长期未更新
    - 老用户活跃度系统性低于新用户
    - "再玩一次"的理由消失
  bound_to:
    - "有限 vs 无穷的多变性"
  tags: [counter-example, novelty, retention]
```

```yaml
- id: ce08
  title: 用真金白银误判动机（Mahalo 之败）
  type: counter-example
  source_chapter: 第4章（L1386–1398）
  source_quote: |
    "尽管他们能够从中获得酬赏，但是这种单纯的经济刺激手段似乎不具备持久的吸引力。……
    如果说他们的行为触发仅仅是经济利益，那还不如直接去做小时工。"
  failure_mode: 假设"给钱就能让用户持续贡献"，用悬赏机制驱动内容社区。
  mechanism: 金钱重新定义行为性质（从兴趣变成低薪打工），且数额小到构成侮辱；挤出了
    社交认同这一真正动机（过度理由效应的机制）。
  warning_signs:
    - 补贴一停贡献即停
    - 用户公开计算时薪
    - 社区氛围趋向交易化
  bound_to:
    - "社交认同大于经济激励"
    - "酬赏必须与内部触发和动机吻合"
  tags: [counter-example, incentive, crowding-out]
```

```yaml
- id: ce09
  title: Quora 强制公开浏览者身份
  type: counter-example
  source_chapter: 第4章（L1411–1417）
  source_quote: |
    "Quora 在没有提醒用户他们的浏览记录将会公之于众的情况下，自动把这项新功能强加给
    用户。顷刻间，用户视若珍宝的匿名权利荡然无存。……Quora 只好在数周后作罢。"
  failure_mode: 以"新奇功能"之名单方面收回用户既有权利（匿名），无提示、无选择。
  mechanism: 自主权被剥夺直接激活逆反心理；信任损失的不对称（收回很难再给回）放大
    抵抗，最终产品方撤回功能并损耗信誉。
  warning_signs:
    - 功能默认全量生效且不可关闭
    - 内部只讨论"刺激"不讨论"用户损失"
    - 上线首日反对集中在"未经同意"
  bound_to:
    - "保障用户自主权"
    - "先问'该不该'再问'能不能'"
  tags: [counter-example, autonomy, privacy]
```

```yaml
- id: ce10
  title: 强迫式记录触发逆反（MyFitnessPal）
  type: counter-example
  source_chapter: 第4章（L1437–1443）
  source_quote: |
    "没过多久，这种在手机上对自己饮食违纪行为供认不讳的做法就变成了强加于我的负担。
    ……在这样的事实面前，我要么臣服，要么放弃，最终我选择了放弃。"
  failure_mode: 把"帮助用户"设计成"审计用户"：漏记一天即前功尽弃，记录本身成为惩罚。
  mechanism: 行为的摩擦与道德压力随时间累积成逆反心理；目标（减肥）与手段（逐餐
    供认）错位，用户放弃手段时连目标一起放弃。
  warning_signs:
    - 断签一天即清零或示警
    - 记录动作本身无酬赏
    - 用户产生"欠债感"
  bound_to:
    - "保障用户自主权"
    - "酬赏必须与内部触发和动机吻合"
  tags: [counter-example, health-app, reactance]
```

```yaml
- id: ce11
  title: Zynga 小镇系列：有限多变性的破产
  type: counter-example
  source_chapter: 第4章（L1478–1484）
  source_quote: |
    "人们发现，它所开发的新游戏其实是新瓶装老酒，只是借用了'农场小镇'的外壳，所以玩家
    的热情很快消失，投资商也纷纷撤资。曾经引人驻足的创新因为生搬硬套而变得索然无味。"
  failure_mode: 复制成功产品的机制外壳而不注入新的不可预测性（小镇系列照搬农场玩法）。
  mechanism: 有限多变性在重复中耗尽，玩家可预见一切后续体验；依赖单一爆款的工作室
    模式又要求持续押中新品，失败一次即资本逃离（股价跌 80%）。
  warning_signs:
    - 新品与旧品只有皮肤差异
    - 玩家社区出现"换皮"共识
    - 收入集中于单一 IP
  bound_to:
    - "有限 vs 无穷的多变性"
  tags: [counter-example, variability, games]
```

```yaml
- id: ce12
  title: 无的放矢的"游戏化"
  type: counter-example
  source_chapter: 第4章（L1402）
  source_quote: |
    "积分、奖章、排名榜等'游戏化'元素是否奏效，完全取决于它们是否能够抓住用户内心的
    '痛痒'。……如果用户没有任何需求……那么'游戏化'元素也不会发挥任何功效。"
  failure_mode: 给无人真正愿意做的任务贴积分徽章，期望游戏机制替代产品价值。
  mechanism: 游戏化只是酬赏的载体；没有内部触发与真实需求时，载体无处附着，奖励
    甚至放大"任务毫无意义"的认知。
  warning_signs:
    - 先有积分体系后有用户需求分析
    - 徽章无人炫耀
    - 排行榜头部固化、尾部无感
  bound_to:
    - "酬赏必须与内部触发和动机吻合"
    - "社交认同大于经济激励"
  tags: [counter-example, gamification]
```

```yaml
- id: ce13
  title: 《圣经》应用的桌面网站之败
  type: counter-example
  source_chapter: 第7章（L2039）
  source_quote: |
    "我们最初将其设计为一个桌面网站，但此举根本没有引起人们对《圣经》的兴趣。直到尝试
    推出移动版本，我们才注意到人们所发生的变化。"
  failure_mode: 内容与动机俱在，但载体不可及——桌面网站无法在"启示时刻"出现在用户手边。
  mechanism: 触发密度受介质限制；B=MAT 中触发与能力两要素因设备不在场而不成立，
    行为频率永远上不去。
  warning_signs:
    - 用户"想起时无法使用"
    - 使用场景与设备场景错位
    - 同一内容换介质后数据剧变
  bound_to:
    - "B=MAT 福格行为模型"
    - "频率优先"
  tags: [counter-example, accessibility, platform]
```

```yaml
- id: ce14
  title: 一次性应用陷阱（下载即巅峰）
  type: counter-example
  source_chapter: 第5章（L1755）
  source_quote: |
    "2010年，移动应用程序的下载比例是 26％，但这些下载的应用程序仅被使用过一次。……
    人们正在使用的应用程序越来越多，但反复使用这些应用程序的频率却越来越低。"
  failure_mode: 把下载量当成功指标，忽视"打开第二次"的结构设计。
  mechanism: 无投入、无触发、无储存价值的应用在首次新鲜感耗尽后没有任何回访理由，
    竞争注意力的高频应用会把它挤出首屏。
  warning_signs:
    - 次日留存远低于行业
    - 首屏无回访入口
    - 用户说"挺好的，但我不用"
  bound_to:
    - "自主型触发是习惯的必要条件"
    - "储存价值五形式"
  tags: [counter-example, retention, mobile]
```

```yaml
- id: ce15
  title: App.net：功能更好的 Twitter 复制品之死
  type: counter-example
  source_chapter: 第5章（L1702–1714）
  source_quote: |
    "科技行业的许多观察家认为该产品实际上比 Twitter 更好。但是，与其他企图复制服务的
    尝试一样，App.net 并没获得成功。……对自己辛辛苦苦建起并精心呵护维持的关注群，
    没有人舍得放弃。"
  failure_mode: 以"无广告、体验更好"正面复制成功产品，期望用户平移。
  mechanism: 用户的储存价值（关注者网络、历史推文、社会资本）留在原产品；切换=
    社交资产清零。功能优势对冲不了储存价值（与 p21、ce05 互证）。
  warning_signs:
    - 差异点全在产品侧、无一在用户资产侧
    - 目标用户与在位产品重合度极高
    - 未提供资产迁移方案
  bound_to:
    - "储存价值五形式（关注者）"
    - "撼动旧习惯需要绝对优势"
  tags: [counter-example, switching-cost, competition]
```

```yaml
- id: ce16
  title: 兜售商模式：为不认识的用户设计
  type: counter-example
  source_chapter: 第6章（L1936–1944）
  source_quote: |
    "他们所谓的'现实扭曲场'使他们无法提出这样一个关键问题，即'我真的认为这有用吗'
    ……其答案几乎总是'不'。……兜售商们对用户往往做不到感同身受。"
  failure_mode: 设计者自己不用产品却坚信用户需要（广告业重灾区：指望用户喜欢自己的
    广告、天天用品牌 App）。
  mechanism: 缺乏第一人称体验时，设计者靠想象填补用户模型，"现实扭曲场"使关键自问
    失效；洞察力缺失导致产品与需求脱节，成功率极低。
  warning_signs:
    - 说不清用户"何时何地以何种情绪"使用
    - 从不亲自走完用户流程
    - 用"用户会喜欢的"替代"我在用的"
  bound_to:
    - "操纵矩阵"
    - "研究用户的实际行为而非内心愿景"
  tags: [counter-example, ethics, product-market-fit]
```

```yaml
- id: ce17
  title: 经销商模式与 Cow Clicker 的"奶牛危机"
  type: counter-example
  source_chapter: 第6章（L1956–1963）
  source_quote: |
    "开发出一款产品之后，如果设计者不相信该产品能提高用户的生活质量，而且他自己也不会
    使用，这就叫剥削利用。……当该游戏走红，一些人不可救药地迷恋上该游戏之后，博格斯特
    关闭了游戏。"
  failure_mode: 纯粹为榨取金钱设计钩子（讽刺品 Cow Clicker 除点击奶牛外一无所有，却真有
    人沉迷）。
  mechanism: 既无内部触发匹配也无价值交付的钩子只能靠操纵漏洞运转；一旦上瘾机制被
    识破或监督到来，商业与道德同时崩塌——博格斯特本人不得不关闭游戏。
  warning_signs:
    - 商业模式依赖放大冲动而非创造价值
    - 设计者回避"生活质量"之问
    - 收入与用户痛苦程度正相关
  bound_to:
    - "操纵矩阵"
    - "习惯不等于成瘾"
  tags: [counter-example, ethics, exploitation]
```

```yaml
- id: ce18
  title: 自检时的自我欺骗信号
  type: counter-example
  source_chapter: 第6章（L1908）
  source_quote: |
    "如果你发现自己在问自己这些问题的时候感到羞愧，或者回答问题的时候需要证明自己是
    正确的，或需要为自己寻找正当理由，那么请立刻停手！你已经失败了。"
  failure_mode: 用正当化说辞回答操纵矩阵两问（"用户应该会喜欢的""这算不上操纵"）。
  mechanism: 当理性化启动时，答案已从"是"滑向"否"；辩解行为本身是动机性推理的证据，
    继续推进只是给剥削披上外衣。
  warning_signs:
    - 回答前先组织辩护
    - 对两问给出例外条款
    - 用商业成功论证道德正当
  bound_to:
    - "操纵矩阵"
    - "自查时感到羞愧就立刻停手"
  tags: [counter-example, ethics, self-deception]
```

```yaml
- id: ce19
  title: "只有 1% 上瘾，无关紧要"的轻慢
  type: counter-example
  source_chapter: 第6章（L1926–1930）
  source_quote: |
    "如果简单地认为这一问题太微不足道，因而无关紧要的话，就会忽略技术上瘾导致的真正
    问题。……必须告知并保护那些对产品慢慢上瘾的用户。"
  failure_mode: 以病理性上瘾比例低为由，不做重度使用的识别、预警与干预。
  mechanism: 极端个案的公共曝光（诉讼、报道）足以定义产品形象；且公司已掌握识别数据，
    "不知道"的辩护不再成立——义务随能力产生。
  warning_signs:
    - 无重度使用预警指标
    - 客服无成瘾求助流程
    - 只优化总时长这一指标
  bound_to:
    - "对过度使用的用户负有告知与保护义务"
  tags: [counter-example, ethics, addiction]
```

```yaml
- id: ce20
  title: "包治百病"的设计方案
  type: counter-example
  source_chapter: 第3章（L945）
  source_quote: |
    "虽然 Facebook 注册器对于惜时如金的人来说是个宝贝，但是也有一些人认为它并不一定能
    简化注册过程。……用户遇到的问题不尽相同，而我们也没有一个包治百病的良方。"
  failure_mode: 把某个简化手法（第三方登录、一键注册）当作普适答案全量套用。
  mechanism: 六要素的短板因人群而异——对惜时者是捷径，对隐私敏感者是新的信任焦虑；
    不诊断短板就套方案，可能在补短板的同时竖起新墙。
  warning_signs:
    - 设计决策引用"行业最佳实践"而无用户细分
    - 同一流程对所有人一致
    - 无针对异议人群的替代路径
  bound_to:
    - "能力六要素与补最短板"
  tags: [counter-example, ux, overgeneralization]
```

```yaml
- id: ce21
  title: 爆品陷阱：有触发有酬赏，无投入
  type: counter-example
  source_chapter: 中文版序言（余晨，L93）
  source_quote: |
    "一个一夜爆红的产品，往往都有着很好的触发，也有着易操作的行动，还有着丰富的社交
    酬赏。但是如果没有后续引发长时间'投入'的能力，爆品也会随着时间推移而丢掉你的注意力。"
  failure_mode: 把"爆红"当"习惯"，触发-行动-酬赏三环俱全却缺第四环，热度自然衰减。
  mechanism: 没有储存价值与下一触发的闭环，循环断在投入处；多变性耗尽后（ce07/ce11）
    无转换成本留住用户。
  warning_signs:
    - 爆发期留存好、次月断崖
    - 用户"用完即走"且无资产沉淀
    - 增长全靠外部触发（投放/话题）
  bound_to:
    - "储存价值五形式"
    - "加载下一个触发"
  tags: [counter-example, viral, retention]
```

```yaml
- id: ce22
  title: 触发成功但循环断裂：动机与能力不同步
  type: counter-example
  source_chapter: 第3章（L865–867、L813）
  source_quote: |
    "但是，设计人员发现，就算触发生效，动机强烈，用户仍常常不按照设计者期望的轨迹前进。
    这是为什么？就是因为可行性不足，换句话说，用户没有能力轻松自如地使用这个产品。"
  failure_mode: 把触发设计（通知、广告、入口）当全部功课，触发后流程摩擦重重。
  mechanism: B=MAT 是乘法关系，触发到位而能力/动机任一为零，行为仍为零；团队常把
    "曝光"误当"行动"，归因于用户懒惰而非流程摩擦。
  warning_signs:
    - 点击率高、完成率低
    - 漏斗在注册/首用处陡降
    - 需要用户"学习"才能用
  bound_to:
    - "B=MAT 福格行为模型"
    - "先解决能力问题，而非动机"
  tags: [counter-example, funnel, friction]
```
