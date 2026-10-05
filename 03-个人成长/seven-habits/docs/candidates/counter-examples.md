# candidates/counter-examples.md — 反例提取器候选清单

> 提取器：counter-example-extractor（失败模式 / 反例 / 陷阱 / 认知偏误）。串行降级执行。每条含 failure_mode / mechanism / warning_signs / bound_to。

- id: ce01
  title: 个人魅力论的"阿司匹林与创可贴"
  type: counter-example
  source_chapter: 第一章·品德与个人魅力孰重；症结在于治标不治本
  source_quote: |
    "用'阿司匹林'和'创可贴'来治疗心灵痛苦的方法，往往是头痛医头，脚痛医脚，治标而不治本。
     有时似乎取得了暂时的效果，但是深层次的问题没有解决。"
  failure_mode: |
    用技巧、形象、话术去解决品德与思维方式层面的问题；短期见效，长期复发且加深。
  mechanism: |
    行为与态度是"枝叶"，思维方式是"根基"——不换地图，越努力越快到达错误地点；
    信任由品德产生，技巧在品德缺失时会被识破为操纵。
  warning_signs:
    - 追问"有没有快速见效的诀窍"
    - 问题解决后不久反复重现
    - 依赖培训、话术、激励演讲
  bound_to:
    - "思维转换（f20）"
    - "品德第一感情第二理性第三（f19）"
  tags: [counter-example, quick-fix]

- id: ce02
  title: 三种决定论地图（基因/心理/环境）
  type: counter-example
  source_chapter: 第三章（习惯一）·社会之镜
  source_quote: |
    "基因决定论……心理决定论……环境决定论……这三种地图都以'刺激—回应'理论为基础。"
  failure_mode: |
    把自己的现状归因于祖先、父母或环境，从而放弃选择回应的自由。
  mechanism: |
    三种决定论共享"刺激—回应"的动物模型；"社会之镜"（他人评语）是投影而非影像，
    以它自我认知等于从哈哈镜看自己。
  warning_signs:
    - "我天生如此/都怪我父母/这环境就这样"
    - 等待外部条件改变才行动
  bound_to:
    - "刺激与回应之间的距离（f02）"
  tags: [counter-example, determinism, victimhood]

- id: ce03
  title: 消极语言与"要是…就好了"句式
  type: counter-example
  source_chapter: 第三章（习惯一）·聆听自己的语言；"如果"和"我可以"
  source_quote: |
    "'我就是这样做事的。''他把我气疯了！''我根本没时间做。''要是我妻子能更耐心一点就好了。''我只能这样做。'"
  failure_mode: |
    用决定论语言把责任外包给天性、他人、时间与环境；说者被自己的话洗脑，宿命感加深。
  mechanism: |
    语言是思维方式的可观察输出，同时反过来强化思维——推卸责任的话语强化推卸责任的回路。
  warning_signs:
    - 口头禅含"但愿/我办不到/我不得不/要是"
    - 描述困境时主语总是别人或环境
  bound_to:
    - "替换消极语言（p02）"
    - "影响圈（f01）"
  tags: [counter-example, language]

- id: ce04
  title: 重蛋轻鹅的透支行为
  type: counter-example
  source_chapter: 第二章·三类资产；团体的产能
  source_quote: |
    "从没有保养的割草机，到掺水浓汤餐厅……此时老板使尽浑身解数，妄图收复失地，只可惜他已经失去了宝贵的资产——顾客的信任。"
  failure_mode: |
    为当期产出摧毁产能：不保养机器、动用本金、压榨员工、掺水降本、操控配偶与子女。
  mechanism: |
    产出可直接计量，产能的损耗是隐性的、滞后的（账簿只列产量成本利润）；
    透支由"第三季度才坏"的延迟反馈掩护，直到资产死亡。
  warning_signs:
    - 只考核产出指标
    - "先冲一下业绩再说"
    - 人员流失率上升、信任度下降
  bound_to:
    - "产出/产能平衡（f05）"
  tags: [counter-example, short-termism]

