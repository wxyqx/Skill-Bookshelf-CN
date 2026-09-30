# candidates/counter-examples.md — 反例提取器产出

> 提取器: counter-example-extractor（串行降级执行，"干净视角"独立跑完）
> 反例不独立成 skill，是阶段 2 B (Boundary) 段的核心素材。
> 每条含 failure_mode + mechanism + warning_signs + bound_to。

```yaml
- id: ce01
  title: 思维上瘾
  type: counter-example
  source_chapter: 第一章
  source_quote: |
    "实际上这种强迫性的思维是一种上瘾症。上瘾症的特点是什么？非常简单：你没法选择
    停止，它甚至比你还强大。它同样给你一种错误的乐趣，而这种乐趣会最终变成痛苦。"
  failure_mode: 把思考当存在，停不下来；脑内独白 24 小时运转，误以为"这就是我"。
  mechanism: 认同思维→从思维活动中汲取自我感→"如果停止思维，我将不复存在"的恐惧
    使人不敢停下；思维反客为主（"你根本没有利用它，而是它在利用你"）。
  warning_signs:
    - 找不到"停止思考的按钮"
    - 独处安静时的背景性不安
    - 反复播放同一批念头（"旧唱片"）
  bound_to:
    - "观察思考者"
  tags: [counter-example, addiction, thinking]

- id: ce02
  title: 小我的时间机器（"某天我就会很好"）
  type: counter-example
  source_chapter: 第一章
  source_quote: |
    "它还不断地把自己投射到未来……它会说：'某天，当这个、那个或其他的事情发生时，
    我就会很好、很幸福，也很平和。'"
  failure_mode: 以过去定义自己（身份）、以未来安慰自己（希望），当下永远只是手段。
  mechanism: 小我由思维构成，只能活在过去与未来；当下对它是威胁，故不断制造
    心理时间。
  warning_signs:
    - 口头禅式"等……就好了"
    - 幸福永远配置在未来条件上
  bound_to:
    - "钟表时间 vs 心理时间判别"
  tags: [counter-example, ego, time]

- id: ce03
  title: 压抑情绪转为生理疾病
  type: counter-example
  source_chapter: 第一章（另见第六章）
  source_quote: |
    "如果你不能感受到你的情绪，或是切断了与情绪的联系，那么你最终会在纯生理这一层面
    体验到它们，它们会以生理问题或疾病的形式出现。"
  failure_mode: 与情绪失联→情绪沉入身体→以躯体化、疾病形式返场。
  mechanism: 情绪是"身体对思维的反应"；未被观察的能量不消失，只在无觉察处积累、
    合并成痛苦之身。
  warning_signs:
    - 说不出自己在感受什么
    - 用忙碌/酒精/食物麻痹
    - 不明原因的躯体紧张
  bound_to:
    - "痛苦之身觉察流程"
    - "与内在身体联结"
  tags: [counter-example, suppression, somatic]

- id: ce04
  title: 痛苦之身以痛苦为食（受害者-迫害者循环）
  type: counter-example
  source_chapter: 第二章
  source_quote: |
    "如果你被痛苦所控制，你会想要更多的痛苦。这时你会成为受害者或者迫害者：你要么为
    别人制造更多的痛苦，要么受痛苦的折磨，或者两者皆是。实际上，这两者没什么太大的
    区别。"
  failure_mode: 被激活后主动制造/寻找痛苦事件（吵架、自怜、戏剧化），以维持供能。
  mechanism: 痛苦之身靠与自身频率共振的经历生存；控制你的人生的"你"其实是它；
    "它会在你的生活中创造一种经常能激活它能量的情况，以便它继续生存。"
  warning_signs:
    - 无事生非的冲突冲动
    - 反复向他人讲述自己的受害故事
    - 心情差时疯狂消极思考
  bound_to:
    - "痛苦之身觉察流程"
  tags: [counter-example, pain-body, cycle]

- id: ce05
  title: 宁愿痛苦也不丢熟悉的自我
  type: counter-example
  source_chapter: 第二章
  source_quote: |
    "你可能宁愿在痛苦中，与痛苦之身认同，也不愿冒风险去丢失你熟悉的不幸自我而跃入
    一个未知之中。"
  failure_mode: 治疗/改变的最大阻抗：对"失去不幸身份"的恐惧大于对痛苦的厌恶。
  mechanism: 痛苦已成自我感的一部分；摆脱痛苦=小我死亡，无意识恐惧启动抗拒。
  warning_signs:
    - 从痛苦中获取兴奋感与谈资
    - 忍不住琢磨、回味、复述伤害
  bound_to:
    - "痛苦之身觉察流程"
  tags: [counter-example, identity, resistance]

- id: ce06
  title: 争论中非赢不可（错误=死亡）
  type: counter-example
  source_chapter: 第二章
  source_quote: |
    "即使是一件微不足道的平常小事，像在与别人的争论中迫切地希望打败对方，以证明自己
    是对的，都是由于小我对死亡的恐惧而引起的。……错误就等于死亡。很多战争就因此
    而起。"
  failure_mode: 把观点胜负当生死，防卫、攻击、辩解成瘾；人际关系破裂。
  mechanism: 认同观点=认同小我；承认错误即小我之死，故必须赢。
  warning_signs:
    - 生理性被点燃、必须回嘴
    - 事后反刍"我当时应该这么说"
  bound_to:
    - "非反应的'不'"
  tags: [counter-example, ego, conflict]

- id: ce07
  title: 用外在成就填补无底洞
  type: counter-example
  source_chapter: 第二章
  source_quote: |
    "他们拼命追求财富、成功、权力、名望或者一种特殊的关系……但是，即使他们拥有了这些
    东西，这种内在的空虚仍然存在，并且还是个无底洞。"
  failure_mode: 以财产/地位/关系/知识喂小我，越喂越饿；得到后短暂满足随即空虚。
  mechanism: 小我需要不断被喂养；外在物皆无常，认同它们=把自我押在必输的赌局上。
  warning_signs:
    - "得到之后"的空虚大于快乐
    - 下一个目标永远在别处
  bound_to:
    - "内在目的 vs 外在目的"
  tags: [counter-example, ego, achievement]

- id: ce08
  title: 以"希望"否定当下
  type: counter-example
  source_chapter: 第三章
  source_quote: |
    "促使你不断向前迈进的是希望，但是希望会使你将注意力集中在未来之上，而这种对未来
    的关注会促使你否定当下，因此造成你的不快乐。"
  failure_mode: 靠"未来会好"硬撑，从而错失当下、维持痛苦。
  mechanism: 希望是心理时间的产物；当下被贬值为通往未来的通道。
  warning_signs:
    - "熬过这段就好了"成为口头禅
    - 无法在当下找到任何可感激之物
  bound_to:
    - "接纳然后行动"
  tags: [counter-example, hope, time]

- id: ce09
  title: 目标沦为踏脚石
  type: counter-example
  source_chapter: 第三章
  source_quote: |
    "如果你过于注重目标……当下失去了固有的价值，而沦为通向未来的踏脚石。……你不会
    再看到路边的花朵或闻到它的芬芳。"
  failure_mode: 目标至上主义：生活被切成"忍耐—达成—新忍耐"，从不停留。
  mechanism: 注意力全在未来=心理时间；当下的行动失去质量与欢乐。
  warning_signs:
    - "等我……就……"句式高频
    - 对过程毫无感觉，只关心里程碑
  bound_to:
    - "内在目的 vs 外在目的"
    - "钟表时间 vs 心理时间判别"
  tags: [counter-example, goals]

- id: ce10
  title: 钟情的戏剧性事件（问题成为身份）
  type: counter-example
  source_chapter: 第九章（另见第三章）
  source_quote: |
    "大部分人都会有他们钟情的戏剧性事件。他们的故事就是他们的身份。……他们抗拒和
    害怕得最多的，就是戏剧性事件的终结。"
  failure_mode: 与问题共生：连寻求解决方案也变成戏码的一部分；治好=失去自我。
  mechanism: 问题=心理反刍+自我感来源；小我需要敌人与冲突维持孤立身份。
  warning_signs:
    - 故事讲了十年，版本越来越精细
    - 帮助无效时反而恼怒
  bound_to:
    - "此刻问题清零法"
  tags: [counter-example, identity, drama]

- id: ce11
  title: 麻醉剂式回避
  type: counter-example
  source_chapter: 第四章（另见第五章）
  source_quote: |
    "许多人利用酒精、药物、性爱、食物、工作、电视或购物作为麻醉剂来消除他们的不安。
    ……会让你产生依赖，并带有强迫性，而你通过它们所获得的只是短暂的缓解而已。"
  failure_mode: 用麻醉剂压制普通无意识的不安，产生依赖；使用只是延迟突破。
  mechanism: 麻醉剂"抑制过度活跃的思维"而不解决认同，故需不断加码。
  warning_signs:
    - 一停下就慌，必须找事/找东西填塞
  bound_to:
    - "无意识分层与挑战测试"
  tags: [counter-example, addiction, avoidance]
  note: 下游引用时须加医疗警示：作者不否认成瘾需专业帮助，本条不构成停药/戒断建议。

- id: ce12
  title: 抱怨=制造受害者身份
  type: counter-example
  source_chapter: 第四章
  source_quote: |
    "试着觉察你自己是否用语言或是思想在抱怨一个你身处的状况……抱怨通常是人们对本然
    不接受的表现。当你在抱怨时，你就使自己变成了一个受害者。"
  failure_mode: 以抱怨代替行动/离开/接纳；不快乐传染给周围人（"比疾病传播更快"）。
  mechanism: 抱怨强化对本然的抗拒，把无力感固化成身份。
  warning_signs:
    - 对天气/同事/伴侣的持续性吐槽
    - 说完抱怨毫无轻松感
  bound_to:
    - "接纳然后行动"
  tags: [counter-example, complaint, victimhood]

- id: ce13
  title: 用一生等待开始新的生活
  type: counter-example
  source_chapter: 第四章
  source_quote: |
    "任何一种形式的等待，都让你无意识地在你的此时此刻创造了一种内心的冲突：你不要
    此时此刻，你把希望寄托于未来。……人们总是用一生来等待开始新的生活。"
  failure_mode: 大等待吞噬人生：等假期/等升职/等孩子长大/等开悟，唯独不等在当下。
  mechanism: 等待=否定现在、需要未来；生命质量随等待塌陷。
  warning_signs:
    - "先把这段熬过去"成为生活主结构
    - 闲暇时反而空虚
  bound_to:
    - "等待状态识别与撤离"
  tags: [counter-example, waiting]

- id: ce14
  title: 探究过去=无底洞
  type: counter-example
  source_chapter: 第四章
  source_quote: |
    "如果你试图探究过去，它将会变成一个无底洞，永远探究不完。你可能会想，你需要更多
    的时间才能了解过去或者摆脱过去……这是一个幻象。"
  failure_mode: 无限回溯模式："再挖一点童年，我就能好"；时间越多，过去越重。
  mechanism: 注意力投向过去=给它供能并造出"过去的我"；理解≠化解。
  warning_signs:
    - 每个新问题都能联到同一个起点
    - "等我搞明白为什么"成为前置条件
  bound_to:
    - "不研究过去"
  tags: [counter-example, past, therapy-contrasting]
  note: 涉及创伤处理时须转介专业支持，本条不构成放弃治疗的依据。

- id: ce15
  title: 接纳沦为"精神上的标记"（假接纳）
  type: counter-example
  source_chapter: 第四章
  source_quote: |
    "如果你不再继续向前迈进，你的这种接纳就成了一个精神上的标记，它使你的小我不断地
    沉浸在不幸之中，而且还会加强你和其他人的分离感。"
  failure_mode: 用"我允许一切发生"的话术包裹消极认同，灵性化的小我原地踏步。
  mechanism: 只停在接纳第一阶段，未拆产生消极情绪的机制；"每件事都很好"的口头
    接纳与内在感受分裂。
  warning_signs:
    - 灵性话术与实际情绪长期不符
    - 以"接纳"命名回避行动
  bound_to:
    - "假接纳警报"
  tags: [counter-example, spiritual-bypassing]

- id: ce16
  title: 人际关系=思维互动
  type: counter-example
  source_chapter: 第六章
  source_quote: |
    "大部分的人际关系主要由思维互动组成，而不是由人类之间的相互沟通和合一组成。
    这就是为什么在人际关系中有如此多的冲突的原因。"
  failure_mode: 对话时注意力在自己的评判与反辩上；"赋予自己思维的注意力比赋予别人
    说话内容的注意力要多得多"。
  mechanism: 思维占据注意力→听不到对方话语之下的本体→冲突必然。
  warning_signs:
    - 对方未说完已备好反驳
    - 事后记不住对方说了什么
  bound_to:
    - "用身体倾听与思考"
  tags: [counter-example, communication]

- id: ce17
  title: 苦修式身体否认
  type: counter-example
  source_chapter: 第六章
  source_quote: |
    "其他人则通过入定或灵魂出体的方式来逃避身体。……事实上，没有人曾经通过拒绝身体、
    折磨身体或是身体经验来达到开悟。"
  failure_mode: 把身体当罪/障碍：禁欲、苦修、出体逃逸——对抗身体即对抗本质。
  mechanism: 对动物性本性的无意识抗拒制造羞耻与分裂；转化工作恰在身体中。
  warning_signs:
    - 灵修以自我惩罚为荣
    - 对感官喜悦的系统性罪恶感
  bound_to:
    - "转化通过身体发生"
  tags: [counter-example, asceticism]

- id: ce18
  title: 上瘾式爱情（爱恨循环）
  type: counter-example
  source_chapter: 第八章
  source_quote: |
    "所有沉溺上瘾都源于你无意识地拒绝去面对和经历痛苦。每一次上瘾症都始于痛苦，又以
    痛苦收场。……关系本身不会造成痛苦和不快乐，它们只是将已经在你内在的痛苦和不快乐
    引发出来。"
  failure_mode: 把伴侣当药：激情期高潮、失效期戒断反应（嫉妒、控制、报复），爱恨
    两极摇摆直至破裂。
  mechanism: 上瘾对象掩盖而非解决内在痛苦；药物失效时痛苦更烈，且被投射给对方。
  warning_signs:
    - 离开对方的可能性即引发恐慌
    - 同一个人既是天堂又是地狱
  bound_to:
    - "完全接受你的伴侣"
    - "爱情关系不是让你幸福，而是让你更有意识"
  tags: [counter-example, relationship, addiction]

- id: ce19
  title: 通过恋爱逃避独处
  type: counter-example
  source_chapter: 第八章
  source_quote: |
    "如果你独自一人的时候感到不安，你就会寻找一种爱情关系来掩盖你的不安。可以肯定的
    是，在你与别人的爱情关系中，你的不安又会以其他形式重新出现。"
  failure_mode: 用关系逃避与自己相处；不安换个伴侣重现，或归咎伴侣。
  mechanism: 不安源于与本体失联，关系无法替代；"你需要与自己建立关系吗？"——二元
    分裂本身就是问题。
  warning_signs:
    - 空窗期恐慌大于失恋痛
    - 恋爱动机清单里"逃避独处"权重高
  bound_to:
    - "爱情关系不是让你幸福，而是让你更有意识"
  tags: [counter-example, relationship, loneliness]

- id: ce20
  title: 集体受害者身份
  type: counter-example
  source_chapter: 第八章
  source_quote: |
    "如果她们的自我感源于这个事实，并使她们陷入这种集体受害者身份中不能自拔，她们
    就是错的。……如果女人排斥男性，这就会助长一种孤立的感觉并会强化小我。"
  failure_mode: 以群体苦难叙事（"他们对我们所做的"）作为自我感来源，愤怒与仇恨
    成为归属；被困于过去。
  mechanism: 集体痛苦之身真实存在（作者承认历史不公），但认同它=给它续命；
    "过去比现在更强大"是伪真理。
  warning_signs:
    - 群体怨愤成为主要身份内容
    - 离开怨愤叙事的愧疚感
  bound_to:
    - "不要从痛苦中汲取身份认同"
  tags: [counter-example, collective, identity]
  note: 下游引用时须注明：不否认结构性不公，仅警示"以受害者身份为自我感"的心理陷阱。

- id: ce21
  title: 认同消极心态，拒绝积极变化
  type: counter-example
  source_chapter: 第九章
  source_quote: |
    "一旦你认同了你的某种消极心态，你就不想放手，同时你在无意识的层面还会抗拒积极的
    变化……你就会忽视、拒绝或破坏你生活之中的积极方面的事情。"
  failure_mode: 抑郁/愤怒/不开化成了人格设定；好运与好关系被无意识破坏。
  mechanism: 身份认同优先于幸福——改变=威胁"我是谁"。
  warning_signs:
    - 好事发生时莫名不适
    - 自称"我就是这种人"以终止讨论
  bound_to:
    - "假接纳警报"
    - "无意识分层与挑战测试"
  tags: [counter-example, identity, negativity]

- id: ce22
  title: 反抗低能量周期
  type: counter-example
  source_chapter: 第九章
  source_quote: |
    "许多疾病正是由于反抗低能量周期而产生的，然而低能量周期对于重建来说极为关键。
    我们总是想要有所作为……这些使你很难或无法接受低能量周期。"
  failure_mode: 强制永远高峰：低谷时自责、硬撑、用刺激拉抬，身体以疾病强制重启。
  mechanism: 能量有循环（几小时到几年），抗拒循环=与生命之流对抗。
  warning_signs:
    - 低谷即自我攻击
    - 休假时负罪感
  bound_to:
    - "无常与循环的接受"
  tags: [counter-example, energy, burnout]
  note: 涉及健康论述，下游引用须加医疗警示。

- id: ce23
  title: 智力与意识不协调
  type: counter-example
  source_chapter: 第十章
  source_quote: |
    "我遇到过许多高智商的和受过高等教育的人，他们完全没有意识……事实上，如果智力和
    知识的增长与相应的意识增长不协调，不幸和灾难的爆发潜力是巨大的。"
  failure_mode: 高智商+零临在=高效制造灾难（个人与集体）；聪明被小我劫持。
  mechanism: 制约反应与智力无关；无意识者的每一步都由旧模式代驾。
  warning_signs:
    - 以分析代替觉察
    - 同类错误在不同领域重复
  bound_to:
    - "无意识分层与挑战测试"
  tags: [counter-example, intelligence, blind-spot]

- id: ce24
  title: 口是心非的假臣服
  type: counter-example
  source_chapter: 第十章
  source_quote: |
    "放弃反应不是指仅口头上说'好，你是对的'，脸上却写着'我才不屑于你这种幼稚的
    无意识之举'。这种口是心非的反应，只是把抗拒放置在另一个层面。"
  failure_mode: 以"不争了"包装轻蔑；以"我不在乎"包装怨恨——戴面具的抗拒。
  mechanism: 小我极其狡猾，会把投降表演成新式武器；真臣服放下整个争斗能量场。
  warning_signs:
    - 嘴上认输、身体紧绷
    - "随便你"式撤退
  bound_to:
    - "非反应的'不'"
    - "两次臣服机会"
  tags: [counter-example, passive-aggression, surrender]
```
