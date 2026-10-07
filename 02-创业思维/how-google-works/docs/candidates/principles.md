# 候选原则（principle-extractor 产出）

> 来源：《重新定义公司：谷歌是如何运营的》（How Google Works）
> 提取范围：作者明确提出的"应该如何 / 不应该如何"的可套用规则、清单、判断规则、断言与箴言。
> 不含思维框架、案例细节、反例分析、术语定义（分别归 framework / case / counter-example / glossary extractor）。

```yaml
- id: p01
  title: 聚焦用户，一切水到渠成
  type: principle
  source_chapter: 前言 · 谷歌是如何运营的（并见第六章"聚焦用户"）
  source_quote: |
    "两人一直秉承着几条基本原则，其中首要的，就是聚焦用户（focus on the user）。……如果谷歌能提供优质服务，
    那么资金问题就能迎刃而解。""'聚焦用户'这句话只说了一半，完整的句子应该是：'聚焦用户，一切水到渠成。'"
  summary: |
    把"为用户做对的事"设为第一决策准则，信任创意精英能事后找到赢利方式；用户利益与客户利益冲突时，用户优先。
  tags: [principle, strategy, user-first]

- id: p02
  title: 遇到问题，去和工程师谈谈
  type: principle
  source_chapter: 前言 · 谷歌是如何运营的
  source_quote: |
    "计划还有什么意义？计划只是在拖我们的后腿罢了。一定有比计划更有效的方式，去和工程师谈谈吧。"
    "遇到问题时莫忘'去和工程师谈谈'。"
  summary: |
    遇到业务难题时，不要先写计划书，而是直接与一线做产品的人对话，从掌握事实与能力的人那里找答案。
  tags: [principle, decision, ground-truth]

- id: p03
  title: 尽可能多聘顶尖工程师，给足自由发挥的空间
  type: principle
  source_chapter: 前言 · 谷歌是如何运营的
  source_quote: |
    "谢尔盖和拉里创造出一款伟大的搜索引擎并提供其他优质服务的计划其实非常简单：尽可能多地聘请有才华的软件工程师，
    给他们自由发挥的空间。"
  summary: |
    产品卓越的路径不是流程管控，而是密度足够高的顶尖人才加最大化的自主权。
  tags: [principle, talent, autonomy]

- id: p04
  title: 无法管理想法，就管理思考的环境
  type: principle
  source_chapter: 前言 · 谷歌是如何运营的
  source_quote: |
    "如果你无法管理创意精英的想法，就必须学会管理他们进行思考的环境，让他们乐于置身其中。"
  summary: |
    对创意型人才，管理者的抓手不是命令其头脑，而是营造文化、空间与机制，使其自愿产出最好的想法。
  tags: [principle, management, environment]

- id: p05
  title: 主要要素成本曲线下降，行业剧变不可避免
  type: principle
  source_chapter: 前言 · 谷歌是如何运营的
  source_quote: |
    "如果某行业产品主要要素的成本曲线下降，那么该行业必将会出现剧变。"
  summary: |
    判断一个行业是否即将被颠覆的可操作信号：盯住其核心生产要素的成本曲线，一旦陡降，转变时机已到。
  tags: [principle, assertion, industry-analysis]

- id: p06
  title: 产品卓越压倒营销
  type: principle
  source_chapter: 前言 · 谷歌是如何运营的
  source_quote: |
    "如果产品乏善可陈，其劣势是市场营销和公关营造的品牌力量完全不足以反转的。"
  summary: |
    在信息对称的时代，不要指望用营销补救劣质产品；资源应先投向把产品做卓越。
  tags: [principle, product, marketing]

- id: p07
  title: 秘诀就是快速
  type: principle
  source_chapter: 前言 · 谷歌是如何运营的
  source_quote: |
    "要想持续保持产品的成功及品质的卓越，秘诀就是快速。"
  summary: |
    实验与迭代成本骤降后，速度本身成为产品质量的来源；把"快"当作组织纪律而非口号。
  tags: [principle, product, speed]

- id: p08
  title: 只求渐变不求突破，企业终将落伍
  type: principle
  source_chapter: 序言 · 谷歌的"痴心妄想"（拉里·佩奇）
  source_quote: |
    "不少企业安于现状，只求渐变，不求突破。如果只求渐变，时间一长，企业就会逐渐落伍，科技行业尤其如此。"
  summary: |
    渐进改良是慢性自杀；必须以革命性目标要求自己，而不是比上一版好一点。
  tags: [principle, assertion, ambition]

- id: p09
  title: 强迫自己着眼未来，投资看似疯狂的赌注
  type: principle
  source_chapter: 序言 · 谷歌的"痴心妄想"（拉里·佩奇）
  source_quote: |
    "所以，你需要强迫自己着眼于未来。也是因此，谷歌才会投资无人驾驶汽车以及'热气球互联网计划'等看似高风险的领域。
    今天看似最冒险的赌注放在几年之后看也就不会显得那么疯狂了。"
  summary: |
    主动配置资源到几年后回头看才"合理"的项目；不指望环境推着你面向未来。
  tags: [principle, strategy, long-term]

- id: p10
  title: 物色独立思考者，设定远大目标
  type: principle
  source_chapter: 序言 · 谷歌的"痴心妄想"（拉里·佩奇）
  source_quote: |
    "谷歌才会投入大量精力去物色善于独立思考的人，并设定远大的目标。因为只要有了合适的人才和足够远大的梦想，
    你的目标往往就可以实现。"
  summary: |
    目标能否实现，取决于两件事的乘积：人才的独立思考能力 × 目标的远大程度；两者都要拉满。
  tags: [principle, talent, goal-setting]

- id: p11
  title: 在企业成立之初就确定企业文化
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "在企业成立之初就认真考虑并且确定你希望的企业文化，这才是明智之举。最好的方法就是询问构成企业核心队伍的创意精英。"
  summary: |
    文化不能交给命运自然生成；创业之初就要问团队"我们重视什么"，把答案记下来。
  tags: [principle, culture, founding]

- id: p12
  title: 相信自己的口号：使命宣言要实话实说
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "在面对商业用语的时候，人们的'测谎仪'已经被磨炼得异常灵敏了……当你把企业使命写在纸上的时候，还是实话实说为好。
    ……如果你歪曲事实，无异于玩火自焚。"
  summary: |
    自检方法：把信条换成反面说法，若员工无动于衷，说明是空话；员工会激烈反对的才是真信条。
  tags: [principle, culture, authenticity]

- id: p13
  title: 别用海报传达价值观，要反复当面交流
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "注意不要通过海报或手册形式分享企业价值观，而要进行不厌其烦、推心置腹的交流。"
  summary: |
    价值观靠高频的人际沟通与奖励行为巩固，不靠张贴物；不常传达的愿景等于废纸。
  tags: [principle, culture, communication]

- id: p14
  title: 拥挤出成绩
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "办公室的设计应本着激发活力、鼓励交流的理念，而不要一味制造阻隔、强调地位。……我们必须为他们提供一个拥挤的环境。"
  summary: |
    办公空间按"最大化偶遇与交流"设计，而不是按级别分配面积；伸手能拍到同事肩膀的环境才有创意碰撞。
  tags: [principle, culture, office-design]

- id: p15
  title: 让不同职能的团队挤在一起办公
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "这就要求产品经理与工程技术人员（或是化学家、生物学家、设计师以及公司其他负责产品设计研发的创意精英）
    一同吃住、并肩工作。"
  summary: |
    打破按职能分楼的格局，把产品、工程、设计等团队物理上放在一起，缩短协作回路。
  tags: [principle, organization, office-design]

- id: p16
  title: 杂乱是种美德
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "制造混乱并非目的……但是，混乱往往是自我表达和创新的衍生品，因此可以算是一种好事吧。……
    你完全可以抛开顾虑，让你的办公室潇洒地乱一回。"
  summary: |
    容忍办公环境的凌乱，把它视为工作活跃度的信号，不要用整洁指标扼杀自我表达。
  tags: [principle, culture, office-design]

- id: p17
  title: 无关紧要的资源上省钱，关键资源不惜投入
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "在奢华的办公设施和宽敞的办公室等无足轻重的资源上，我们能省就省，但对于那些关系重大的资源，我们则不惜倾力投入。"
  summary: |
    资源分配的二分法：办公面积之类面子工程从简，计算能力、工具、数据之类生产资料顶配，并以此根除攀比。
  tags: [principle, resource-allocation]

- id: p18
  title: 在家办公是瘟疫，把人聚在办公室
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "在家办公其实无异于一种会在整个公司内蔓延、让员工士气萎靡不振的瘟疫。……还是在你的办公室准备好各种设施，
    然后欢迎员工来使用吧！"
  summary: |
    偶发创意依赖面对面碰撞；与其远程妥协，不如把办公室做成比家里更有吸引力的工作场所。
  tags: [principle, culture, office-design]

- id: p19
  title: 别听"河马"的话
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "从本质上来讲，薪金的高低与决策能力完全无关。……如果把'河马'的声音屏蔽掉，有价值的观点就会受到重视。"
  summary: |
    会议室里不给最高薪者自动话语权：论点靠数据与论据取胜，谁有理听谁的，形成"提议不问出处"的任人唯贤环境。
  tags: [principle, decision, hippo]

- id: p20
  title: 把提出质疑设为硬性义务
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "如果员工对某个问题存在疑义，就必须把自己的顾虑提出来。……我们才应当把'提出质疑'作为一种硬性规定，
    而不是可做可不做。"
  summary: |
    异议不是权利而是义务：有疑义不说等于失职；把它定为硬规定，让沉默寡言者也必须开口制衡权威。
  tags: [principle, culture, dissent]

- id: p21
  title: 7 的法则：管理者至少带 7 个直接汇报人
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "在谷歌，我们要求每位管理者的桌上至少要放7份直接报告……这一原则会让企业的组织结构趋于扁平，
    减少管理层的监督并赋予员工更多自由。"
  summary: |
    用"下限管理幅度"倒逼扁平：汇报对象不少于 7 人，管理者忙到无法事事插手，员工自然获得自由。
  tags: [principle, organization, flat-hierarchy]

- id: p22
  title: 按职能而非业务线划分部门
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "谷歌坚持按职能划分部门……以业务或产品线为基础的组织结构会造成'各成一家'的局势，
    从而对人员和信息的自由流动形成扼制。"
  summary: |
    尽可能长期保持工程/产品/财务/销售的职能型结构并直接向 CEO 汇报，防止事业部各自为政。
  tags: [principle, organization, structure]

- id: p23
  title: 分部有独立损益表时，让外部客户成为赢利主力
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "如果你所在企业的分部各有自己的损益表，请确保让外部消费者和合作伙伴成为部门赢利的主要推动力。"
  summary: |
    若必须设利润中心，就要保证各部门的钱来自外部客户而非内部转移定价，否则盈亏指标会扭曲方向。
  tags: [principle, organization, incentive]

- id: p24
  title: 别把组织结构图当秘密
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "另外，也请尽量不要把企业组织结构文件作为秘密藏起来。"
  summary: |
    组织透明是信息自由流动的前提；藏起来的结构图只会滋生猜测与内耗。
  tags: [principle, transparency, organization]

- id: p25
  title: 重组要速战速决
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "把所有重组工作安排在一天内完成……重组的关键，一是要速战速决，二是要在重组敲定前就开始实施。"
  summary: |
    组织调整一拖就烂：把重组压缩到极短时间，并且在方案敲定前就让团队参与实施，用混乱换速度。
  tags: [principle, organization, reorg]

- id: p26
  title: 重组前先权衡各团队的不同倾向
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "第一，留意不同团队的不同倾向：工程人员喜欢复杂，市场人员喜欢增加管理层，销售人员喜欢招助理。
    你需要从中做出权衡。"
  summary: |
    重组设计前认清各职能的系统性偏好（工程要复杂、市场要层级、销售要助理），有意识地抵消其偏差。
  tags: [principle, organization, reorg]

- id: p27
  title: 两个比萨原则
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "这个原则规定，团队人数不能多到两个比萨还吃不饱。……小团队要比大团队更有效率，他们不会花那么多时间钩心斗角。"
  summary: |
    团队规模以两个比萨能喂饱为上限；大团队可以存在，但不能阻碍原有小团队做突破性创新。
  tags: [principle, organization, team-size]

- id: p28
  title: 组织以最有影响力的人为中心
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "找出最有影响力的人物，组织就以此人为中心。不要把岗位或经验作为选择管理者的标尺，而要看他的表现和热情。"
  summary: |
    围绕实际影响力组织团队而非围绕头衔；选管理者看表现与热情，找出后立刻压上重任。
  tags: [principle, organization, leadership]

- id: p29
  title: 高层会议一半席位留给产品专家
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "在管理层的顶端，最有影响力的人……应该是产品负责人。在首席执行官召开的会议上，
    至少有一半与会者应是产品与服务方面的专家。"
  summary: |
    用会议席位结构保证决策层注意力落在产品质量上，财务与销售议题不占主导。
  tags: [principle, organization, product]

- id: p30
  title: 产品设计不得带有组织结构的痕迹
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "一款产品的设计绝不应该带有企业组织结构的痕迹。打开iPhone手机的包装盒，你能推测出苹果公司的大权掌握在谁手里吗？
    当然能。苹果公司地位最高的人就是你们这些消费者。"
  summary: |
    检验标准：用户能否从产品结构反推出你的内部权力地图？能，就说明部门利益渗进了产品，必须重构。
  tags: [principle, product, organization]

- id: p31
  title: 选领导只挑不把私利置于整体利益之上的人
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "在物色领导者的时候，要挑选那些不会将一己之利置于企业整体利益之上的人。"
  summary: |
    领导者的第一筛选条件是利益排序：凡是把部门利益凌驾于公司之上的，再能干也不用。
  tags: [principle, leadership, incentive]

- id: p32
  title: 驱逐恶棍
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "一旦在团队中发现害群之马，最好的方法是减少其职责，并让骑士接手剩下的工作。对于极端败坏的恶行，
    你需要立即动手，把恶棍铲除出去。"
  summary: |
    对品行不端者零容忍：先削权再清除，极端恶行立即处理；"一日为恶，终身为恶"，不给第二次机会。
  tags: [principle, culture, talent]

- id: p33
  title: 保护明星
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "明星对企业的贡献足以支撑其狂妄，你就需要对他们多加容忍，甚至悉心保护。"
  summary: |
    对成就足以抵消大牌做派的顶尖人才，要刻意容忍其不循常规，防止文化的条条框框误伤他们。
  tags: [principle, culture, talent]

- id: p34
  title: 别把恶棍和明星搞混
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "切记不要把'恶棍'和'明星'搞混。恶棍的恶行是人品不端的产物，而明星的行为是出类拔萃的结果。"
  summary: |
    判断标准不是"难不难相处"而是"私利还是业绩"：恶棍把私利置于集体之上，明星对个人与集体利益同等重视。
  tags: [principle, culture, talent]

- id: p35
  title: 警惕恶棍比例的临界点
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "恶棍所占的比例有一个临界点。这个比例达到一定数值时……大家就会认为自己必须迎合恶棍的做法才有出路。"
  summary: |
    恶棍数量过了某个很低的阈值，好人会开始模仿恶行并层层扩散；监控比例，别等文化溃败才动手。
  tags: [principle, culture, warning]

- id: p36
  title: 给员工自由和责任，而非规定工时
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "作为领导者，你需要给员工以自由和责任。不要强迫他们加班加点，也无须规劝他们早些回家陪伴家人。
    ……他们就会全力以赴地确保完成工作。"
  summary: |
    放弃"工作与生活平衡"的统一标尺：只要求对结果负全责，把节奏决定权交还员工本人。
  tags: [principle, management, work-life]

- id: p37
  title: 没有人是不可或缺的
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "没有人对企业来说是真正不可或缺的。……给这种人安排一个假期，让别人填上空缺。"
  summary: |
    谁自称"离了他公司就转"，就强制其休假验证；既锻炼接班人，也拆掉个人的安全感把戏。
  tags: [principle, management, succession]

- id: p38
  title: 不轻易增设流程与门槛
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "添加流程或增设门槛的前提条件一定要严格，如果不是出于能够让人百般信服的业务上的考量，就不要增设这些障碍。"
  summary: |
    成长期的混乱不要用加流程来治；每一次设审批都要拿出强业务理由，否则一律说"好"。
  tags: [principle, culture, process]

- id: p39
  title: 快乐强扭不来：放宽限制，信赖员工
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "信赖你的员工，不要因惧怕出纰漏而杞人忧天，真正的快乐只有在这样自由放任的环境中才能绽放。"
  summary: |
    快乐文化靠自由放任与员工互嘲（如 Memegen）生长，不靠强制的派对与团建；没有什么"神圣不可侵犯"。
  tags: [principle, culture, fun]

- id: p40
  title: 领导者要有"跟我来"的态度
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "任何有志于做创意精英领导者的人，都需要拥有这样的态度。……热情对领导力不可或缺，如果你缺少热情，就马上走人。"
  summary: |
    领导不是喊"冲啊"，而是身先士卒（捡垃圾、擦前台、深夜在场）；没有热情就不配做创意精英的领导。
  tags: [principle, leadership, passion]

- id: p41
  title: 不作恶：人人都有拉绳中止的权力
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "每家企业都应'不作恶'，这句话就如北极星一般，为管理方式、产品计划以及办公室政治指明了方向。"
  summary: |
    给每个员工以道德否决权：任何人以价值观为由喊停一项决策时，全员必须停下来共同评估。
  tags: [principle, culture, ethics]

- id: p42
  title: 改造文化三步：找症结、写未来、去糟粕
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "要改变企业文化，首先要找出症结所在。……接下来，阐明你希望塑造的企业文化。……
    在弘扬前人理念的同时，我们也应大胆剔除糟粕。"
  summary: |
    变革既有文化的操作顺序：诊断真实文化（而非宣言）→ 明确目标文化并示范 → 继承传统精华、公开废除过时规矩。
  tags: [principle, culture, change]

- id: p43
  title: 着装标准：别光着身子就行
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "（在公司会议上，曾经有人要求埃里克阐述一下谷歌的着装标准。埃里克给出的答案是：'别光着身子就行。'）"
  summary: |
    对与工作无关的个人事务（穿着等）只设最低底线，把规范减少到极限。
  tags: [principle, culture, freedom]

- id: p44
  title: 你的计划一定是错误的：投团队不投计划
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "如果你有商业计划，那你的计划一定是错误的。……风险投资家应永远遵守投团队而不投计划的准则。既然计划会错，那么人就得对。"
  summary: |
    把"计划必然有硬伤"当作默认前提：评估事业时看团队的调整能力，而不是计划的严密程度。
  tags: [principle, strategy, planning]

- id: p45
  title: 计划可变，基础岿然不动
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "你的计划虽然可以调整，但必须以合乎现今社会运作方式的基本原理为基础……计划可变，基础则应岿然不动。"
  summary: |
    战略的正确写法：把支撑计划的基本原理（如成本曲线、平台逻辑）固化下来，具体计划随时推翻重来。
  tags: [principle, strategy, planning]

- id: p46
  title: 记录基本原则，而非商业计划
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "谷歌并不需要记录什么商业计划……但为了招纳新人和保证大家前进方向的一致，谷歌必须把计划所依据的基本原则记录下来。"
  summary: |
    组织对齐靠一页基本原则而不是厚厚的路线图；原则给定了，创意精英自己知道怎么做。
  tags: [principle, strategy, alignment]

- id: p47
  title: 信赖技术洞见，而非市场调查
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "不断改进以及使用巧妙的商业手段无可厚非，但如果把市场调查看得比技术创新还要重要，那就本末倒置了。"
  summary: |
    战略的根基是"用创新方式应用科技"带来的成本骤降或功能跃升，不是细分人群与口味调研。
  tags: [principle, strategy, technical-insight]

- id: p48
  title: 用"技术洞见之问"检验每个产品
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "我们要求谷歌所有正在生产的主要产品的负责人写出几句话，说明他们的产品计划背后的技术洞见。……
    如果你找不出一个有说服力的答案，那就好好反思吧。"
  summary: |
    对每个在做的产品回答："它背后的技术洞见是什么？"写不出来，产品大概率平庸，尽早砍掉或重构。
  tags: [principle, product, technical-insight]

- id: p49
  title: 满足用户尚未意识到的需求更重要
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "市场调查不能指导你去解决连消费者自己也没想到可以解决的问题。与满足消费者的现有需求相比，
    满足消费者尚未意识到的需求更为重要。"
  summary: |
    别去找快马：用户访谈只能告诉你现状的痛点，突破性产品要瞄准用户自己都还没想到的需求。
  tags: [principle, product, user-research]

- id: p50
  title: 找到你的极客，看他们在研究什么
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "无论你从事什么业务，你所在的行业都潜藏着一个巨大的技术知识库。……找到你的极客，看看他们在研究什么，
    这样，你就挖掘到了迈向成功的技术洞见。"
  summary: |
    寻找技术洞见的最短路径：公司里谁在实验室里折腾有趣的东西，那里就是你的战略方向来源。
  tags: [principle, strategy, technical-insight]

- id: p51
  title: 从具体问题的解决方案出发加以拓展
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "找到一个具体问题的解决方案，然后想办法对这个解决方案加以拓展，这也是寻找技术洞见的一个方法。"
  summary: |
    技术洞见常以"为某个具体问题而生的粗糙方案"起步；做成后主动追问：这项技术还能用在哪些领域？
  tags: [principle, strategy, technical-insight]

- id: p52
  title: 为成长而优化，全球扩张必须是核心
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "全球扩张必须成为企业的基础核心。现今的竞争日渐激烈，任何竞争优势都难以持久，因此你必须有一个'快速长大'的战略。"
  summary: |
    优化方向选规模而非收入：先让使用量/覆盖面指数级增长，赢利模式随后跟上。
  tags: [principle, strategy, growth]

- id: p53
  title: 只看平台，不看产品
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "随着平台的不断扩张和不断升值，越来越多的投资会涌进来……因此我们说，科技行业中的企业永远'只看平台，不看产品'。"
  summary: |
    评估与投入的对象是能吸聚供需双方、随使用量增值的平台，而不是单个产品的成败。
  tags: [principle, strategy, platform]

- id: p54
  title: 建网络不为省成本，而为提高质量
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "在互联网时代，创建网络不仅仅是为了降低成本和方便运营，更是为了从根本上提高产品质量。"
  summary: |
    交易成本塌陷后，开放网络的正确用途是借外部之力重塑产品模式，只拿它省成本是错失良机。
  tags: [principle, strategy, network]

- id: p55
  title: 与合作伙伴慷慨分成
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "谷歌最重视公司的发展，而不是如何赚取更多的钱，因此我们的做法是尽量给合作伙伴多分。"
  summary: |
    分成谈判中让伙伴多拿：短期让利换来合作规模扩张，最终自己受益；重发展轻分成比例。
  tags: [principle, partnership, growth]

- id: p56
  title: 专攻你已经领先的方向
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "之所以专注于搜索，是因为谷歌认为自己在这方面比任何企业都要领先。"
  summary: |
    选择聚焦点的依据不是市场预测而是相对优势：在你已领先的那一件事上做到极致，其余合作或放弃。
  tags: [principle, strategy, focus]

- id: p57
  title: 用五把标尺衡量产品
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "我们通过五把标尺来衡量搜索引擎的好坏：速度（快比慢好）、准确（搜索结果与用户的搜索请求有多接近）、
    好用、全面、新鲜。"
  summary: |
    给核心产品定义一组简明、可感知的质量标尺（速度、准确、好用、全面、新鲜），所有改进对齐这五项。
  tags: [principle, checklist, product-quality]

- id: p58
  title: 把开放当战略：先问能否助扩张与收入
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "我们可以将开放当作一种战略措施，问问自己：开放能否帮助扩张业务和赚取收入？开放可以为企业带来道德光环，
    从而吸引创意精英的到来。"
  summary: |
    开放与封闭无关道德，是可计算的战略选项；判断标准是开放能否带来扩张、创新与人才吸引力。
  tags: [principle, strategy, open]

- id: p59
  title: 封闭的两个前提
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "如果你能像苹果一样通过封闭系统大获全胜，那么当然可以选择封闭。如果不能，那就选择开放吧。"
  summary: |
    只有两种情况选封闭：产品有明显技术洞见优势且身处高速成长的新兴市场；或开放会实质损害用户体验（如搜索算法）。
  tags: [principle, strategy, open]

- id: p60
  title: 给用户随时退订的自由
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "如果用户选择离开谷歌，这支团队会尽量为他们提供方便。……如果用户可以轻松选择退订你的服务，
    那么你就得付出努力，让他们愿意继续留下来。"
  summary: |
    不锁用户：降低退出门槛，倒逼自己靠产品优势而非切换成本赢得忠诚。
  tags: [principle, strategy, open, user-first]

- id: p61
  title: 莫被竞争对手牵着鼻子走：以敌为傲但不追随
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "如果你把注意力放在竞争对手身上，那你绝不会实现真正的创新。……为你的竞争对手骄傲吧，但不要追随他们。"
  summary: |
    竞争对手只用来保持警醒，不用来定义路线；为他们的成功高兴，把时间花在别人尚未想到的事上。
  tags: [principle, strategy, competition]

- id: p62
  title: 战略从"5 年后世界"倒推
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的（埃里克的战略会议笔记）
  source_quote: |
    "先想想看，5年后世界会是什么情形？然后以此为基点，往前推算。对于那些你推断必定会发生变化的因素多加留心，
    尤其是受科技驱使而使成本曲线下降的生产要素。"
  summary: |
    制定战略的第一步不是盘点现状，而是想象 5 年后的世界，再倒推今天该做什么；盯住必然变化的要素。
  tags: [principle, strategy, future]

- id: p63
  title: 把大部分时间花在产品和平台上
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的（埃里克的战略会议笔记）
  source_quote: |
    "你需要靠产品和平台制胜。所以，你应该把大部分时间用来考虑产品和平台。"
  summary: |
    信息触手可及、资金来源广泛的时代，战略时间预算的大头应给产品与平台，而非渠道与关系。
  tags: [principle, strategy, product]

- id: p64
  title: 面对挑战者：无视只短期有效
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的（埃里克的战略会议笔记）
  source_quote: |
    "无视挑战者的做法只会在短期内有效，如果你选择的是并购或创建，你必须对挑战者的技术洞见和进攻套路了如指掌。"
  summary: |
    应对破坏者的决策规则：无视是短期止痛；要并购或自建对抗，就必须先吃透对方的技术洞见与打法。
  tags: [principle, strategy, disruption]

- id: p65
  title: 战略讨论禁用市场调查与幻灯片
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的（埃里克的战略会议笔记）
  source_quote: |
    "不要使用市场调查和竞争者分析。幻灯片会扼杀讨论，应该从与会人员那里听取意见。"
  summary: |
    战略会靠人与人的观点交锋推进：不投市场报告，不播幻灯片，直接听在场创意精英的判断。
  tags: [principle, meeting, strategy]

- id: p66
  title: 战略迭代必须快速且以研究为基础
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的（埃里克的战略会议笔记）
  source_quote: |
    "迭代对战略至关重要。迭代必须快速，且必须以研究为基础。"
  summary: |
    战略不是一次性定稿的文件：快速循环修订，每轮修订由新的事实研究驱动。
  tags: [principle, strategy, iteration]

- id: p67
  title: 慎选共同制定战略的人
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的（埃里克的战略会议笔记）
  source_quote: |
    "请务必慎重选择那些与你一起制定战略的人。你不应该只看谁与你共事的时间长，也不应该只看谁的头衔大，
    而应当选择能力最强的创意精英。"
  summary: |
    战略班底按"能力 × 对未来改变的见解"遴选，资历和头衔不作数。
  tags: [principle, strategy, talent]

- id: p68
  title: 招聘是管理者最重要的工作
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "对于管理者而言，'工作中最重要的事情'是招聘人才。……物色人才好似刮胡子：如果你不每天下功夫，别人就会看出来。"
  summary: |
    把招聘当作日常核心职责持续投入，像教练物色运动员一样亲自上；不是人力资源部的杂务。
  tags: [principle, talent, hiring]

- id: p69
  title: 职位越高越要亲自抓招聘
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "在多数企业中，高管职位越高，对于招聘事宜越是不管不问。但实际上，这样的做法是本末倒置。"
  summary: |
    反转常见行为：高管亲自读简历、主持面试、填反馈表；把招聘下放给助理等于放弃最重要的职责。
  tags: [principle, talent, hiring]

- id: p70
  title: 摒弃层级招聘制，由委员会定夺
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "应该摒弃层级制，招聘结果应该通过同事评估、由委员会来定夺。……创意精英们比具体职位更重要，公司比经理人更重要。"
  summary: |
    录用权从用人经理手里收走，交由同事评估委员会，防止经理因私心拒绝比自己强的人。
  tags: [principle, talent, hiring-committee]

- id: p71
  title: 没有空缺也要招最优秀的人
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "招聘目的应是尽可能吸引最优秀的人才，即便暂时没有与此人经验相匹配的空缺职位也应如此。"
  summary: |
    招聘以人而非岗位为单位：遇到顶尖人才先招进来，再为其创造位置；宁人浮于位，不错过俊杰。
  tags: [principle, talent, hiring]

- id: p72
  title: 羊群效应：起点就定高标准
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "A级人才大多会招聘A级人才，但B级人才却不仅会招聘B级人才，还会招来C级和D级人才。……
    应该从一开始就设置较高的招聘标准，这样才能吸引高水平人才。"
  summary: |
    招聘质量是自我强化的：第一次打折就会滑向 B/C/D；早期把标准定到最高，让优秀吸引优秀。
  tags: [principle, talent, quality-bar]

- id: p73
  title: 产品人员的招聘务必最严格
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "在产品人员的招聘过程中务必严格把关，如果你能确保产品这一企业核心部门的人员的质量，
    这种卓越的质量便会感染其他团队。"
  summary: |
    质量标准从核心部门向外辐射：产品团队绝不让步，其他团队的门槛自然被拉高。
  tags: [principle, talent, quality-bar]

- id: p74
  title: 警惕把"激情"挂嘴边的人
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "如果一个人一张口就大肆强调'我是个对……很有激情的人'，接下来又讲到旅游、足球或家庭这种非常空泛的话题，
    那么你就应提高警惕。"
  summary: |
    真激情体现在坚持与行动里，不在自我标榜里；听应聘者谈具体追求时的眼睛是否发亮。
  tags: [principle, talent, interview]

- id: p75
  title: 雇用比你聪明的人
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "请务必雇用那些比你聪明的人。……我们希望你在招聘时不要太看重应聘者掌握了多少知识，
    而要重视他们尚未开发的潜力。"
  summary: |
    招人只招让自己变强的人；衡量的是智力与潜力（应对指数级变化的能力），不是现有知识存量。
  tags: [principle, talent, hiring]

- id: p76
  title: 雇用学习型动物
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "我们理想的应聘者，都是那些勇于乘坐过山车且学习不辍的人。这些'学习型动物'不仅有处变不惊的智慧，
    也有乐于享受变化的心态。"
  summary: |
    招聘画像的核心维度：成长型思维 + 对学习如饥似渴；他们不怕问蠢问题、不怕得到错答案。
  tags: [principle, talent, hiring]

- id: p77
  title: 勿偏重专业经验而忽视智慧
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "偏重专业而忽视智慧的做法完全是本末倒置，在高科技行业更是如此。……雇用专家会留下隐患……
    而聪明的通才不存在偏见。"
  summary: |
    按职位经验招人会招来专家偏见；在变动的行业里，聪明的通才比资深专家更值钱。
  tags: [principle, talent, hiring]

- id: p78
  title: 用"错失的机遇"之问检验学习力
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "他会问应聘者：'1996年互联网发展浪潮中，你错失了哪些机遇？你做对了什么？做错了什么？'……
    这个问题也可以用于近期发生的任何大事上。"
  summary: |
    让应聘者剖析错失的浪潮并承认具体错误，看其如何从失误中成熟；这题没法用套话应付。
  tags: [principle, talent, interview]

- id: p79
  title: 招进来后让学习型动物继续学习
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "在把学习型动物招入公司之后，请让他们继续学习！为每位员工创造不断学习新东西的机会。"
  summary: |
    学习机会本身就是留住学习型动物的待遇：哪怕与本职无关的技能也要让他们接触并实践。
  tags: [principle, talent, learning]

- id: p80
  title: 机场测试
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "想象一下，你要与一位同事一起在机场里因飞机延误而待上整整6个小时。你能与他开心聊天打发时间吗？"
  summary: |
    终极共事自检：航班延误 6 小时时你愿意真的坐下来和这位（前）同事聊天吗？把"谷歌范儿"纳入面试评分。
  tags: [principle, talent, hiring]

- id: p81
  title: 博兹沃茨法则：看他对助理的态度
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "通常，我们都会询问助理对应聘者的看法，也会听取他们的意见。姑且把这叫作'博兹沃茨法则'吧。"
  summary: |
    品行看细节：观察应聘者对待服务生、行政助理的方式，并正式征询助理的意见作为录用参考。
  tags: [principle, talent, interview]

- id: p82
  title: 避免千篇一律，拥抱观点多样性
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "和不喜欢的人共事不可避免，因为一家公司的全体员工不应该千篇一律，千篇一律恰恰是失败的温床。……
    观点多样性是你最好的法宝。"
  summary: |
    不必喜欢每位同事，但必须接纳与自己不同的人；多元背景是防止集体盲区的商业武器。
  tags: [principle, talent, diversity]

- id: p83
  title: 进门前抛掉偏见，以事实评判人才
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "在准备面试时，请务必在进门前把你的偏见抛到一边。……我们无法强迫自己摒除对性别、种族以及肤色等因素的偏见，
    因此，我们应建立以事实为准的客观方式来评判人才。"
  summary: |
    承认偏见无法自除，所以用统一的客观标准与数据（而非印象）评估所有应聘者。
  tags: [principle, talent, objectivity]

- id: p84
  title: 加大光圈甄才
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "有洞见的管理者会把光圈调大，将那些被一般标准排除在外的人也纳入考虑范围。"
  summary: |
    物色人选时放宽筛选条件：纳入跨领域转岗者、无经验的高潜力者；愿意冒险任用才能得到非凡之才。
  tags: [principle, talent, sourcing]

- id: p85
  title: 用职业发展趋势衡量人选
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "最优秀的人才通常是那些职业生涯处在上升阶段的人，因为如果顺着他们的职业趋势向前推，
    你会发现他们非常有潜力获得成长和成功。"
  summary: |
    看轨迹而非看峰值：上升期的人未来产出高，已到瓶颈期的资深者可预测但难有惊喜。
  tags: [principle, talent, sourcing]

- id: p86
  title: 为高层选人勿迷信相关经验
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "科技已经使得当今多数行业环境充满了变数，拥有相关工作经验已不再是成功的保证。……
    他们应该把注意力放在创意精英的能力上。"
  summary: |
    高管招聘的最大陷阱是按经验划线；谷歌的 CFO、法务总顾问都来自"毫无相关经验"的高能力者。
  tags: [principle, talent, hiring]

- id: p87
  title: 全员出动招募人才
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "物色人选人人有责，这个洞见需要渗透到企业深层。招聘官管理招聘流程，但人人都应参与到招聘工作中来。"
  summary: |
    招聘不是招聘官的独角戏：把物色人才写进每个人的职责，防止招聘官用平庸者充数。
  tags: [principle, talent, sourcing]

- id: p88
  title: 把招聘纳入每个人的考核
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "要把招募人才纳入每位员工的职责，并进行评估。……然后，在评估业绩和提拔员工时将这些数据作为参考。"
  summary: |
    统计每人举荐与参与面试的次数、反馈质量，并计入绩效与晋升评估——招聘才真正成为全员的事。
  tags: [principle, talent, performance]

- id: p89
  title: 面试是最重要的商务技能
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "对于商务人士而言，最重要的技能是面试技巧。"
  summary: |
    识别人才的技能是管理者的第一技能；抓住一切面试机会练习，用面试官委员会等机制专精化。
  tags: [principle, talent, interview]

- id: p90
  title: 面试前必须做足功课
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "要想成功组织面试，就必须做好准备。……最重要的，是要细心斟酌你的面试问题。"
  summary: |
    研究应聘者的履历与业绩、预设计挑战性问题；临时翻简历开场的面试必然失败。
  tags: [principle, talent, interview]

- id: p91
  title: 面试的目标是找到对方的局限
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "你的目标不是要进行一次礼貌的谈话，而是找到此人的局限，即便如此，面试过程也不应太过紧张。"
  summary: |
    面试不是寒暄而是探边界：问题开放、留反驳余地，看对方如何捍卫观点、局限在哪里。
  tags: [principle, talent, interview]

- id: p92
  title: 问领悟，不听复述
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "不要只让对方干巴巴地复述自己的经历，而是要让对方分享从经历中获得了什么样的领悟。"
  summary: |
    用"你经历过哪些出乎意料的事"之类的问题逼出思想；简历复述式回答视为无效信息。
  tags: [principle, talent, interview]

- id: p93
  title: 用情景题看授权风格
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "'当你遭遇危机，或是需要做出一个重大决断的时候，你会怎么应对？'……可以让你看出对方是那种
    '自己动手，丰衣足食'的类型，还是喜欢依靠他人帮助的类型。"
  summary: |
    借假设情境判断资深候选人是控制型还是信任型：亲力亲为者难容优秀下属，借力者更容易建强团队。
  tags: [principle, talent, interview]

- id: p94
  title: 注意面试前后的表现
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "你必须保持敏锐的观察力，尤其要注意对方在正式面试开始之前和之后的表现。"
  summary: |
    正式问答之外才是真实人格：等待时、闲聊时、以为没人看时的举止都计入评估。
  tags: [principle, talent, interview]

- id: p95
  title: 珍视提出深刻问题的应聘者
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "你不仅需要斟酌你提出的问题，也要留意那些提出深刻问题的应聘者。这些在提问时语出惊人的人充满了好奇心。"
  summary: |
    候选人反向提问的质量是好奇心的直接证据；面试是双向审视，他们也在考察你。
  tags: [principle, talent, interview]

- id: p96
  title: 面试时间设为 30 分钟
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "有谁规定面试时间必须要持续一个小时？走进面试现场不过几分钟，你往往就能判断出应聘者于这家公司和这项工作都不适合。
    ……正因如此，谷歌的面试只有半个小时。"
  summary: |
    默认面试时长 30 分钟：不合适的人不必苦挨到钟点，合适的人随时加面；时间紧反而逼出干货。
  tags: [principle, talent, interview]

- id: p97
  title: 每位应聘者至多 5 位面试官
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "在4次面试之后，面试官的人数每增加一位，只能为面试决策的准确度带来不到1%的提高。……
    我们规定，每位应聘者至多只能接受5位面试官的面试。"
  summary: |
    用数据设面试上限：5 位封顶，超过后边际价值趋近于零，只会拖慢流程折磨候选人。
  tags: [principle, talent, interview]

- id: p98
  title: 面试官必须有自己的主张
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "如果单个面试官打出了3分，这便是逃避的表现。因为这个数字说明这位面试官不置可否，推卸责任。……
    面试官必须要有自己的明确立场。"
  summary: |
    禁止骑墙评分：要么坚定推荐（愿为这个人辩护），要么明确否决；平均分是失职。
  tags: [principle, talent, interview]

- id: p99
  title: 四维统一评价标准
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "在谷歌，我们从四个方面对应聘者做出评价……领导力……职务相关知识……一般认知能力……谷歌范儿。"
  summary: |
    对所有职能与级别用同一套四维评分：领导力、职务相关知识、一般认知能力、谷歌范儿（个性与文化契合）。
  tags: [principle, checklist, talent]

- id: p100
  title: 招聘委员会：用人经理有否决权无决定权
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "谷歌特地成立了招聘委员会来做招聘决策。委员会的决策以数据为根据……用人部门的经理虽然没有招聘决定权，
    却手握一票否决权。"
  summary: |
    录用决策由 4-5 人、观点多样的委员会按数据作出；部门经理可以否决但不能独断，防止山头化。
  tags: [principle, talent, hiring-committee]

- id: p101
  title: 信息包是唯一依据
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "信息包是招聘委员会唯一可用的信息来源，这也是一条非常重要的准则。信息包里不包含的内容，一律不予考虑。"
  summary: |
    决策只认书面信息包：想影响结果就写进包里，别指望会上口才；标准化的信息包保证全员同等信息。
  tags: [principle, talent, hiring-committee]

- id: p102
  title: 观点必须用事实支撑
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "仅仅表达自己的观点是不够的，你必须用事实支撑你的观点。……凡是不包含具体资料的招聘信息包，
    委员会都不会予以考虑。"
  summary: |
    面试反馈不许写"他很聪明"：每个结论都要附具体观察或数据；无事实支撑的意见不进决策。
  tags: [principle, talent, evidence]

- id: p103
  title: 升职决策也交委员会
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "升职决策也应该由委员会定夺，而不应该对管理层的意见言听计从。"
  summary: |
    与招聘同理：晋升事关全公司，由委员会按数据定夺，顺带替管理者省去当面回绝的尴尬。
  tags: [principle, talent, promotion]

- id: p104
  title: 宁缺毋滥
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "招聘中有一条黄金法则是不可违背的，那就是：宁缺毋滥。如果质量和速度不可兼得，那质量一定要放在首位。"
  summary: |
    招聘的唯一黄金法则：任何情况下质量优先于速度；空着的岗位好过凑数的员工。
  tags: [principle, talent, quality-bar]

- id: p105
  title: 宁"漏聘"不"误聘"
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "我们宁愿'漏聘'（也就是没有招聘那些应该招聘的人），也不愿意'误聘'（也就是把那些不该招入企业的人招进来）。"
  summary: |
    在拿不准时选择不录：漏掉的损失有限，误聘的解雇成本与团队污染远更高；自检"换掉最差10%能否改善"。
  tags: [principle, talent, hiring]

- id: p106
  title: 给优秀人才超出常规的回报
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "如果你希望顶尖的员工能拿出更加优异的表现，那就用超出常规的薪酬来做嘉奖和激励吧。"
  summary: |
    创意精英与运动员一样能产生杠杆式影响：对做出超常规贡献者给超常规报酬，不看职级看影响。
  tags: [principle, talent, compensation]

- id: p107
  title: 薪酬起点放低，按影响付薪，打破平均主义
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "你的薪酬曲线的起点应当放低一些。……不要在发薪和提拔人才上本着'人人平等'的洞见。……
    最高的报酬理应属于那些与卓越产品和伟大创意关系最密切的人。"
  summary: |
    入职时钱不是核心卖点；入职后按影响拉开差距——低职级的关键贡献者理应比高职级平庸者挣得多。
  tags: [principle, talent, compensation]

- id: p108
  title: 换出巧克力，留下葡萄干
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "如果你逼迫他们把自己团队中的成员轮换出来，他们便会想把巧克力留给自己，而把葡萄干换给别人。……
    希望管理者能把他们的巧克力换给他人，把葡萄干留给自己。"
  summary: |
    轮岗的隐藏失败模式是管理者藏优推劣；监控轮换名单，确保被轮出去的是团队里的佼佼者。
  tags: [principle, talent, rotation]

- id: p109
  title: 用新挑战留住人才，为其创造职位
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "想要留住创意精英，最好的方法就是避免让他们太过安逸，而是不断用新的想法保持他们工作的趣味性。"
  summary: |
    留人靠持续的新趣味与挑战：列席管理会议、轮值主席、为其量身造岗——公司可以为了人才自我调整。
  tags: [principle, talent, retention]

- id: p110
  title: 挽留人才先倾听
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "想要挽留人才，你首先要学会倾听。你的员工希望有人能听取他们的意见，他们希望能融入企业之中，也希望得到应有的重视。"
  summary: |
    挽留对话从倾听离职动因开始，帮对方把眼光放长远、算清机会成本，而不是急着喊"留下吧"。
  tags: [principle, talent, retention]

- id: p111
  title: 听取离职者的"电梯演讲"
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "顶尖的创意精英之所以考虑离职，是因为他们想要自立门户。不要打击他们的积极性，而要主动听取他们的'电梯演讲'。"
  summary: |
    对想创业的员工：听其构想，若不成熟就建议边工作边完善；拿出可投资的方案再送行，甚至投钱。
  tags: [principle, talent, retention]

- id: p112
  title: 面对最后通牒，一小时内出手
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "如果你还想给出更好的待遇条件来试着挽留，那你出手一定要火速（间隔时间最好不要超过一个小时）。
    因为时间一长，这位员工在心中就越发倾向于那家新的公司了。"
  summary: |
    挽留窗口以小时计：要么迅速给出对等反报价，要么干脆放手；拖延只会把人心推向对方。
  tags: [principle, talent, retention]

- id: p113
  title: 爱他就让他走
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "如果员工的离职对于个人发展的确是正确的选择，那就让他走吧。……对他的新工作表示祝贺，
    并欢迎他加入你们公司的离职员工交流群。"
  summary: |
    挽留失败就体面送行：祝贺并把对方纳入离职员工网络，把关系延续到公司围墙之外。
  tags: [principle, talent, alumni]

- id: p114
  title: 防范以解雇为乐的人
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "世界上有一些人以炒别人的鱿鱼为乐。请注意防范这种人……'解雇他们就行了'这句话，
    只是那些不愿在人才招聘上下功夫的人用来规避责任的借口。"
  summary: |
    把"解雇"当管理工具的人是文化毒药；听到"招错了大不了解雇"这类话，先追问其招聘投入。
  tags: [principle, talent, warning]

- id: p115
  title: 谷歌招聘之行为准则（清单）
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "雇用那些比你更聪明、更有见识的人。不要雇用那些不能让你有所收获也不能对你构成挑战的人。……
    务必雇用优秀的候选人。宁缺毋滥。"
  summary: |
    九组"雇用/不要雇用"对照清单：聪明有见识、为产品文化增值、做实事、自动自发、启发他人、共同成长、
    多才多艺、道德坦诚，最后落到宁缺毋滥。
  tags: [checklist, talent, hiring]

- id: p116
  title: 职业选择如冲浪：先选行业再选公司
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作（职业建议）
  source_quote: |
    "在职业生涯的起点，这样的排序恰恰是本末倒置。……选择好行业才是重中之重。把行业视为你冲浪的地点，
    把公司当成你赶上的海浪。"
  summary: |
    个人职业决策规则：行业（浪）大于公司（板）；在起飞的行业里，入错公司也比入错行伤害小。
  tags: [principle, career]

- id: p117
  title: 挑公司听科技达人的
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作（职业建议）
  source_quote: |
    "在挑选公司的时候，听听那些真正懂行的科技达人的意见。这些天才级的创意精英可以比常人更早预测出科技的走向。"
  summary: |
    用"最聪明的人往哪里去"作为选公司信号：科技达人的职业去向是行业前景的先行指标。
  tags: [principle, career]

- id: p118
  title: 规划 5 年后的简历，目标要够不着
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作（职业建议）
  source_quote: |
    "如果你通过总结发现自己已经达到了理想工作的要求，就说明你的规划不够大胆。不妨重新开始规划，
    设定一份需要努力争取而非唾手可得的理想工作。"
  summary: |
    职业规划操作法：写出 5 年后理想职位的招聘广告与简历，倒推差距；目标一步能到说明定低了。
  tags: [principle, career, planning]

- id: p119
  title: 学统计学：数据是 21 世纪的利剑
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作（职业建议）
  source_quote: |
    "数据的民主化意味着，擅长分析数据的人是这个时代的赢家。数据是21世纪的利剑，谁是舞剑好手，谁就是当代的剑侠。"
  summary: |
    个人能力投资方向：与廉价化要素（数据、计算）配套的分析技能；不会算，至少学会提出好问题并善用答案。
  tags: [principle, career, data]

- id: p120
  title: 靠阅读加深行业理解
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作（职业建议）
  source_quote: |
    "要在某个行业里脱颖而出，最简便有效的方法，是加深对行业的理解。要加深理解，最好的方法莫过于阅读。"
  summary: |
    把行业顶级文字资料（含公司战略文件）系统读完；说自己没时间阅读，等于说不想理解自己的行业。
  tags: [principle, career, learning]

- id: p121
  title: 练好 30 秒电梯演讲
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作（职业建议）
  source_quote: |
    "你不仅要阐述你的项目内容、背后的技术洞见、你是如何衡量成功的……做好功课，多多练习，这样，你的演讲才有说服力。"
  summary: |
    随时能用 30 秒讲清项目、技术洞见、成功衡量与公司利益关联；这是职场人的必备肌肉。
  tags: [principle, career, communication]

- id: p122
  title: 出国去
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作（职业建议）
  source_quote: |
    "业务永远向全球扩展，但人却天生具有地域性。因此，无论你身在哪里、来自何处，
    你都应该抓住一切机会走出去，到不同的地方工作和学习。"
  summary: |
    主动寻求跨国项目或旅行，用消费者的视角观察他乡；哪怕与出租车司机的一席谈也可能是战略灵感。
  tags: [principle, career, learning]

- id: p123
  title: 从事富有激情的事业
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作（职业建议）
  source_quote: |
    "人生最大的奢侈，莫过于从事富有激情的事业。这也是一条通往幸福的清晰路径。"
  summary: |
    职业路径的终极校准问题：你热爱的才能做出最好成果；找不到就先调整方向缩短与它的距离。
  tags: [principle, career, passion]

- id: p124
  title: 决策的方式、时机与实施同等重要
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "在制定决策的时候，不能一心只想做出正确的决定。制定决策的方式、时机和实施决策的具体方法，
    与决策本身同样重要。"
  summary: |
    评估决策时把过程纳入：一个"对"的决定若方式粗暴、时机不当，落地效果等同于错的决定。
  tags: [principle, decision]

- id: p125
  title: 用数据做决策，以数据开场
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "在交流意见和讨论观点时，我们会以公布数据的方式作为会议的开场。我们不希望以'我觉得'这句话来服人，
    而是用'请看数据'这句话来服人。"
  summary: |
    "少了数据，你就没法做出决定"：会议以投屏数据开场，论点必须挂在数据上而非职位或直觉上。
  tags: [principle, decision, data]

- id: p126
  title: 幻灯片是数据的载体，不是论点的主宰
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "幻灯片不应被用来主导会议或论点的走向，而应作为数据的载体，以便让每个人都能接触到相同的数据。"
  summary: |
    演示材料的正确角色：让所有人看到同一份事实基础；数据错了再花哨的片子也没用。
  tags: [principle, meeting, data]

- id: p127
  title: 信赖一线员工对数据的掌握
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "最了解数据的人，是那些工作在第一线的员工，而往往不是管理层。……收入能解决一切问题。"
  summary: |
    领导者不要在细节里迷路：最懂数据的是一线，财务讨论盯住收入等真问题而非 EBITDA 黑话。
  tags: [principle, decision, data]

- id: p128
  title: 谨防"摇头娃娃"附和
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "如果会议上所有人一致点头，这并不意味着大家意见一致，而只是说明你下面坐了一群'摇头娃娃'。"
  summary: |
    全场一致是危险信号而非胜利信号：点头的娃娃出门就会反对执行；必须逼出真实异议。
  tags: [principle, decision, warning]

- id: p129
  title: 共识≠人人同意
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "'共识'并不是指人人都必须同意，而是指共同达成对公司最有利的决策，并围绕决策共同努力。"
  summary: |
    共识的正确打开方式：人人充分发言、分歧充分交锋，最后人人愿意挺身支持同一决定。
  tags: [principle, decision, consensus]

- id: p130
  title: 负责人不要先亮明立场
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "如果你是负责人，那么请注意，不要在会议一开始就申明自己的立场。你的任务，是抛开大家的职位差异，
    鼓励每个人发表自己的观点。"
  summary: |
    主持决策讨论时藏起自己的倾向：先表态等于给讨论定调，众人只会附和。
  tags: [principle, decision, facilitation]

- id: p131
  title: 点出沉默者，让异议早现形
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "特别要注意那些三缄其口的人，把那些还没发言的人点出来。……你应该一开始就尽力让可能出现的异议'现形'。"
  summary: |
    主动点名让未发言者表态；异议必须赶在决策期限逼近前暴露，否则会被合理地排斥。
  tags: [principle, decision, dissent]

- id: p132
  title: 要正确的决策，不要人人同意的最低标准
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "最好的决策应该是正确的决策，而不是竭力争取大家一致同意而找出的最低标准，也未必是领导人自己的决策。"
  summary: |
    共识流程的靶心是"对公司最有利"：既不是折中方案，也不是领导偏好，谁对跟谁走。
  tags: [principle, decision, consensus]

- id: p133
  title: 该响铃时就响铃
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "对于决策者而言，最重要的任务就是：设立最后期限，进行决策工作，按最后期限完成。"
  summary: |
    讨论像课间玩耍没有铃就不会停：决策者必须设时限、按时限拍板，超过一定度的分析不再提升决策质量。
  tags: [principle, decision, deadline]

- id: p134
  title: 别成为紧迫感的奴隶
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "把乐于行动的劲头拿出来，中止没有意义的讨论和分析，让团队行动起来……但要注意，不要成为紧迫感的奴隶。
    在最后一刻来临之前，都要保持灵活变通。"
  summary: |
    响铃是手段不是目的：期限前保持开放，期限一到果断；行动偏好与耐心要靠时机拿捏平衡。
  tags: [principle, decision, timing]

- id: p135
  title: PIA 谈判准则：耐心、信息、备选方案
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "所谓'PIA'，就是要有耐心（patience）、信息（information）以及备选方案（alternatives）。
    其中，耐心尤其重要：在决心采取行动之前，应该尽可能长时间地静观其变。"
  summary: |
    高风险谈判/决策前的三项自检：我还有耐心吗？信息够吗？备选方案在哪？能等就尽量等。
  tags: [principle, negotiation, checklist]

- id: p136
  title: 少做决策
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "其实，你就不应该多做决策。你的任务，就是分析数据、鼓励讨论、引导大家达成共识，凭借你过人的才识做出决策。"
  summary: |
    管理者的产出不是决定数量：把决策尽量交出去，自己只保留少数真正需要高层拍板的事项。
  tags: [principle, decision, delegation]

- id: p137
  title: 判断何时出马、何时放权
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "首席执行官或企业高管必须磨炼的一项重要技能，就是判断何时该自己出马、何时该把决策权交给别人。"
  summary: |
    CEO 只保留产品发布、并购、公共政策等关键决策权，其余放给其他领导者，仅在其严重失误时介入。
  tags: [principle, decision, delegation]

- id: p138
  title: 决策足够重要就每天开会
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "如果决策足够重要，应该每天开会。这样的会议频率，可以让大家明白眼前的决策有多么关键。"
  summary: |
    对关乎存亡的决策用"每日同题会议"加压：既标记重要性，又省去重复背景的时间，逼出深度分析。
  tags: [principle, decision, meeting]

- id: p139
  title: 奥普拉法则：晓之以理更要动之以情
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "如果你想改变他人，不仅要晓之以理，更要学会动之以情。我们把这称为'奥普拉·温弗瑞法则'。"
  summary: |
    只有论据赢不了落实：要让人们从感情上接受一个自己不同意的决定，先让其感到被倾听和被重视。
  tags: [principle, decision, communication]

- id: p140
  title: "你们两边说得都对"
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "'你们两边说得都对'这句话就能派上用场。……必须让相关人员要么保留异议、服从决定，要么就公开向上级汇报。"
  summary: |
    拍板后先肯定败方的可取之处，再给两条明路：留下执行（disagree and commit），或公开向上申诉。
  tags: [principle, decision, consensus]

- id: p141
  title: 会议准则（清单）
  type: principle
  source_chapter: 第四章 决策：共识的真正含义（每场会议都需要有主人）
  source_quote: |
    "会议应该有一位决策者或主持。……决策者应当亲力亲为。……会议应该很容易取消。……会议规模应以便于管理为宜。
    ……守时很重要。……开会时就认真开会。"
  summary: |
    八条会议纪律：每会必有一主；决策者提前24小时发议程、48小时内发决议与待办；目标不明即取消；
    与会者不超8人（10人为上限）；不必要就退场；准时开始结束；会中不摸鱼。
  tags: [checklist, meeting]

- id: p142
  title: 马背原则：环视四周，继续上路
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "我们只需坐在马背上（这通常只是打比方），快速环视四周，然后继续上路。……不要认为你每次都需要从马上跳下来，
    用几周的时间拟出一份50页长的法律声明。"
  summary: |
    在高速环境中带着不完全信息行动：快速判断、给出指引、事成之后继续赶路，别事事做完美分析。
  tags: [principle, decision, speed]

- id: p143
  title: 律师必须是团队一员
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "要想'马背原则'奏效，你们的律师必须是商业团队及产品团队的一员，而不能是那种偶尔被叫来'救火'的人。"
  summary: |
    马背原则的适用前提：法务等支持职能必须嵌进业务团队，从事后审查者变为同行决策者。
  tags: [principle, organization, legal]

- id: p144
  title: 把 80% 的时间花在 80% 的收入上
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "把80%的时间花在80%的收入上。……必须把注意力和热情都集中在核心业务上。"
  summary: |
    管理者最重要的决策是时间分配：光鲜的新业务再有趣，赢利靠核心业务，先喂饱核心再谈新欢。
  tags: [principle, time-management, core-business]

- id: p145
  title: 接班人计划：找 10 年后的接班人
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "正确的做法，是集中注意力寻找那些已经崭露头角、升职速度快的杰出创意精英。问问自己：
    这其中有人具备在10年后运营公司的能力吗？"
  summary: |
    热爱事业就要为离开做规划：盯升职最快的高潜力人才，给足待遇与发展，防止其停滞或跳槽。
  tags: [principle, succession, talent]

- id: p146
  title: 领导者需要自己的教练
  type: principle
  source_chapter: 第四章 决策：共识的真正含义
  source_quote: |
    "作为企业领导者，你需要自己的教练。"
  summary: |
    最顶尖的运动员都有教练，高管更不该例外；管理是可习得的技能，前提是学生愿意倾听和学习。
  tags: [principle, leadership, coaching]

- id: p147
  title: 当最牛的路由器：默认共享一切
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "现在，最有能力的管理者不但不独霸信息，还会分享信息。……领导者的目标，就是要时刻促进信息在整个企业中的流动。"
  summary: |
    把"被人讥为路由器"变成荣誉：信息的默认状态是流动而非囤积，管理者的价值在于让信息畅通。
  tags: [principle, communication, transparency]

- id: p148
  title: 共享一切：剔除信息者必须举证
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "'共享一切'并不意味着'先剔除那些有可能损害公司形象或打击士气的信息，然后把剩下的信息进行共享'，
    而是指'除了极少数有违法律法规的信息，其他一概与大家共享'。"
  summary: |
    透明规则的举证责任倒置：不是证明"为什么可以共享"，而是要给出"为什么不能共享"的具体理由。
  tags: [principle, communication, transparency]

- id: p149
  title: 掌握细节：10 秒规则
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "如果业务负责人不能在10秒钟内把遇到的重大困难流畅地说出来，那么此人就不胜任。如今，'事不关己'的管理方法
    已经不再适用，作为管理者，必须掌握细节。"
  summary: |
    用"10 秒内说出最大困难"现场检验业务负责人；管理者必须掌握细节，不能当甩手掌柜。
  tags: [principle, management, detail]

- id: p150
  title: 掌握细节更要掌握真相
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "埃里克掌握了细节，但拉里却掌握了真相。因此，不能只见树木不见森林。"
  summary: |
    中层会过滤信息：用"每周摘要"等直达一线的工具交叉验证，别把从管理者处听来的当成全部事实。
  tags: [principle, communication, ground-truth]

- id: p151
  title: 为讲真话营造安全的环境
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "好消息放到明天一样好，坏消息留到明天则会变得更坏。正因如此，即便忠言逆耳，
    你也必须营造一个让大家时时敢于提出难题和发表忠言的环境。"
  summary: |
    坏消息的金丝雀是资产不是威胁：建立让员工敢提尖锐问题、敢报忧的机制，并奖励报忧者。
  tags: [principle, communication, candor]

- id: p152
  title: 项目之后开"事后讨论会"并公布结果
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "在产品或重要功能问世时，我们会要求各团队组织'事后讨论会'，让全体成员聚在一起讨论哪些做对了，哪些做错了。
    之后，我们会公布讨论结果。"
  summary: |
    每次重要发布后强制复盘：做对与做错并陈，结果全员可见；复盘的最大收获是公开透明的过程本身。
  tags: [principle, learning, retrospective]

- id: p153
  title: 多莉机制：尖锐问题逐一回答
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "任何人都可以把最尖锐的问题直接抛给首席执行官和他的团队……无论问题尖锐与否，
    他们都得把列出的问题从头至尾逐一回答。"
  summary: |
    向上提问的民主化：匿名提交、全员投票排序，高管必须照单全答；用红绿牌评判回答是否有保留。
  tags: [principle, communication, mechanism]

- id: p154
  title: 爬升—报告—遵从：善待带来坏消息的人
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "如果有人带着坏消息或难题来找你，这就说明他们正处于'爬升——报告——遵从'模式。……
    为了鼓励他们说出问题，你应当用心倾听、竭力相助。"
  summary: |
    对报告问题的人先谢后查：他们已完成分析并主动暴露风险；处置坏消息的方式决定下次还有没有人报。
  tags: [principle, communication, candor]

- id: p155
  title: 制造话题与谈话条件
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "作为领导者，你需要为他们提供帮助。……领导者如果能将初入企业的创意精英介绍给这些资深者，
    就搭起了一道最有意义的桥梁。"
  summary: |
    谈话不会自动发生：用集体观影、公开"使用说明书"、接访时间等制造话题和渠道，并主动为新人牵线元老。
  tags: [principle, communication, facilitation]

- id: p156
  title: 祷文不会因重复而失色
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "在生活中，很多情况下一件事情需要重复大约20遍才能被人真正听进去。……作为领导者，
    你必须习惯于苦口婆心、诲人不倦。"
  summary: |
    核心理念要说到自己都觉得腻（约 20 遍）别人才开始听；重复是领导职责，不是沟通失败。
  tags: [principle, communication, repetition]

- id: p157
  title: 重复无效时，先查理念
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "如果你把某句话重复了20遍，别人却仍然听不进去，那么问题就不在于你的沟通方式，而是在于你所传达的理念。……
    你的计划有瑕疵。"
  summary: |
    沟通失灵的诊断规则：反复讲仍无人认同，说明不是话术问题，而是战略或理念本身站不住。
  tags: [principle, communication, diagnosis]

- id: p158
  title: 信息轰炸七原则（清单）
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "1.沟通能否强化你希望深入人心的核心理念呢？……2.沟通有效吗？……3.沟通是否有趣、鼓舞人心？……
    4.沟通是否发自肺腑？……5.沟通对象是否合适？……6.你使用的沟通媒介合适吗？……7.诚实谦虚，积攒人品。"
  summary: |
    发送任何信息前的七问：强化核心理念？有新内容？有趣鼓舞？真情实感？对象精准？媒介合适？诚实谦虚？
  tags: [checklist, communication]

- id: p159
  title: 用旅行报告作为会议开场
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "在员工外出旅行的时候，让他们整理一篇'暑假游记'式的报告，总结一下自己的见闻和学到的经验。
    然后，会议就以做旅行报告开始。"
  summary: |
    用旅行报告替换例行近况汇报：让会议从人的见闻开始，打破职务边界，人人都能谈全行业。
  tags: [principle, meeting, communication]

- id: p160
  title: 务必确保你愿意为自己工作
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "务必要确保你愿意为自己工作……至少一年一次针对自己的表现写一份评估，然后读一读，
    看看你自己是否愿意接受自己的管理。之后，把这份评估发给你管理的员工。"
  summary: |
    管理学金科玉律：每年写一份自我评估并公开发给下属，主动请求批评，比 360 度测评更见真话。
  tags: [principle, management, self-review]

- id: p161
  title: 电邮常识（清单）
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "1.迅速回复。……2.在写电子邮件的时候，每个字都很重要……3.经常清理收件箱。……4.先处理后收到的邮件。……
    5.不要忘了，你是台路由器。……6.在你使用密件抄送功能时，问问自己为什么要这么做。……7.不要拿邮件泄愤。
    ……8.要方便跟踪进度。……9.帮助未来的你更方便地搜索信息。"
  summary: |
    九条电邮纪律：迅速回复所有人（哪怕只答"明白了"）；字字有用；一次处理完毕；先处理新邮件；
    主动转发有用信息；慎用密送（隐瞒就公开抄送否则别寄）；不拿邮件泄愤；抄送自己跟进；给未来的搜索留关键词。
  tags: [checklist, email, communication]

- id: p162
  title: 一对一会谈：清单对对碰
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器（备一本情境手册）
  source_quote: |
    "管理者应当把最想在会谈中涉及的5件事写出来，员工也应该列一份这样的单子。把两张不同清单拿出来后，
    单子上十有八九会有几个条目是重复的。"
  summary: |
    一对一开场法：双方各写最想谈的 5 件事再对照；重合条目优先解决，完全不重合本身就是最大问题信号。
  tags: [principle, one-on-one, management]

- id: p163
  title: 一对一会谈大纲（清单）
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器（备一本情境手册）
  source_quote: |
    "1. 工作表现……2. 与同事之间的关系……3. 领导与管理……4. 创新（最佳实践）……
    你是否将业界或世界上最顶尖的人或企业作为对比标杆？"
  summary: |
    比尔·坎贝尔的四块会谈大纲：工作表现（销售/交付/质量/预算）、同事关系、领导与管理（指导/清恶棍/招聘/激励）、
    创新（进步、新技术、标杆对比）。
  tags: [checklist, one-on-one, management]

- id: p164
  title: 董事会：要关心，莫插手
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器（备一本情境手册）
  source_quote: |
    "在会议结束时，如果董事会能够支持你提出的战略措施自然是最理想的。要达到这个目的，你就必须在沟通上做到
    百分之百的坦诚。……你应当让大家多质疑、少插手。"
  summary: |
    与董事会的关系定位：成员鼻子进来（知情建言）、手指出去（不插手经营）；换百分百坦诚换支持。
  tags: [principle, governance, board]

- id: p165
  title: 向董事会报忧，坦诚以对
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器（备一本情境手册）
  source_quote: |
    "在董事会上报忧总是要比报喜困难。……因此，最好的解决方法就是诚实以对：我们面前的确有难解的问题，
    如何解决我们心里也没有数。"
  summary: |
    给董事会的材料里"不足"部分花最长准备时间；直说"问题难解、尚无答案"，反而换来真正的帮助。
  tags: [principle, governance, candor]

- id: p166
  title: 董事会只谈战略和产品，否则换人
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器（备一本情境手册）
  source_quote: |
    "董事会成员应该讨论战略和产品，而不是管理方式和诉讼纠纷（如果你的董事会成员不是这样，那你就该考虑换人了）。"
  summary: |
    董事会议程的分配原则：法律与事务性议题压缩给下属委员会 15 分钟概述，正席留给战略与产品讨论。
  tags: [principle, governance, board]

- id: p167
  title: 让创意精英而非公关准备董事会汇报
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器（备一本情境手册）
  source_quote: |
    "组织发言的人并非传播部门或法律部门的人员，而是乔纳森团队中深入参与业务的产品经理。……
    把这个任务委派给传播方面的人员，你就白白浪费了让企业未来的领导者收获实际经验的大好机遇。"
  summary: |
    高规格汇报任务是对创意精英的培训机会：派一线产品经理上台，别外包给公关；他们日后多成大器。
  tags: [principle, governance, talent]

- id: p168
  title: 会外定期电话联络董事
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器（备一本情境手册）
  source_quote: |
    "在不开董事会会议的时候，要定期打电话与董事们联络。"
  summary: |
    董事会关系靠日常维护：会期之外定期通话，不让董事会只在坏消息时见到你。
  tags: [principle, governance, relationship]

- id: p169
  title: 对合作伙伴学外交官：搁置道德评判
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器（备一本情境手册）
  source_quote: |
    "如果要建立有效的合作关系，就必须把你的道德评判搁置起来。……我们不会以其国家的意识形态为基础，
    而是以其实际行动为标准。"
  summary: |
    竞合关系经营术：承认对方理念体系无法根除，以行动而非价值观为评价标准，寻找共同利益推进合作。
  tags: [principle, partnership, diplomacy]

- id: p170
  title: 为最重要的伙伴设双赢专职
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器（备一本情境手册）
  source_quote: |
    "对于最为重要的合作伙伴，我们建议企业派专人来兼顾两方利益：一是要满足合作伙伴的需求，
    二是帮助自己的企业追求利益。"
  summary: |
    关键伙伴关系不要交给天然偏袒己方的销售：设专人同时照顾双方利益，做"双层博弈"的外交官。
  tags: [principle, partnership, role]

- id: p171
  title: 媒体访问：对话而非传话
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器（备一本情境手册）
  source_quote: |
    "一场成功的访谈不应干巴巴地重复营销说辞，而应是一场交流真知灼见的对话。……
    '要做一个有思想的领导者，你就必须有自己的思想。'"
  summary: |
    受访规则：拒绝照本宣科的问题清单，用见解和例证真答问题；没挨过负面评论，说明你没聊到点上。
  tags: [principle, media, communication]

- id: p172
  title: 靠关系而非层级成事
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "当你处于混乱之中的时候，要想把事情做成，唯一的途径就是靠建立关系。"
  summary: |
    混乱是互联网企业的常态（流程顺畅反而说明僵化）；在无层级可查的组织里，事靠人际关系网推动。
  tags: [principle, communication, relationships]

- id: p173
  title: 三周原则：新职位前三周只听不做
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "埃里克遵循'三周原则'，也就是说，在接手新职位的前三周里，你不必做什么。你只需听取大家的心声，
    看看他们的问题和关注点在哪里。"
  summary: |
    接手新角色的前 3 周只听、问、记：了解人、关心人、赢得信任，为日后靠关系成事打地基。
  tags: [principle, onboarding, relationships]

- id: p174
  title: 该赞美时不要吝啬
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "在管理中，人们对赞美的使用不足，也低估了赞美的价值。该赞美的时候，不要吝啬。"
  summary: |
    赞美是被系统性低估的管理工具：成本为零而回报巨大，发现值得表扬的行为立刻说出口。
  tags: [principle, management, praise]

- id: p175
  title: 创新的判据：新颖+出人意料+非常实用
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "如果你的产品只是满足了消费者提出的需求，那么你就不是创新，而只是做出回应。……
    创新的东西不仅要新颖、出人意料，还要非常实用。"
  summary: |
    用三重判据区分创新与回应：满足了用户提出的需求只是回应；渐进改善积累起来也可称"非常实用"。
  tags: [principle, innovation, definition]

- id: p176
  title: Google[x] 三重标准筛选构想（清单）
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（了解环境）
  source_quote: |
    "第一，这个想法必须涉及一个能够影响数亿人甚至几十亿人的巨大挑战或机遇。第二，这个想法必须提供一种
    与市场上现存的解决方案截然不同的方法。第三，将突破性解决方案变为现实的科技至少必须具备可行性。"
  summary: |
    立项前过三关：问题够大（影响数亿人）、方法全新（另辟蹊径而非改良）、技术可行（已存在或指日可待）；不过关就不做。
  tags: [checklist, innovation, moonshot]

- id: p177
  title: 去大市场创新，勿在无人问津处孤军奋战
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（了解环境）
  source_quote: |
    "不要把眼光放在无人问津的市场并在这里孤军奋战。你应当发掘创新的途径，跻身进入大型或有潜力发展壮大的市场上。"
  summary: |
    创新环境的前提是飞速发展且竞争激烈的大市场；市场无人问津多半是撑不起扩张，别把冷清当蓝海。
  tags: [principle, innovation, market]

- id: p178
  title: 首席执行官必须兼任首席创新官
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "单独设立首席创新官的做法行不通，因为这个职位的权力无法营造出原始的混沌（而只有在原始混沌之中，
    才能诞生惊喜）。换句话说，首席创新官的职位需要由首席执行官兼任。"
  summary: |
    创新不可外包给委员会或专职高管：只有 CEO 有权营造混沌、保护自下而上的构想，此职必须亲自兼任。
  tags: [principle, innovation, ceo]

- id: p179
  title: 给创意的人空间而非任务
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "有创意的人不需要别人来布置任务，而需要有人提供空间。"
  summary: |
    创意无法靠指派产生：设创新委员会、下创新指标只会扼杀创意；正确动作是腾出空间与自由。
  tags: [principle, innovation, autonomy]

- id: p180
  title: 把创新融入每个部门（第一追随者原则）
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "如果你只将创新局限为某个团队的特权，那么你或许能为这个团队吸引到创新人才，却无法吸引足够的'第一追随者'。"
  summary: |
    "将孤独的疯子变成领袖的是第一个追随者"：创新必须感染每个部门，否则追随者无处可去。
  tags: [principle, innovation, organization]

- id: p181
  title: 雇用乐观的人
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "你所雇用的人，不仅要有能够产生新构想的头脑，也要足够疯狂地相信这些构想有机会实现。
    你需要挖掘和吸引这些乐观的人才。"
  summary: |
    乐观是创新的必要条件：招人时除了看构想能力，还要看其是否敢于押注构想能成真。
  tags: [principle, talent, optimism]

- id: p182
  title: 用户与客户冲突时，以用户为先
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（聚焦用户）
  source_quote: |
    "我们的用户就是使用我们产品的人，而我们的客户则是花钱投放广告以及购买我们技术使用权的公司。……
    如果出现矛盾，我们还是会以用户利益为重。这是所有行业都必须遵从的做法。"
  summary: |
    分清"用户"与"客户"（如运营商才是摩托罗拉口中的客户）：两者冲突时，永远站用户一边。
  tags: [principle, user-first, strategy]

- id: p183
  title: 未做详细财务分析也可发布
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（聚焦用户）
  source_quote: |
    "这项功能无疑会为用户带来便利，我们心知肚明，发布才是最佳的商业决策。"
  summary: |
    若功能对用户有明显好处，不要等财务模型齐备才放行；财务论证是事后补充，不是发布闸门。
  tags: [principle, product, decision]

- id: p184
  title: 往大处想：把想法放大 10 倍
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "'你想得不够大'这句话后来被拉里·佩奇的'把想法放大10倍'取而代之，这两句话可以帮助人们从老旧思想中跳脱。"
  summary: |
    产品评鉴的标准问句："你想得不够大／把想法放大10倍"；10 倍目标逼你从头设计，而非修补现状。
  tags: [principle, innovation, ambition]

- id: p185
  title: 赌注下得越大，成功的概率越大
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "赌注下得越大，成功的概率往往也越大，因为企业无法负担失败的损失。……如果你下了一连串较小的赌注，
    没有一个能威胁到企业的安危，那么你便有可能以平庸告终。"
  summary: |
    反直觉的资源律：小赌注输得起就不会拼命，结果是一连串平庸；大赌注让全组织不成功便成仁。
  tags: [principle, innovation, risk]

- id: p186
  title: 巨大的挑战吸引顶尖人才
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "较大的问题通常也较容易解决，因为挑战越大，越能吸引顶尖人才。……巨大的挑战往往是吸引以及留住创意精英的强大磁场。"
  summary: |
    招聘与留人的隐藏杠杆：把大难题交给对的人是播撒快乐，难题本身就是最好的人才磁铁。
  tags: [principle, talent, challenge]

- id: p187
  title: OKR 要（近乎）遥不可及
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（制定（近乎）遥不可及的目标）
  source_quote: |
    "合理的OKR应当有一定难度，达到其中所有的要求应是不可及的。如果你的OKR全是绿色的，说明你所设的目标不够高。
    ……一个完善的OKR虽然只能完成70%，要好过设置存在漏洞但完成100%的OKR。"
  summary: |
    设目标的反常识规则：全绿=定低了；好 OKR 完成七成胜过宽松 OKR 完成十成，关键成果必须可量化。
  tags: [principle, okr, goal-setting]

- id: p188
  title: OKR 打分不作他用，日常工作不入 OKR
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "OKR需要打分，但这分数不作他用，甚至没有人来记录。唯一的用途，就是让员工诚实地评判自己的表现。"
  summary: |
    OKR 的两条纪律：打分只用于自我诚实评估、不挂钩薪酬考核；OKR 只装需要额外努力的目标，日常例行工作除外。
  tags: [principle, okr, measurement]

- id: p189
  title: 70/20/10 资源配置原则
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "将70/20/10作为我们的资源配置原则，即将70%的资源配置给核心业务，20%分配给新兴产品，
    剩下的10%投在全新产品上。"
  summary: |
    资源分配的固定比例：70% 核心业务、20% 新兴产品、10% 疯狂构想；用制度框架给"说好"文化兜底。
  tags: [principle, resource-allocation, innovation]

- id: p190
  title: 投入过多与不足同样有害
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "投入过多与投入不足同样不可取。……过度投资会让人产生固执的偏见，这时，大家只能看见那些投入大量资源的项目中
    积极的一面。"
  summary: |
    资源投入的甜点位：投太少压死创意，投太多滋生沉没成本偏见（如苹果牛顿）；对新构想保持克制。
  tags: [principle, resource-allocation, bias]

- id: p191
  title: 创意喜欢限制
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "'创意喜欢限制'……资源上的稀缺，是激发创意的催化剂。"
  summary: |
    给创意设边界而非给预算：适度的强制条件（拉里用相机和节拍器起家谷歌图书）比充裕经费更能催生突破。
  tags: [principle, innovation, constraint]

- id: p192
  title: 20% 时间制的重点在自由，不在时间
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "该制度的重点在于自由，而不在时间长短。……这个制度对那些看管严格的管理者起到了制约平衡的作用，
    让人们得以把时间花在工作不允许的地方。"
  summary: |
    制度化自主权：允许工程师把 20% 时间用于自选项目，可攒可散、不计考核；自由感而非工时是核心。
  tags: [principle, innovation, autonomy]

- id: p193
  title: 先造原型，再拉伙伴
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "我们总是会提醒那些想要用20%时间做项目的人先造出产品原型，因为原型可以调动众人的兴趣。"
  summary: |
    构想的推进器是原型而非说服：先做出可见的模型，用原型吸引同事投入他们的 20% 时间。
  tags: [principle, innovation, prototype]

- id: p194
  title: 演示日：禁止孤军奋战
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "一支团队用一周的时间为新的构想建立原型，并且在周末之前向大家做原型展示。……除自己之外，
    工程师至少还需要挑选一个人加入项目，孤军奋战是不允许的。"
  summary: |
    集中建原型的组织机制：一周冲刺＋周末公开展示＋强制至少两人成组＋鼓励跨团队协作。
  tags: [principle, innovation, mechanism]

- id: p195
  title: 创意无处不在：警惕"创意只出自员工"的谬论
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（创意无处不在）
  source_quote: |
    "最大的危险不在于误认为只有管理者才有好创意，认为创意只能出自公司的员工才是最危险的谬论。
    创意无处不在，创意有可能来自公司内部，也同样有可能来自公司之外。"
  summary: |
    创意来源的边界是全世界：用户翻译、草根制图、外部开发者都是创意供给者；把边界外的人当成编外员工。
  tags: [principle, innovation, openness]

- id: p196
  title: 交付，迭代
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "打造一款产品，投放市场，看看反响如何，设计并加以改进，再重新投入市场。这就是交付和迭代，
    在此方面最为眼疾手快的公司，才能成为赢家。"
  summary: |
    发布不是终点而是起点：尽快交付、用真实反馈驱动改进；完美是优秀的敌人，能交付才是真正的艺术家。
  tags: [principle, product, iteration]

- id: p197
  title: 别靠营销吹捧上市
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（交付，迭代）
  source_quote: |
    "具体实行交付——迭代模式的时候，尽量不要在产品上市时借助市场营销手段和公关宣传的力量。……
    我们只有在产品展现出胜者锋芒之后才会投入资源。"
  summary: |
    低调试营业式发布：让产品靠自己积累升力，展现胜者锋芒后再砸营销，避免"被吹捧上天却名不符实"。
  tags: [principle, product, launch]

- id: p198
  title: 别把糟糕的产品推向市场
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（交付，迭代）
  source_quote: |
    "不要把糟糕的产品投放市场，指望着靠品牌力量在早期吸引人气。产品应当具有卓越的性能，
    但刚上市时，功能有限是可以接受的。"
  summary: |
    交付迭代的边界条件：性能必须卓越、功能可以有限；可在上市后追加"眼前一亮"的功能，但底子不能烂。
  tags: [principle, product, quality]

- id: p199
  title: 以数据锄弱扶强，不计沉没成本
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（交付，迭代）
  source_quote: |
    "领导者必须不计之前的投入，确保锄弱扶强。发展壮大的产品应该获得更多资源，停滞不前的产品则相反。"
  summary: |
    迭代期的资源铁律：按产品势头分配资源，涨者加码、滞者减码；别为挽回投入给弱品输血（Excite 反例）。
  tags: [principle, resource-allocation, data]

- id: p200
  title: 用数据抵制沉没成本谬误
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（交付，迭代）
  source_quote: |
    "多数人都会计算已经投入项目的资源，以此作为一个继续投资的原因。这，就是沉没成本谬误。……
    而以数据为据，则可抵制此谬误的诱惑。"
  summary: |
    "已经砸了几百万"不是继续投入的理由；预先设立数据系统，用使用数据而非投入量决定去留。
  tags: [principle, decision, sunk-cost]

- id: p201
  title: 败得漂亮：修改创意而不否决创意
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（败得漂亮）
  source_quote: |
    "修改创意，而不要否决创意：世界上多数伟大发明的最终用途与最初设想都是天差地别。……失败中往往会隐藏着珍宝。"
  summary: |
    项目失败后的标准动作：解剖其组成部分寻找可移植的技术与用途（Wave→Gmail/G+），而非整包丢弃。
  tags: [principle, failure, learning]

- id: p202
  title: 不要拿失败的团队问罪
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（败得漂亮）
  source_quote: |
    "不要拿失败的团队问罪，而要确保他们能在公司里找到合适的岗位。因为下一批创新者正在静观其变，
    想看看失败的团队会不会受到惩罚。"
  summary: |
    失败团队的处置决定下一次创新意愿：妥善安置成员（如 Wave 团队反获重用），让失败成为荣誉而非污点。
  tags: [principle, failure, culture]

- id: p203
  title: 管理者的任务是打造反脆弱的环境
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（败得漂亮）
  source_quote: |
    "管理者的任务不是规避风险或防止失败，而是打造一个不会因风险和无可避免的失误而垮台的环境。"
  summary: |
    把失败从"要防止的事故"重新定义为"环境要承受的常态"：目标是组织越挫越强的反脆弱性。
  tags: [principle, failure, resilience]

- id: p204
  title: 失败要快：速战速决喊停
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（败得漂亮）
  source_quote: |
    "败得漂亮就要速战速决。一旦发现项目没有什么前途，就应该以最快的速度喊停，以免浪费更多资源，产生更多机会成本。"
  summary: |
    失败的时机规则之一：确认无前景后以最快速度止血，把人才与资源转投有望成功的项目。
  tags: [principle, failure, timing]

- id: p205
  title: 愿景固执，细节灵活，给好点子长时间
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（败得漂亮）
  source_quote: |
    "创新公司的一个特征，就是会为好点子留出充足的时间来酝酿。……我们在愿景上固执己见，在细节上灵活变通。"
  summary: |
    与"失败要快"并存的另一面：真正的战略赌注给 5-7 年期限；期限拉长，很多"疯狂"就变得可行。
  tags: [principle, innovation, patience]

- id: p206
  title: 设检验标准，需要"一连串奇迹"就停
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（败得漂亮）
  source_quote: |
    "你需要快速地迭代，建立检验标准，看看每次迭代有没有把你一步步推向成功。……当你需要'一连串的奇迹'才能成功时，
    那你就该考虑就此打住了。"
  summary: |
    失败时机的判据：每次迭代是否有向成功推进的可验证进展；若成功依赖奇迹连环发生，立即止损。
  tags: [principle, failure, iteration]

- id: p207
  title: 与钱无关：不用金钱鼓动 20% 项目
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌（与钱无关）
  source_quote: |
    "来自外部的奖励非但不能激发创意，反倒会将一件原本能给人带来满足感的事情变成赚钱的差事，从而阻滞灵感。"
  summary: |
    20% 项目不发奖金：外部金钱奖励会把内在动机变成功利交易，工作本身的意义就是报酬。
  tags: [principle, innovation, motivation]

- id: p208
  title: 把难题提出来
  type: principle
  source_chapter: 结语 想象无止境
  source_quote: |
    "有时，只需提出最困难的问题，你就能避免来自企业的反对力量对创新和改变产生负面干扰。……
    我们才需要提出这些难题，为的就是要让大家不安。"
  summary: |
    面对无人敢碰的难题，先把它公开问出来：难题能扭转大企业规避风险的风气，自造的不安好过对手给的不安。
  tags: [principle, organization, candor]

- id: p209
  title: 问"可能会怎样"，别问"一定会怎样"
  type: principle
  source_chapter: 结语 想象无止境
  source_quote: |
    "我们要提出的问题不是未来'一定会怎样'，而是未来'可能会怎样'。'一定会怎样'的问题要求你对未来做出预测，
    这在瞬息万变的世界中无异于自欺欺人。"
  summary: |
    面向未来的正确提问方式：不要求精确预测，而是展开想象问"依照传统思维不可想、如今已成为可能"的是什么。
  tags: [principle, future, questioning]

- id: p210
  title: CEO 既要核心业务也要放眼未来
  type: principle
  source_chapter: 结语 想象无止境
  source_quote: |
    "首席执行官不仅要考虑企业的核心业务，还要放眼未来；多数企业失败就在于安于现状，只做渐进改变。"
  summary: |
    把"着眼未来"写进 CEO 的岗位职责：渐进改变在科技剧变时代是致命的，领导者必须双线操作。
  tags: [principle, leadership, future]

- id: p211
  title: 既有企业要么借平台再造，要么被淘汰
  type: principle
  source_chapter: 结语 想象无止境
  source_quote: |
    "既有企业必须做出选择。它们可以继续延续老路……这种做法意在维持现状，因此不仅会限制消费者的选择，
    还会遏制行业创新的脚步。……也可以选择另一条路：找到一种策略，利用平台优势持续打造优秀的产品。"
  summary: |
    只有两个选项且没有中间态：把科技仅当效率工具维持现状者终被淘汰；活路是借平台再造并吸引创意精英。
  tags: [principle, assertion, platform]

- id: p212
  title: 五年后自检问题清单（清单）
  type: principle
  source_chapter: 结语 想象无止境（把难题提出来）
  source_quote: |
    "表现突出且资金充足的竞争企业会以什么样的方式危及你的核心业务？……你们的决策过程能产生最佳决策，
    还是最让人接受的决策？你的员工拥有多少自由？"
  summary: |
    组织年度自检清单：竞争者如何借数字平台偷袭？是否常为利润扼杀创新？高管自己用产品吗？最优秀的人三年后还留吗？
    招聘是否高管的头等要务？决策产生最佳还是最可接受的方案？信息路由器还是囤积者更吃香？
  tags: [checklist, self-assessment, future]

- id: p213
  title: 几乎所有大问题都是信息问题
  type: principle
  source_chapter: 结语 想象无止境
  source_quote: |
    "几乎所有大的难题都可以归结为信息问题，也就是说，只要有足够的数据、具备足够的数据处理能力，
    人类所面临的几乎所有问题都有解决方法。"
  summary: |
    作者的底层乐观断言：把大难题翻译成信息问题（数据+计算力），就能看到解决路径；这是全书的信念地基。
  tags: [assertion, technology, optimism]

- id: p214
  title: 赋能而非管理或激励
  type: principle
  source_chapter: 推荐序 赋能：创意时代的组织原则（曾鸣）
  source_quote: |
    "未来组织最重要的功能已经越来越清楚，那就是赋能，而不再是管理或激励。"
  summary: |
    创意革命时代，组织的核心职能从管理、激励转向赋能：提供让人更高效创造的环境与工具，激起创意人的兴趣与动力；
    命令、分派与监工不适用于自激励的创意精英。
  tags: [principle, organization, empowerment]

- id: p215
  title: 是员工使用组织的公共服务，而不是公司雇用了员工
  type: principle
  source_chapter: 推荐序 赋能：创意时代的组织原则（曾鸣）
  source_quote: |
    "我们甚至可以说，是员工使用了组织的公共服务，而不是公司雇用了员工。两者的根本关系发生了颠倒。"
  summary: |
    组织与创意精英的关系要颠倒过来：人是带着志趣来使用平台的主角，组织是公共服务方；
    这要求更高的员工自主性、更高的流动性和更灵活的组织。
  tags: [principle, organization, mindset]

- id: p216
  title: 从基本原则出发思考，勿以"不可能"否定构想
  type: principle
  source_chapter: 序言 谷歌的"痴心妄想"（拉里·佩奇）
  source_quote: |
    "他们习惯用'不可能'来否定自己的想法，而不是从基本物理原则出发去探索可能性。"
  summary: |
    评估构想时回到基本原理推演可行性，而不是凭直觉用"不可能"提前杀死它；
    多数人缺的不是想象力，而是质疑"不可能"的习惯。
  tags: [principle, mindset, innovation]

- id: p217
  title: 摒弃指挥—控制式管理
  type: principle
  source_chapter: 前言 谷歌是如何运营的
  source_quote: |
    "这种方法旨在放慢速度，也的确有效地减缓了速度。也就是说，当企业必须一直加速时，这种结构就会失灵，阻碍企业发展。"
  summary: |
    "信息自下而上流动、决策自上而下传达"的结构诞生于失误成本高、信息垄断于高层的时代，本质是减速器；
    必须持续提速的现代组织必须弃用它。
  tags: [principle, management, structure]

- id: p218
  title: 组合现有科技解决行业重大问题
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的
  source_quote: |
    "寻找技术洞见的途径之一，就是将这些可用的科技及数据资料集中起来，为某个行业中存在的问题寻找新的解决方法。"
  summary: |
    组合创新时代的找洞见之法：信息、连接、计算能力皆已廉价可得，把现成科技、数据与本行业专长重新组合，
    去攻击行业里的具体难题。
  tags: [rule, strategy, technical-insight]

- id: p219
  title: 大型企业成功三步
  type: principle
  source_chapter: 第二章 战略：你的计划是错误的（埃里克的战略会议笔记）
  source_quote: |
    "1.使用创新的方式解决问题。2.利用这个解决方式快速成长与扩张。3.成功很大程度上是以产品为基础的。"
  summary: |
    大型企业共同起点的三步公式，也是战略完整性的自检清单：有创新解法、能借解法快速扩张、以产品为根基。
  tags: [checklist, strategy, growth]

- id: p220
  title: 以舞蹈团为中心，不要打造明星体系
  type: principle
  source_chapter: 第一章 文化：相信自己的口号
  source_quote: |
    "最好的管理体系都是以某个群体为中心而建立的，这个群体并不是一组超级明星，而更像一个舞蹈团。"
  summary: |
    组织的中心应是配合默契的出众群体而非个别超级明星，以此建立长期稳定的人才板凳，
    让机遇来临时有大批板凳队员能顶上领袖位置。
  tags: [principle, organization, team]

- id: p221
  title: 设立面试官委员会
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "在谷歌，我们执行一种名叫'面试官委员会'的模式……得不到主持面试的机会本身就是一种惩罚。"
  summary: |
    把面试从人人逃避的杂活变成少数人享有的特权：须接受培训并陪面至少4次才有主持资格；
    以面试次数、可信度、反馈质量与速度接受指标考核，公布评分、允许挑战者取代在任者。
  tags: [rule, interview, organization]

- id: p222
  title: 面试结束后立刻明确反馈
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "我们告诉面试官，一旦结束对应聘者的面试，就应该立刻将是否录用的决定明明白白地告知用人部门的经理。"
  summary: |
    拖到周五下午写反馈时细节早已模糊；顶尖面试官面试后专门腾出时间立即反馈（48小时后质量大打折扣），
    配套的信息包设计要让决策者在120秒内读完。
  tags: [rule, interview, speed]

- id: p223
  title: 淘汰可被提前准备的智力谜题
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "我们的许多智力谜题（以及答案）都出现在了网上……这些谜题已逐渐失却了检验应聘者能力的功能。"
  summary: |
    面试题若能被搜索和排练，测出的只是演技而非能力；要及时识别并把这类题目从面试中剔除。
  tags: [rule, interview]

- id: p224
  title: 想一手遮天的管理者不用也罢
  type: principle
  source_chapter: 第三章 人才：招聘是你最重要的工作
  source_quote: |
    "如果有人想在自己的团队中一手遮天，那么这样的人不用也罢。"
  summary: |
    因招聘委员会的制约而扬言离职的管理者，在其他方面往往也会飞扬跋扈；
    宁可失去这个人，也不为个别人破坏机制。
  tags: [rule, management, hiring]

- id: p225
  title: OKR全员公开，高管带头
  type: principle
  source_chapter: 第五章 沟通：当最牛的路由器
  source_quote: |
    "每个季度，每位员工都需要更新自己的OKR，并在公司内发布……这个制度的施行需要从高层做起。"
  summary: |
    OKR人人可用、撇开职位差异，发布在公司内网上供任何人查阅（含CEO）；
    高管公开为上一季度的失误打分剖析，让飞速扩张中的各团队始终保持对齐。
  tags: [rule, okr, transparency]

- id: p226
  title: 用OKR让员工不被竞争者分心
  type: principle
  source_chapter: 第六章 创新：缔造原始的混沌
  source_quote: |
    "而如果员工将注意力放在精心设置的OKR上，这个问题就会迎刃而解。因为这样一来，员工就会看到自己该走的路，也无暇担心竞争了。"
  summary: |
    对抗"追赶竞争者陷入平庸"的操作手段：把注意力锁进自设的远大目标，
    竞争者便失去占用团队心智带宽的能力。
  tags: [rule, okr, competition]

- id: p227
  title: 监管应为新企业和破坏性创新留出空间
  type: principle
  source_chapter: 结语 想象无止境
  source_quote: |
    "监管环境必须留出空间，新企业才能进入。……如果实际数据表明新的方法要优于老旧的方法，那么政府就不应阻碍变化，而是给破坏性创新开绿灯。"
  summary: |
    对一切都做规定的体制没有创新余地；法规应以实际数据为准绳，新方法被证明更优时不设置高于旧方法的门槛，
    勿重演英国《红旗法案》。
  tags: [principle, policy, innovation]
```