- id: ce05
  title: 用唠叨、威胁、吼叫换取"整洁的房间"
  type: counter-example
  source_chapter: 第二章·三类资产
  source_quote: |
    "如果你只关注房间整洁这个产出，总是用唠叨、威胁、吼叫等方法得到金蛋，那就等于牺牲了鹅的健康与幸福。"
  failure_mode: |
    亲子与婚姻中只想要行为结果（金蛋），用地位差强推，摧毁孩子的责任感与关系本身（鹅）。
  mechanism: |
    孩子是"能产金蛋的资产鹅"：恐惧与贿赂能拿到单次行为，却以自律能力和信任为代价；
    结果是"惧怕取代合作，双方更加坚持己见"。
  warning_signs:
    - 不盯就不做
    - 靠奖惩驱动
    - 孩子在青春期后拒绝交流
  bound_to:
    - "P/PC（f05）"
    - "责任型授权（f18）"
  tags: [counter-example, parenting]

- id: ce06
  title: 第三代时间管理的过刚与陷阱
  type: counter-example
  source_chapter: 第五章（习惯三）·四代时间管理理论；集大成
  source_quote: |
    "过分强调效率，把时间崩得死死的，反而会产生反效果，使人失去增进感情、满足个人需要以及享受意外惊喜的机会。"
  failure_mode: |
    逐日排程、以效率为纲：日程密不透风→被打断即崩溃→转向第四象限逃避；人被计划奴役。
  mechanism: |
    第三代只有优先序工具、没有使命锚点，故"对事情仍没有轻重缓急之分"的深层问题未解；
    且违反"人比事重要"，牺牲人际关系。
  warning_signs:
    - 计划稍有变动就内疚或弃守
    - 效率越高家庭关系越差
  bound_to:
    - "第四代时间管理（f07）"
  tags: [counter-example, time]

- id: ce07
  title: 梯子搭错墙的忙碌
  type: counter-example
  source_chapter: 第四章（习惯二）·"以终为始"的定义
  source_quote: |
    "许多人拼命埋头苦干，到头来却发现追求成功的梯子搭错了墙，但是为时已晚……如果通往成功的梯子一直搭错墙，
     那每一次行动无疑加快了失败的步伐。"
  failure_mode: |
    高效执行错误方向：爬得越快，离真正的目标越远；成功后空虚。
  mechanism: |
    忙碌与成果给人"在正轨"的错觉；没有第一次创造，效率只是加速错误（泰坦尼克沉没前拉开躺椅）。
  warning_signs:
    - 极忙但说不出"做正确的事"是什么
    - 达成目标后感到空虚
  bound_to:
    - "领导先于管理（f04）"
    - "以人生终点为衡量（p06）"
  tags: [counter-example, misdirection]

- id: ce08
  title: 情感账户透支后讲技巧
  type: counter-example
  source_chapter: 第六章·情感账户；第八章（习惯五）
  source_quote: |
    "只有对方认同，你的投资才有意义，否则就算你费尽心机，对方也只会把它看作是一种控制、自利、胁迫和屈就，结果是情感账户被支取。"
  failure_mode: |
    在信任余额为零的关系里使用沟通技巧、送礼、说教——一切动作被解读为操纵。
  mechanism: |
    意义由接收方按账户余额定价；透支状态下同一段话从"关心"变"控制"；
    青春期子女对只会纠错的父母关闭沟通通道即为典型。
  warning_signs:
    - 对方回"你到底想干什么"
    - 恶意服从（按指示行事但绝不多做）
  bound_to:
    - "情感账户（f08）"
    - "知彼解己（p13）"
  tags: [counter-example, trust]

- id: ce09
  title: 背后攻击他人换"同盟"
  type: counter-example
  source_chapter: 第六章·正直诚信
  source_quote: |
    "假如我为了取得你的信任，就以其他人的隐私讨好你……我想你多半会在心里盘算：这家伙大概也会把我说过的什么话这样告诉别人吧。"
  failure_mode: |
    用议论不在场的人来拉近与在场者的关系，实际上向所有人证明自己两面三刀。
  mechanism: |
    听者会推理"他今天对我说别人，明天就对别人说我"；短期得金蛋，杀死友谊的鹅。
  warning_signs:
    - 对话以"跟你说个秘密"开场
    - 团队中人前和谐、人后互撕
  bound_to:
    - "维护不在场的人（p17）"
  tags: [counter-example, integrity]

- id: ce10
  title: 有条件的爱激起反叛
  type: counter-example
  source_chapter: 第六章·无条件的爱
  source_quote: |
    "可是孩子却反驳，他不愿为父亲读书。在父亲心目中，进入名校比儿子更重要，这种爱是有条件的。为了维护自主权，儿子必须反抗这种安排。"
  failure_mode: |
    把爱与接纳挂钩于表现（成绩、名校、顺从），孩子以"为反对而反对"维护自主权。
  mechanism: |
    有条件的爱反映爱人者自身不成熟（价值受制于对方表现）；被爱者的反抗是对独立权的捍卫。
  warning_signs:
    - "你这样对得起我们的付出吗"
    - 孩子以自毁式选择对抗安排
  bound_to:
    - "无条件的爱（f08 第七种投资）"
  tags: [counter-example, parenting]

- id: ce11
  title: 赢/输模式的四大浸染源
  type: counter-example
  source_chapter: 第七章（习惯四）·损人利己（赢/输）
  source_quote: |
    "在家里，大人总是喜欢将孩子进行比较……学校是赢/输模式的另一个温床，'正态分布曲线'主要说明的是：
     你之所以得A，是因为有人得了C。"
  failure_mode: |
    家庭比较、学校排名、运动零和叙事、法律对抗不断训练"我赢=你输"的默认反应，带入婚姻与职场。
  mechanism: |
    爱被附加条件后，自我价值只能通过比较实现；内在价值让位于外在排名。
  warning_signs:
    - 把配偶同事当竞争对手
    - 见不得别人好（匮乏心态）
  bound_to:
    - "人际交往六模式（f13）"
    - "富足心态（f12）"
  tags: [counter-example, competition]

- id: ce12
  title: 输/赢"老好人"的压抑与爆发
  type: counter-example
  source_chapter: 第七章（习惯四）·舍己为人（输/赢）
  source_quote: |
    "被压抑的情感并不会消失，累积到一定程度后，反而以更丑恶的方式爆发出来，有些精神疾病就是这样造成的。"
  failure_mode: |
    无标准、无要求、以取悦换认同；压抑愤怒最终以更具破坏性的方式爆发，自我评价日益低落。
  mechanism: |
    输/赢是赢/输的生存土壤（前者的弱点是后者的力量来源）；主管与家长在两模式间摆荡——纪律松时强硬，内疚后纵容，再愤怒再强硬。
  warning_signs:
    - 嘴上说"都行、听你的"
    - 报复性消费/突然翻脸/消极怠工
  bound_to:
    - "人际交往六模式（f13）"
    - "成熟=敢作敢为与善解人意平衡（f12）"
  tags: [counter-example, conflict-avoidance]

- id: ce13
  title: 输/输式报复
  type: counter-example
  source_chapter: 第七章（习惯四）·两败俱伤（输/输）
  source_quote: |
    "他把一辆价值一万美元的汽车以五十美元出售，然后分给妻子二十五美元。……为了报复，不惜牺牲自身的利益。"
  failure_mode: |
    双方都固执己见、都想扳回局面：报复是双刃剑，"谋杀等于自杀"。
  mechanism: |
    由赢/输相遇演化而来——两个损人利己者互不相让，宁可自损也要让对方输。
  warning_signs:
    - "我不好过也不让你好过"
    - 争端已无关利益本身
  bound_to:
    - "人际交往六模式（f13）"
  tags: [counter-example, revenge]

- id: ce14
  title: 嘴上双赢、机制奖励竞争（百慕大之旅）
  type: counter-example
  source_chapter: 第七章（习惯四）章首
  source_quote: |
    "每星期他都会召集全体经理，一边训示合作的重要性，一边却以百慕大之旅作饵。换句话说，总裁口头上高唱互助合作，实际上鼓励彼此竞争。"
  failure_mode: |
    用竞争机制追求合作结果：制度奖励唯一赢家，口头要求团队协作，员工理性选择内斗。
  mechanism: |
    体系层的赢/输抵消品德层的双赢（跳层失败）——"想用竞争模式实现合作，却发现这并不奏效"。
  warning_signs:
    - 激励只表彰个人/部门冠军
    - 部门墙、藏技能、抢资源
  bound_to:
    - "双赢思维五要领（f12）"
  tags: [counter-example, incentive]

- id: ce15
  title: 四种自传式回应毁掉亲子沟通
  type: counter-example
  source_chapter: 第八章（习惯五）·四种自传式回应；父子对话
  source_quote: |
    "价值判断令人不能畅所欲言，追根究底则令人无法开诚布公，这些都是经常影响亲子关系的一大障碍。"
  failure_mode: |
    倾听时插入价值判断、追根究底、好为人师、自以为是——孩子从"想谈谈心事"退到"多说也没什么用"。
  mechanism: |
    以自己的经验与动机衡量对方，把谈话变成审判；回应式倾听本质以自我为中心，让对方有受辱感。
  warning_signs:
    - "当年我……"开场
    - "你应该……"高频出现
    - 孩子说"算了，跟你说了也没用"
  bound_to:
    - "先诊断后开方（f14）"
  tags: [counter-example, listening]

- id: ce16
  title: 不诊断就开药方
  type: counter-example
  source_chapter: 第八章（习惯五）·先诊断，后开方
  source_quote: |
    "'戴上吧，'他说，'我已经戴了十年了，很管用，现在送给你。'……一个不诊断就开药方的医生怎么能信任呢？"
  failure_mode: |
    听几句就摘下自己的眼镜递给对方、开处方——用善意建议快刀斩乱麻，跳过对问题症结的理解。
  mechanism: |
    诊断决定处方的可信度："如果你对诊断本身没什么信心，那么也就不会对据此开的药方有信心。"
  warning_signs:
    - 建议比提问多
    - "我懂我懂"挂嘴边
  bound_to:
    - "先诊断后开方（f14）"
  tags: [counter-example, advice]

- id: ce17
  title: 消极协作减效：一脚油门一脚刹车
  type: counter-example
  source_chapter: 第九章（习惯六）·消极协作减效
  source_quote: |
    "人们在解决问题和下决定的时候往往将太多的时间和精力耗费在玩弄权术、唇枪舌剑、彼此提防……这就像是开车的时候一只脚踩油门，另一只脚却踩刹车。"
  failure_mode: |
    嘴上双赢技巧、心里只想操纵——权术、防卫、放马后炮把合作耗在原地。
  mechanism: |
    低信任环境的自我保护回路：提防→法律化→更提防；缺乏安全感者用"克隆"别人（改造他人符合自己模式）来消除差异。
  warning_signs:
    - 会前私下拉票、会后议论
    - 合同越来越厚、信任越来越薄
  bound_to:
    - "统合综效与第三选择（f15）"
  tags: [counter-example, politics]

- id: ce18
  title: 法律手段过早介入
  type: counter-example
  source_chapter: 第九章（习惯六）
  source_quote: |
    "有些时候法律手段是绝对必要的，但是我认为它只应该在最后关头发挥作用，而不是问题刚一出现的时候，
     过早使用只会让恐惧心理和法律模式制约了统合综效的可能性。"
  failure_mode: |
    合伙人靠严密条文自保，把关系交给律师，扼杀真诚合作的可能性。
  mechanism: |
    法律语言把人设定为对抗方，沟通降级到防备层次（1+1=0.5）。
  warning_signs:
    - 谈判桌上律师代言、本人闭口
    - 凡事先留证据
  bound_to:
    - "统合综效（f15）"
  tags: [counter-example, trust]

- id: ce19
  title: 锯树不磨锯
  type: counter-example
  source_chapter: 第十章（习惯七）章首
  source_quote: |
    "'为什么不暂停几分钟，把锯子磨得更锋利？'对方却回答：'我没空，锯树都来不及，哪有时间磨锯子？'"
  failure_mode: |
    以"太忙"为由无限推迟锻炼、学习、反思与关系建设，产能持续下滑，越忙越钝。
  mechanism: |
    更新是第二象限事务，不紧急故永不开始；忽视更新必然滑入第一象限（健康危机、 burnout）。
  warning_signs:
    - "等这阵忙完再说"
    - 已连续多周无任何更新活动
  bound_to:
    - "不断更新四层面（f16）"
  tags: [counter-example, burnout]

- id: ce20
  title: 沉溺电视与停止阅读
  type: counter-example
  source_chapter: 第十章（习惯七）·智力层面
  source_quote: |
    "长期研究表明，大多数家庭的电视机每周要开约35~45个小时……不再认真读书，不再探索身外的新世界，不再用心思考。"
  failure_mode: |
    离开学校后智力层面停止投入，被动消费取代主动学习；电视的价值观潜移默化。
  mechanism: |
    智力更新（阅读/写作/规划）全是第二象限，被娱乐性内容挤出；
    书中数据为 1989 年语境，30 周年版未更新至数字媒体。
  warning_signs:
    - 屏幕时间 > 学习时间且无自觉
    - "毕业后再没读完一本书"
  bound_to:
    - "不断更新四层面（f16）"
  tags: [counter-example, media]

- id: ce21
  title: 社会之镜与贴标签
  type: counter-example
  source_chapter: 第三章（习惯一）·社会之镜；第十章·改变他人
  source_quote: |
    "这些零星的评语不一定代表真正的你，与其说是影像，不如说是投影，反映的是说话者自身的想法或性格弱点。"
  failure_mode: |
    按他人即时评价与旧标签定义自我与子女；被贴标签者按标签行事（皮格马利翁效应反例）。
  mechanism: |
    社会之镜是变形镜；教师的看法经由自我实现预言变成学生的成绩。
  warning_signs:
    - "你就是懒/你不是学数学的料"
    - 用过去表现预测他人未来
  bound_to:
    - "以潜能期许他人（p22）"
    - "自我意识（f02）"
  tags: [counter-example, labeling]

- id: ce22
  title: 由外而内求变
  type: counter-example
  source_chapter: 第一章·新的思想水平
  source_quote: |
    "我见过一些婚姻不和谐的夫妇，两个人都想改造对方，不断列举对方的'罪状'以达到目的。
     我也见过一些劳资纠纷，双方耗费大量时间和精力订立规章制度，仿佛这样就能够找到信任的基础。"
  failure_mode: |
    把问题定位在"那里/那一方"，用改变他人、改制度、换人的方式回避自我改变；僵局固化。
  mechanism: |
    "由外而内"路线把改变的先决条件放在对方与环境上，而对方也在等我们改变——互相等待即互相指责。
  warning_signs:
    - "只要他改了就好了"
    - 制度越订越细、关系越来越差
  bound_to:
    - "由内而外（f20/本书总纲）"
    - "影响圈（f01）"
  tags: [counter-example, blame]

- id: ce23
  title: 有自制力却无使命的"伪面具"
  type: counter-example
  source_chapter: 第五章（习惯三）·勇于说不
  source_quote: |
    "他们能够掌握重点，也有足够的自制力，却不是以原则为生活中心，又缺少个人使命宣言。……他们带着伪面具，外在表现的也许内心并不认同。"
  failure_mode: |
    把要事第一当纪律问题来修（打卡、自律工具），根基仍是摇摆的生活中心，终被诱惑拖回第三四象限。
  mechanism: |
    "只有由至诚的信念与目标出发，才能够产生坚定说不的勇气"——自制力不能替代方向。
  warning_signs:
    - 工具换了一个又一个
    - 拒绝诱惑时屡战屡败
  bound_to:
    - "生活中心（f10）"
    - "使命宣言（f11）"
  tags: [counter-example, discipline]

- id: ce24
  title: 把"双赢"让成"输/赢"
  type: counter-example
  source_chapter: 第七章（习惯四）·哪一种最好；连锁商店总裁对话
  source_quote: |
    "'可你们为什么要选择输/赢模式呢？'……'没有啊，我们是想要双赢的。'……'那这不是输/赢模式是什么？'
     当意识到他所谓的双赢实质上是输/赢模式时，他很震惊。"
  failure_mode: |
    以双赢之名行让步之实：对方得寸进尺，压抑的怨恨最终以两败俱伤收场。
  mechanism: |
    缺乏勇气（只善解人意不敢作敢为）时，双赢滑向输/赢；"平静的关系下面涌动着的是压抑的情感"。
  warning_signs:
    - "为了关系我忍了"
    - 回家对家人发泄职场委屈
  bound_to:
    - "人际交往六模式（f13）"
    - "成熟=勇气与体谅平衡（f12）"
  tags: [counter-example, concession]
