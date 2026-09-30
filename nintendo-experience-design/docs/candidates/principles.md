# 候选提取：原则 / 清单 / 规则 / 断言（principle-extractor）

> 来源：《任天堂的体验设计——创造不知不觉打动人心的体验》（玉树真一郎）
> 提取范围：全书（前言、第1–5章）。未做筛选；框架/案例/反例/术语不在此列。
> 格式：YAML 列表。

```yaml
- id: p01
  title: 任何人都能创造打动人心的体验
  type: principle
  source_chapter: 前言
  source_quote: |
    "如何才能打动人心？如何才能让人理解？如何才能让人行动？……我奉上自己的结论：任何人都能创造打动人心的体验。"
  summary: |
    打动人心的体验不是天才的专利，而是一门可学习、可实践的方法。
    把"用户经历体验的过程"本身当作设计对象，普通人也能做出打动人心的产品、教育与沟通。
  tags: [maxim, assertion, experience-design]

- id: p02
  title: 最重要的规则必须让用户瞬间了解"自己应该做什么"
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "也就是说，最重要的必须是玩家能够瞬间了解'自己应该做什么'。"
  summary: |
    拿掉所有卖点之后，产品要传达的第一条信息是：用户此刻该做什么。
    这条规则不必靠说明书宣布，但必须几秒内被凭直觉接收，否则用户会走投无路。
  tags: [rule, onboarding, affordance]

- id: p03
  title: 人不是因为产品有趣才行动，而是因为自身的直觉体验有趣
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "玩家不是因为游戏有趣才玩，是因为'不由自主就想到了，不由自主就做了'才玩的。"
  summary: |
    行动动机来自用户自己的心理过程（产生假设、想验证），而不是产品本身的品质。
    设计者要停止问"我的东西够不够好"，转问"用户会不会不由自主地产生'要做××吗'的假设"。
  tags: [principle, assertion, motivation]

- id: p04
  title: 无论什么时候都必须考虑用户会有怎样的体验
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "无论什么时候，设计师都必须考虑让玩家有怎样的体验、如何打动玩家。"
  summary: |
    体验设计的第一工作习惯：对每个接触点都先问"这一刻用户的心情是什么、要打动他什么"。
    体验设计就是时时刻刻考虑人的心情。
  tags: [rule, mindset, user-experience]

- id: p05
  title: 用户之前的心路历程决定体验的意义
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "重要的是，在酷栗宝登场之前，玩家是怎样的心情……正是玩家的心路历程决定了体验的意义。"
  summary: |
    同一个事件（遇到敌人）在用户不同心理状态下意义完全不同。
    评价或设计任何体验时，看的不是单个事件本身，而是用户在它发生之前累积了怎样的心情。
  tags: [principle, assertion, experience-design]

- id: p06
  title: 让高兴逐次积累，直到用户自己意识到"有趣"的那一刻
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "情绪持续高涨，超过某一点的时候，玩家会有意识地意识到'这个很有趣'。这一瞬间，正是设计师的目标。"
  summary: |
    "有趣"是用户的主观结论，无法直接给予。设计师能做的是让每次直觉体验都带一点高兴，
    让情绪逐步累积，直到用户自己说出"这很有趣"——那一刻才是设计目标。
  tags: [principle, goal-setting]

- id: p07
  title: 能让人直观理解的东西就很有趣
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "直觉设计，不仅直观地传达信息，还承担着让人觉得有趣这一最重要的功能。能让人直观理解的东西就很有趣。"
  summary: |
    直观的理解本身就会产生乐趣，"易懂"与"有趣"不是取舍关系。
    把东西设计得让人一看就懂，就已经是在制造有趣。
  tags: [maxim, assertion, simplicity]

- id: p08
  title: 从开始到"觉得有趣"之间的时间必须用直觉设计填满
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "快则需要几分钟，慢则需要几十分钟。必须用直觉设计来填补这段时间。"
  summary: |
    用户从上手到意识到"有趣"之间有几分钟到几十分钟的空窗。
    这段不能指望用户靠耐心撑过去，必须用一连串小的直觉体验（假设→尝试→高兴）填满。
  tags: [rule, onboarding, pacing]

- id: p09
  title: 每个直觉设计必须简短（约10秒内给出确认）
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "假设在确认其正确之前，会让玩家感到不安……最多10秒钟就会停止游戏。正因为如此，每个直觉设计都应该尽量在短时间内结束。"
  summary: |
    假设未确认前用户一直处于不安中，超过约10秒不安就会压垮体验。
    所以每个"假设→尝试→高兴"单元必须做短，尽快让用户得到确认。
  tags: [rule, pacing, time-limit]

- id: p10
  title: 每个直觉设计都要提高"高兴体验"的发生概率
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "第三个要点，在每个直觉设计中，提高玩家获得愉悦体验的概率。"
  summary: |
    直觉体验不能赌运气。要保证用户在每次小小的"假设—尝试"中大概率得到"猜对了"的高兴，
    失败率过高的单元要重新设计。
  tags: [rule, success-rate]

- id: p11
  title: 让体验简单、容易是绝对条件
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "如果眼前的问题足够简单和容易，那么人们就会解决它。相反，当眼前的问题复杂和困难时，人们则不会试图解决它。"
  summary: |
    行动与否取决于门槛高低：足够简单容易，人就会不由自主去做；复杂困难，人连试都不试。
    想让人产生假设并尝试，必须把体验本身降到几乎不需要努力的程度。
  tags: [principle, simplicity]

- id: p12
  title: 复杂难懂的东西谁都能做，制作简单容易的东西才是真正的难点
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "复杂难懂的东西，其实谁都能做出来。制作简单、容易的东西，才是真正的难点。"
  summary: |
    把复杂留给用户是偷懒，把简单留给用户才是功夫。
    不要用"功能丰富、深度复杂"来证明价值——做简单容易的东西需要多得多的设计投入。
  tags: [maxim, simplicity]

- id: p13
  title: 为传达示能，必须排除一切漂亮、有趣的设计
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "设计师必须排除一切漂亮的设计，放弃让人觉得有趣的事情，集中精力告诉玩家该做什么。这才是对设计师最大的考验。"
  summary: |
    开场阶段"好看""有趣"都会与"让用户知道该做什么"争夺注意力。
    要敢于牺牲漂亮和有趣，把全部信息量集中用于传达"该做什么"这一件事。
  tags: [rule, affordance, trade-off]

- id: p14
  title: 让示能借助用户一看就懂的工具和形态传达
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "为让玩家有正确的假设，并且提高正确尝试的概率，有必要让其明确记起……这一示能。……游戏画面和控制器融为一体，成功传达了示能。"
  summary: |
    想让用户做出正确尝试，就要把"该做什么"寄托在他一见就懂其用途的形态上（十字键、握把、旋钮），
    让画面/界面与操作工具融为一体来传达示能。
  tags: [rule, affordance, design]

- id: p15
  title: 把需要学习的内容集中在体验最初的阶段（初始效应）
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "答案是②，'将4种道具集中在最初的阶段'……在学习心理学中有'初始效应'。在体验开始的时候，人们的注意力和学习效率就会提高。"
  summary: |
    依据初始效应，人在体验开始时注意力和学习效率最高。
    要把必须学习的要素（道具、功能、规则）集中放在最开头教，而不是分散到全程——先集中教完，后面才能安心复杂。
  tags: [rule, onboarding, primacy-effect]

- id: p16
  title: 直觉设计只能建立在"所有用户都知道"的共同记忆上
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "不管什么样的玩家，大家都应该知道'木柴会燃烧'这一点……只要能把握所有玩家的记忆，就能进行体验设计。"
  summary: |
    问题的每个线索都必须取自人人都有的记忆（木柴会燃烧）。
    设计前先确认：这个联想是不是目标人群中所有人都具备？否则体验对一部分人直接失效。
  tags: [rule, common-memory]

- id: p17
  title: 构成问题/谜题的信息绝不能传达错误
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "为明确……等信息，设计师非常小心地设计游戏画面和声音。因为信息是解开谜题的一部分，所以不能传达错误。"
  summary: |
    用户要靠你给出的线索拼出解法，任何一条信息含糊或误导都会让问题无解。
    构成问题的每条信息都要逐一核对，宁可少给，不可给错。
  tags: [rule, information-design]

- id: p18
  title: 故意设置"不合理"的障碍来强制用户学习
  type: principle
  source_chapter: 第2章 · 惊喜设计（《勇者斗恶龙》开场分析）
  source_quote: |
    "明明是国王的房间，却从外面上了锁，这种不合理的设计也是为让玩家直观地了解游戏规则。"
  summary: |
    用户不会主动学习时，可以故意造一个不讲道理的小障碍（国王的房间从外面上锁），
    逼他在解决问题时学会必须掌握的操作。与初始效应配合：把必学内容一口气集中在这个障碍里。
  tags: [rule, teaching, onboarding]

- id: p19
  title: 让用户在解开问题的瞬间感到"我很聪明"
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "玩家在解开谜题的瞬间，可能有一种自己的人生得到肯定的感觉。游戏就是想让你拥有'我很聪明，我很厉害'这样的感觉。"
  summary: |
    体验设计的目标是让用户把成功归功于自己。
    让用户凭自己的记忆和才智解出问题，他获得的不是"产品好用"，而是"我很聪明"的自我肯定。
  tags: [principle, self-efficacy]

- id: p20
  title: 体验设计必须始终以用户的头脑性质和记忆为起点
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "如果你想设计出让人们广泛享受的流行体验，就必须始终以用户为起点进行设计，考虑'用户拥有怎样的大脑和心灵的性质''用户拥有怎样的记忆'。"
  summary: |
    不要从自己的感性和偏好出发。面向大众的设计要回答两个问题：
    所有人共同的大脑/心灵性质是什么？所有人共同的记忆是什么？答案就是设计的原材料。
  tags: [principle, user-first]

- id: p21
  title: "了解"比"好、正确"更重要
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "无论多么经典的游戏，在实际体验之前，用户都不会感到有趣。为让用户感到有趣，最重要的是引导用户'了解'游戏的玩法。总之，'了解'比'好、正确'更重要。"
  summary: |
    用户在亲自体验之前无法感知你的"好"和"正确"。
    第一步永远是让他了解（知道该做什么、怎么用），"好、正确"是了解之后才被感知的东西。
  tags: [principle, prioritization]

- id: p22
  title: 贴近用户＝按"了解→好、正确"的顺序决定优先级
  type: principle
  source_chapter: 第1章 · 直觉设计
  source_quote: |
    "为贴近用户，必须按照用户遵循的'了解'→'好、正确'的体验顺序来决定优先级。……宣扬'好、正确'的设计……这才是设计师面临的最大陷阱。"
  summary: |
    "贴近用户"的可操作定义：按用户经历体验的顺序排序信息——先保证"了解"，再展示"好、正确"。
    反过来先宣扬优点（不考虑用户情况的"好、正确"），就是设计师最大的陷阱。
  tags: [principle, prioritization, pitfall]

- id: p23
  title: 疲劳和厌倦是直觉设计的致命缺点，必须主动应对
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "让人疲劳和厌倦，这正是直觉设计的致命缺点。"
  summary: |
    假设与尝试自带不安，连续的直觉体验必然累积疲劳和厌倦（心理饱和）。
    这不是设计失误而是结构必然，必须用另一种设计（惊喜）来对冲，否则用户终将离开。
  tags: [principle, fatigue]

- id: p24
  title: 在疲劳厌倦达到顶峰的时机插入出乎意料的体验
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "为激活因疲劳和厌倦而变得脆弱的大脑的学习功能，特意穿插一些出乎大脑意料的体验，这是设计长时间体验的重要技巧。"
  summary: |
    长体验的节奏管理核心：找准用户开始疲劳厌倦的节点，在那里放"意料之外"。
    无法预测未来的大脑会重新激活学习动力。
  tags: [rule, pacing, surprise]

- id: p25
  title: 要制造惊讶，必须事先让用户做出（错误的）预测
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "为让玩家出乎意料，事先让玩家做出明确的预测……让玩家做出错误的预测。"
  summary: |
    惊讶不会凭空产生——必须先花时间让用户建立起明确的预测并坚信，之后打破它。
    没有铺垫的"意外"只是混乱。
  tags: [rule, surprise, setup]

- id: p26
  title: 制造惊讶的战略＝有意识地背叛两种"坚信"
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "1. 对前提的坚信→'这个游戏是××' 2. 对日常的坚信→'应该不会出现禁忌'。有意识地背叛这两种坚信，才是设计师应采取的战略。"
  summary: |
    用户只有两类可被打破的坚信：对"眼前这件事是什么"的坚信（前提），
    和对"日常生活应该如此"的坚信（日常）。设计惊讶时先问：这次打破的是哪一种？
  tags: [rule, surprise, strategy]

- id: p27
  title: 低成本制造惊喜：打破"对日常的坚信"，用禁忌主题
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "有效的方法是，不要颠覆对前提的坚信，而是打破对日常的坚信，用'禁忌主题'就能令人吃惊。这样虽然会减少惊讶，但有一定的缓解疲劳和厌倦的效果。"
  summary: |
    颠覆前提要长期说谎、成本极高；想轻松地制造惊喜，就动用禁忌主题打破"日常生活中不会出现这个"的坚信。
    惊讶弱一些，但足以缓解疲劳厌倦。
  tags: [rule, surprise, taboo]

- id: p28
  title: 惊喜设计实施三步（掌握疲劳时机→先构建误解→再暴露误解）
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "1. 掌握玩家疲劳和厌倦的时机……2. 事先构建让玩家产生误解的游戏主题……3. 设计能'暴露'误解的游戏剧情。"
  summary: |
    惊喜设计的操作顺序：先定位用户疲劳厌倦达到顶峰的时机→在此之前花长时间让他建立错误坚信→
    再设计暴露误解的剧情，让两种坚信同时落空。
  tags: [rule, procedure, surprise]

- id: p29
  title: 有意识地使用消极主题，不必怕人格被怀疑
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "设计师必须舍弃自己人格可能被怀疑的不安心理，有意识地使用消极主题。"
  summary: |
    反派、暴力、肮脏、死亡等消极主题是制造惊讶的必需原料。
    设计者要克服"用这些东西显得我很坏"的不安——使用它们是为了用户的体验，不是个人品味。
  tags: [rule, taboo, mindset]

- id: p30
  title: 以不引起怀疑的程度让用户赢
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "游戏通常会以不引起怀疑的程度让玩家获胜，然后让其心情愉快地去冒险。"
  summary: |
    设计"侥幸"体验时暗中提高用户获胜概率，但幅度必须小到用户察觉不到。
    让他把好运当成自己努力的结果，心情愉快地继续。
  tags: [rule, probability]

- id: p31
  title: 10种禁忌主题清单
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "本书总结了10种具有代表性的禁忌主题……性/饮食/得失/认可 肮脏/暴力/混乱/死亡 侥幸与偶然/个人隐私"
  summary: |
    制造惊讶的原材料库，共10种：本能4种（食/饮食、得失、认可、性）＋回避4种（肮脏、暴力、混乱、死亡）
    ＋侥幸与偶然＋个人隐私。在"日常生活中不应出现"的前提下，让任何一个登场就能打破对日常的坚信、消除疲劳厌倦。
  tags: [checklist, taboo, surprise]

- id: p32
  title: 禁忌主题的4个检验指标
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "'这个体验，描绘的是人类本能的欲望吗？'……'这个体验，有人们想要回避的东西吗？'……'这个体验是否让用户下注并祈祷'……'这个体验能体现出个性吗？'"
  summary: |
    判断一个体验是否具有"惊讶制造力"的4问：
    ①描绘人类本能的欲望了吗；②包含人们想回避的东西吗；
    ③让用户下注祈祷了吗；④能体现用户个性（暴露隐私）了吗。
  tags: [checklist, taboo, evaluation]

- id: p33
  title: 惊喜设计是让体验持续下去的"必要之恶"
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "惊喜设计，可以表现为让体验持续下去的必要之恶。……当你想要创造一种能够被很多人接受的流行体验时，你绝对不能忘记这个观点。"
  summary: |
    理想用户若永不知疲倦就不需要惊喜；但面向大众的流行体验必然面对会累的普通人，
    因此惊喜设计不可省略——它是维持长体验的必要成本。
  tags: [principle, surprise, necessity]

- id: p34
  title: 非生活必需品必须持续制造惊喜
  type: principle
  source_chapter: 第2章 · 惊喜设计
  source_quote: |
    "游戏不是生活必需品，所以需要产生惊喜。"（岩田聪）
  summary: |
    生活必需品不会被厌倦（没人对洗涤剂厌烦），非必需品随时可被抛弃。
    你的产品越接近"非必需"，就越有义务不断制造新鲜和惊喜，这是它的宿命。
  tags: [maxim, surprise, product]

- id: p35
  title: 把信息碎片分散在环境中，让用户自己收集构筑故事（环境故事）
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "'环境故事'，玩家自发地收集分布在环境中的信息，构筑故事，它就是这样一种故事表达方式。"
  summary: |
    大脑本能地讨厌信息分散、会自动拼出"发生了什么"。
    想传达复杂信息时，不必讲完整——把碎片分散布置在环境里，让用户自己收集、推理、构筑。
  tags: [rule, storytelling, environment]

- id: p36
  title: 把每个场景的信息量最小化，让发展容易被预测
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "首先，将玩家必须理解的每个场景的内容最小化。每个场景的信息量减少，故事就容易被理解，未来的发展就容易被预想到，很快就会有节奏。"
  summary: |
    单个场景塞太多信息，用户就预测不了走向、跟不上节奏。
    把每个单元必须理解的内容压到最小，用户才能形成预想，投入下一个对比。
  tags: [rule, information-design, pacing]

- id: p37
  title: 用节奏和对比把体验排列成波浪
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "节奏和对比，让一连串的体验像波浪一样愉快地摇摆，让人忘记时间。"
  summary: |
    按信息量和主动/被动两个维度交替排列体验（信息多的被动段→信息少的主动段……），形成波浪。
    没有波浪就疲劳厌倦，有波浪用户才能持续投入。
  tags: [rule, pacing, rhythm]

- id: p38
  title: 先紧张后缓和——体验顺序很重要
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "既不让其高度紧张，也不让其高度缓和，先紧张后缓和，体验顺序很重要。"（引桂枝雀"笑，就是紧张和缓和"）
  summary: |
    缓和之所以有解脱感，全靠之前的紧张。
    不要从头到尾一个强度，要把紧张安排在缓和之前——顺序本身就是设计对象。
  tags: [rule, pacing, order]

- id: p39
  title: 用伏笔制造时间差：先埋暗示，后揭示含义
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "在不知道某个信息的真正含义的情况下，先提示，然后利用时间差让对方注意到其真正的含义。这是非常精细的技巧。它被叫作……伏笔。"
  summary: |
    把重要信息的真正含义藏起来，只先呈现现象；
    等用户日后恍然大悟"原来那个是这个意思"，会产生强烈的快感和向别人叙述的冲动。
  tags: [rule, foreshadowing]

- id: p40
  title: 不要明确说明一切，让用户自己当解说员
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "游戏总是不明确说明眼前发生的事情，让玩家备受折磨。……玩家运用五感和思考来叙述故事，这对大脑来说是一种很充实的体验。"
  summary: |
    事情不要全说完。留出让用户用五感和思考自己拼出"发生了什么"的余地——
    自己叙述出的故事才有充实感和参与感。
  tags: [principle, storytelling]

- id: p41
  title: 必须让用户切实感受到成长，否则瞬间被抛弃
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "如果无法让玩家切实感受到成长的话，那么就会在瞬间被抛弃。"
  summary: |
    用户不关心虚构人物变强了多少，只关心自己有没有变化。
    长体验若不能让用户感到"我变了/我变强了"，再精美也会被放弃。
  tags: [rule, growth]

- id: p42
  title: 虚构故事只是手段，必须让用户在现实中实际成长
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "游戏设计师真正想要描绘的，不是在游戏中展开的'虚构故事'，而是玩家自身成长的'故事'。……设计师必须让作为现实存在的玩家在现实世界中实际成长。"
  summary: |
    情节、角色、世界观都是手段，真正要设计的是用户在现实中发生的改变。
    评估内容时先问：用户离开之后，现实中的他哪里不一样了？
  tags: [principle, growth, means-end]

- id: p43
  title: 先让用户认识整体与共同性质，再让"空缺"被识别
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "如果没有事先认识到整体的范围和共同的性质，就无法将'空缺'作为'空缺'来认识。……人们发现空缺就想填，而且不由自主就填了。"
  summary: |
    收集欲的启动顺序：先给用户看整体和规则（1～8），"缺的那块"（9）才会被识别为空缺，人就会不由自主去填。
    想让人收集，先让他看见"图鉴"的形状。
  tags: [rule, collection, gap]

- id: p44
  title: 成长必需重复，设计要点是让人不厌其烦地重复
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "重复是成长必需的，重要的是如何让人不厌其烦地将某种行为反复进行的体验设计。"
  summary: |
    一切成长都来自重复，而人天然厌倦重复。
    设计者的核心课题不是"要求重复"，而是把重复包装成每次都有空缺可填、可期待的体验。
  tags: [principle, repetition, growth]

- id: p45
  title: 给重复配上节奏，让人不自觉跟随
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "如果被指示举起手臂66次，人们完全没有劲头。……广播体操还有一个促进反复的东西，那就是节奏。"
  summary: |
    明确的次数要求让人疲惫，均匀的节奏却让人身体先动起来。
    把要重复的行为嵌进节奏（音乐、固定间隔）里，空缺会一个接一个被自动填上。
  tags: [rule, repetition, rhythm]

- id: p46
  title: 不给"问题已解决"的间隙，让紧张感持续
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "对于已经解决的问题，我们的内心会轻易消除紧张感，而对于尚未解决的问题，则会保持紧张感。……通过让方块持续掉落，设计师使玩家得不到缓解紧张感的间隙。"
  summary: |
    利用蔡格尼克效应：想让人停不下来，就不给"告一段落"的空隙，让下一个问题立刻出现。
    间隙一出现，紧张释放，用户就会离开。
  tags: [rule, tension, zeigarnik]

- id: p47
  title: 故事开始必须提示未解决的问题；有未解决问题的人才是主人公
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "为让读者对故事产生兴趣，故事开始一定会提示未解决的问题。……'有未解决问题的人物'才是主人公。"
  summary: |
    兴趣来自未解决。开场就摆出一个悬而未决的问题，并把它挂在主人公身上——
    没有"未解决问题"的主人公无法承载兴趣。
  tags: [rule, story-opening]

- id: p48
  title: 准备风险与回报不同的多个选项，让用户自己选择斟酌
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "从设计师的角度来看，就是准备风险和回报不同的几个选项，设计让人自由选择斟酌的体验。"
  summary: |
    不要给唯一最优解。提供"低风险低回报/高风险高回报"式的并列选项，
    用户会凭直觉斟酌并走出属于自己的路径，在正确选择后切实感到成长。
  tags: [rule, choice, risk-reward]

- id: p49
  title: 让用户自行调整难度
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "玩家调整游戏难度。实际上，这是成长不可或缺的要素。"
  summary: |
    把难度选择权交给用户（走还是跑、收不收集、用不用高风险打法），
    每个人都会自动玩到"对自己难度适中"的程度，从而获得最大成长。收集、选项等主题都兼任难度调节器。
  tags: [principle, difficulty, growth]

- id: p50
  title: 失败归因于用户，成功及时表扬——以用户为主语的反馈
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "游戏让玩家觉得'失败是你的错'是必要的。……为让玩家真心'想变得更好，想成长'，只能让玩家在失败的基础上后悔自己的操作。"
  summary: |
    失败要让用户归因于自己的操作（而不是运气或设计），成功时要明确表扬"你做得好"。
    这样用户才会产生"我要变强"的真实意愿。
  tags: [rule, feedback]

- id: p51
  title: 无论何时都必须对用户的行为做出反应
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "无论何时都必须对玩家的行为做出反应，这才是游戏最基本的结构。"
  summary: |
    交互媒体的基本义务：有输入必有相应的输出。用户每个行为都要得到评价（好/坏），
    否则他无法体会自己行为的意义，也就不会继续。
  tags: [rule, feedback, interaction]

- id: p52
  title: 共鸣的三个必要条件
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "所谓共鸣，就是深信'对方一定和自己有着强烈的相同想法'的状态。共鸣有三个必要的条件。"
  summary: |
    设计共鸣的检查清单：①用户对主人公有兴趣；②用户相信主人公与自己想法相同；
    ③用憎恨以外的情感。三条件齐备，用户才会把主人公的心情当成自己的心情。
  tags: [checklist, empathy]

- id: p53
  title: 绝不能通过憎恨产生共鸣
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "'是他不好，我恨他'，这种把责任推给别人的想法无法促进玩家成长，所以必须想办法避免。"
  summary: |
    归咎他人（憎恨）虽然也是强烈情感，但会把责任外移、阻断成长。
    设计情感体验时必须引导用户绕开憎恨，用其他情感达成共鸣。
  tags: [rule, empathy, growth]

- id: p54
  title: 打击主人公——让主人公不幸来打动用户
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "如果想强烈地打动玩家的心，只要强烈地打动主人公的心就可以了。……给主人公带来无法解决的问题，使其不幸并遭受打击。也许你不想这么做，但这是设计游戏体验的设计师必须去做的。"
  summary: |
    镜像神经元让用户的情绪跟随主人公。
    想打动用户，就必须"残酷"地让主人公遭遇打击和不幸——这是创作者绕不开的必修动作。
  tags: [rule, empathy, protagonist]

- id: p55
  title: 把同行者设计成"麻烦的所在"
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "同行者有着不断给主人公制造麻烦的宿命。麻烦的同行者在推动故事向前发展的同时，还是将玩家的兴趣吸引到主人公身上的引擎。"
  summary: |
    伙伴不是来帮忙的，是来添乱的。身边人制造的麻烦无法无视，
    既持续打击主人公、推动剧情，又让用户和主人公对同一对象产生相同情绪（共鸣的第一步）。
  tags: [rule, companion, empathy]

- id: p56
  title: 先给能喜欢上同行者的小插曲，再把同行者逼入绝境
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "在加入能喜欢上同行者的小插曲之后，把同行者逼到死亡或绝望的边缘就可以了。"
  summary: |
    逆转共鸣的做法：先安排让用户看到同行者可爱/可敬之处的小事件，然后让他陷入死亡或绝望。
    用户会在瞬间超越憎恨，与主人公一起呐喊——成长发生在这里。
  tags: [rule, empathy, reversal]

- id: p57
  title: 让用户亲手决定命运走向、面对从未体验过的状况
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "用自己的双手来决定让自己产生共鸣、倍加珍惜的生命的走向。在从未体验过的状况下，只根据现在的自己能想到的做决定……一切都是为让玩家拥有自己意志的体验。"
  summary: |
    故事的终点不是结局，而是"意志"：让用户在毫无先例的处境中，亲手为珍视之物做决定。
    这样的体验会驱使用户开始叙述自己的故事。
  tags: [principle, agency, ending]

- id: p58
  title: 刻意保留解释余地
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "设计师刻意在故事中保留没有明确的部分，引导玩家拥有'自己怎么想'的意志。"
  summary: |
    不要把含义说尽。故意留下没有明确答案的部分，让每个用户带着自己的解释去叙述——
    解释各异的作品会被评价为"深刻、引人深思"。
  tags: [rule, ambiguity]

- id: p59
  title: 让故事回到起点，让用户对比出自己变了
  type: principle
  source_chapter: 第3章 · 故事设计
  source_quote: |
    "正因为想让通过故事成长的人注意到自己的成长，设计师才特意让主人公回到家这个起点，让玩家想起经历故事之前的自己，进而比较经历故事体验前后的自己。"
  summary: |
    成长若不被用户自觉，就等于没发生。
    把结局安排回起点（同样的场景、同样的任务），用户会在对照中亲眼看到自己的变化。
  tags: [principle, ending, growth]

- id: p60
  title: 只有强烈激发感情的体验才会变成长久记忆
  type: principle
  source_chapter: 第4章 · 体验设计的本质
  source_quote: |
    "情景是否给人留下深刻的印象，取决于体验者的感情是否强烈。……你现在记得的，应该是强烈震撼、激发你的情感的体验。"
  summary: |
    记忆的筛选标准是感情强度：被强烈打动过的情景才会长期保存。
    想被记住，先追求感情的强度，而不是信息的完整。
  tags: [principle, memory, emotion]

- id: p61
  title: 从自己的记忆出发做体验设计
  type: principle
  source_chapter: 第4章 · 体验设计的本质
  source_quote: |
    "从追溯你的记忆开始，你的体验设计就开始了。以确实激发你个人感情的体验（＝记忆）为基础，设计出打动无数人心灵的体验就可以了。"
  summary: |
    设计的合法起点是自己的记忆：那些确实强烈激发过你感情的经历。
    以它们为原型，向外推及"所有人共同的性质和记忆"，就能做出打动无数人的东西。
  tags: [principle, memory, starting-point]

- id: p62
  title: 不要直接追求好结果，重新设计"得到结果的过程"
  type: principle
  source_chapter: 第5章 · 应用篇（总论）
  source_quote: |
    "'有趣'终究是结果，不是过程。正因为如此，设计师必须思考'怎样的过程才能在结果上得到有趣的评价'。"
  summary: |
    好方案、好产品是副产品；直接冲着结果去会做出"结果正确、过程痛苦"的东西。
    把"思考/制作"这个过程本身设计成快乐的体验，好结果的概率自然提高。
  tags: [principle, process]

- id: p63
  title: 改变的不是物本身，而是物所处的心理脉络
  type: principle
  source_chapter: 第5章 · 应用篇（总论）
  source_quote: |
    "重要的不是石头本身，而是石头和用户交互的环境。用户在具体的环境中接触石头，这样才会产生体验的价值。"
  summary: |
    面对"无聊的东西"，不要死磕改进物品本身，去看它被使用的环境（放在路中央的石头就想踢）。
    体验价值＝物×环境×心理状态。从观察无聊、不顺畅的体验入手，找到拉低价值的心理脉络再设计。
  tags: [principle, context]

- id: p64
  title: 三种设计的选择指标（难理解→直觉；疲劳厌倦→惊喜；没价值→故事）
  type: principle
  source_chapter: 第5章 · 应用1 思考/策划
  source_quote: |
    "1. 如果问题令人难以理解，运用直觉设计。2. 如果问题让人疲劳和厌倦，运用惊喜设计。3. 如果问题没有价值，运用故事设计。"
  summary: |
    应用体验设计前的快速分诊：问题出在"难以理解"用直觉设计；
    出在"疲劳厌倦"用惊喜设计；出在"没有价值"用故事设计。
  tags: [checklist, decision]

- id: p65
  title: 思考/策划卡住时，停止考虑他人、思考个人隐私
  type: principle
  source_chapter: 第5章 · 应用1 思考/策划
  source_quote: |
    "当你不得不进行'思考/策划'的时候，请试着停止考虑他人。取而代之，请思考一下个人的隐私。越是暴露个人隐私，越能让你自己感到惊讶和兴奋。"
  summary: |
    策划时满脑子"顾客、上司"会让灵感枯竭。用"个人隐私"主题重启思考：想那些"对所有人保密、
    在别人面前不能说的话"，让你呼吸急促、心跳加速就成功——先让自己惊讶，才能持续思考。
  tags: [rule, ideation, taboo]

- id: p66
  title: 思考时不急于下结论，碎片化收集让你兴奋确信的事
  type: principle
  source_chapter: 第5章 · 应用1 思考/策划
  source_quote: |
    "在持续思考的时候，也不要急于下结论，将自己觉得兴奋的事情、能产生共鸣的事情、能确信的事情碎片化地收集起来，这是诀窍。不要管思考的东西是否有用……"
  summary: |
    持续思考的诀窍：先不收敛。把让你兴奋、共鸣、确信的东西记成碎片，别管有没有用——
    此刻的目标只是远离疲劳厌倦、保持思考。
  tags: [rule, ideation]

- id: p67
  title: 把思考碎片摆在眼前，从共同点中发现最重要的主题
  type: principle
  source_chapter: 第5章 · 应用1 思考/策划
  source_quote: |
    "把这些思考碎片放在眼前，你一定会产生直觉……从思考碎片的共同点中发现对你来说重要的事情。"
  summary: |
    把记下的碎片（笔记、便利贴）铺在眼前，凭直觉找出它们的共同点——
    深处通常藏着你人生最重要的主题（理想、价值观、守护之物）。
  tags: [rule, ideation]

- id: p68
  title: 给策划讲述"失去重要东西、陷入危机"的故事
  type: principle
  source_chapter: 第5章 · 应用1 思考/策划
  source_quote: |
    "讲述一个你失去重要的东西、陷入危机的故事。然后，你自己做一个能找回重要东西的策划方案。"
  summary: |
    给"思考/策划"装上故事：构想一个"如果做出这个方案就能找回自己最重要的东西"的脉络，
    把策划等同于寻找自己的幸福，无意识会驱动大脑持续认真思考。
  tags: [rule, motivation, story]

- id: p69
  title: 不谈"好的策划"，谈"没用的策划"
  type: principle
  source_chapter: 第5章 · 应用2 讨论/引导
  source_quote: |
    "不谈'好的策划'，谈'没用的策划'。"
  summary: |
    会议沉默的根源是"必须说出好点子"的信念。打破这条默认规则——先集体谈"没用的策划"，
    斩断制约团队的锁链，讨论才重获自由，创造性发言才会出现。
  tags: [rule, facilitation]

- id: p70
  title: 主动提好意见、占据优势地位的引导者是二流引导者
  type: principle
  source_chapter: 第5章 · 应用2 讨论/引导
  source_quote: |
    "你不认为主动提出好意见、试图占据优势地位的引导者属于二流引导者吗？"
  summary: |
    引导者的价值不在于自己贡献聪明意见，而在于让成员畅所欲言。
    忍不住抢话、争优势地位的引导者，只会压制讨论。
  tags: [maxim, facilitation]

- id: p71
  title: 舍弃对效率的追求，团队才会出现创造性发言
  type: principle
  source_chapter: 第5章 · 应用2 讨论/引导
  source_quote: |
    "只有舍弃这种对效率的追求，才能让团队变得和睦、活跃起来，出现创造性的发言。"
  summary: |
    谈"没用的话"、共享内部话题看起来低效，但正是这种"浪费"制造了安全感和认同感。
    想要创造性，就要先放弃对"每句话都必须有效"的执念。
  tags: [principle, facilitation, trade-off]

- id: p72
  title: 让团队共享"我们自己的风格"
  type: principle
  source_chapter: 第5章 · 应用2 讨论/引导
  source_quote: |
    "把团队的自我认识当作'我们自己的事情'来谈。简单来说，就是在团队中共享'这个团队的风格'。"
  summary: |
    让成员说出"我们团队都是××的人啊"这类发言，用"假设→尝试→高兴"（大家猜、大家确认）的方式
    固化团队认同——知道什么话能引起共鸣后，讨论自然热烈。
  tags: [rule, team]

- id: p73
  title: 回顾过去的发言，找出深层含义作伏笔
  type: principle
  source_chapter: 第5章 · 应用2 讨论/引导
  source_quote: |
    "回顾过去的发言，提出'深层含义是什么'。从成员提过的意见，以及一度被忽略的主张中找出意义，将其作为伏笔。"
  summary: |
    讨论绕的"弯路"其实是伏笔。之后从被忽略的发言里翻出关键意义
    （"其实答案早就在讨论中出现了"），制造恍然大悟的高潮。
  tags: [rule, facilitation, foreshadowing]

- id: p74
  title: 让团队成员成为英雄，而不是引导者自己
  type: principle
  source_chapter: 第5章 · 应用2 讨论/引导
  source_quote: |
    "从成员过去的意见中找出重要性，就能让那个成员成为英雄。……对引导者来说，重要的不是自己成为英雄，而是让团队成员成为英雄。"
  summary: |
    伏笔手法的真正用途：把"英雄时刻"献给成员——他随口一提的话成了破局关键。
    引导者的成功指标是别人被奉为英雄。
  tags: [rule, facilitation]

- id: p75
  title: 内容不是问题，叙述方式（怎么说）才是问题
  type: principle
  source_chapter: 第5章 · 应用3 传达/演示
  source_quote: |
    "无论内容多么充实，无聊的演示都是无聊的。换句话说，内容不是问题。……重要的不是故事内容（说什么），而是故事叙述（怎么说）。"
  summary: |
    演示（传达）失败时，别再打磨内容。听众疲劳的原因在"怎么说"——
    顺序、节奏、悬念，这些叙述层的设计才是无聊与否的分水岭。
  tags: [maxim, presentation]

- id: p76
  title: 注意力下降发生在"讲话流程无法被预测"的时候
  type: principle
  source_chapter: 第5章 · 应用3 传达/演示
  source_quote: |
    "在演示中注意力下降的时候，是'讲话的流程无法被预测的时候'。"
  summary: |
    听众走神不等于内容无聊，而是他预测不到你接下来要说什么。
    保持吸引力的机制与游戏相同：让听众不断建立"接下来应该是××吧"的假设。
  tags: [rule, presentation, attention]

- id: p77
  title: 用连接词/悬念预告下一张幻灯片，再切换
  type: principle
  source_chapter: 第5章 · 应用3 传达/演示
  source_quote: |
    "用连接词预告下一张幻灯片的内容后再往下进行。……在说完连接词后，切换幻灯片。只要做到这一点，演示就会一下子变得有吸引力。"
  summary: |
    幻灯片切换突然＝注意力最大杀手。切换前先用疑问、话说一半、"例如"等连接词预告下一张的内容，
    让听众的预测先跑起来再翻页。
  tags: [rule, presentation]

- id: p78
  title: 演示中永远不要用"接下来"这个连接词
  type: principle
  source_chapter: 第5章 · 应用3 传达/演示
  source_quote: |
    "有一个连接词不具备让听众想象未来的能力。这个连接词就是'接下来'（序列）。……只要演示中不说'接下来'这个连接词，演示就会变得容易让人看下去。"
  summary: |
    唯一没有预告功能的连接词是"接下来"——它只报顺序，不让听众想象内容。
    想让人看得下去，把"接下来"从演示词汇里删掉。
  tags: [rule, presentation, negative]

- id: p79
  title: 定期在演示中插入禁忌主题和沉默
  type: principle
  source_chapter: 第5章 · 应用3 传达/演示
  source_quote: |
    "定期插入禁忌主题/沉默。……特别有效果的是沉默。推翻演示的前提——'演示者是说话者'，一下子就能吸引听众注意。"
  summary: |
    演示者有责任把听众拉到最后：定期把10种禁忌主题（性、饮食、得失、认可、肮脏、暴力、混乱、死亡、
    侥幸偶然、个人隐私）织进话语的每个角落；沉默是最强的惊喜——它推翻"演示者在说话"这一前提。
  tags: [rule, presentation, taboo]

- id: p80
  title: 最后再展示一次演示开头的幻灯片
  type: principle
  source_chapter: 第5章 · 应用3 传达/演示
  source_quote: |
    "最后再展示一次演示开始放的幻灯片。……在看演示之前无法了解的事情，在看了演示之后就能了解了。我们要给听众那种成长的实在感。"
  summary: |
    开场先展示观点/问题/总结（当时看不懂），演示结束前再放同一页——
    听众能亲自确认"我现在懂了"，获得成长的实在感，坚持听完不疲劳。
  tags: [rule, presentation]

- id: p81
  title: 优先考虑第一次使用的用户
  type: principle
  source_chapter: 第5章 · 应用4 设计/产品设计
  source_quote: |
    "优先考虑第一次使用的用户，一定要让其觉得产品简单、易用。……'第一次'是人生只有一次的最有效的学习机会，体验设计师绝对不能错过。"
  summary: |
    第一次使用时学习效率最高（初始效应），且第一次用不顺就没有第二次。
    设计资源优先砸给"第一次的用户"，让他们觉得简单易用。
  tags: [principle, first-time-user]

- id: p82
  title: 时刻意识到"不熟悉也没热情的普通用户"的存在
  type: principle
  source_chapter: 第5章 · 应用4 设计/产品设计
  source_quote: |
    "无论何时，设计师都应该意识到存在'对产品不熟悉，也没有热情的普通用户'。"
  summary: |
    开发者为热爱产品的深度用户设计，会让普通用户掉队。
    时刻假设有一个不熟悉产品、也没有热情的普通用户在场，为他保住简单易用。
  tags: [rule, persona]

- id: p83
  title: 用户的人生才是主角，产品只是配角
  type: principle
  source_chapter: 第5章 · 应用4 设计/产品设计
  source_quote: |
    "对用户来说，重要的不是产品，而是用户自己的人生。用户的人生才是主角，产品只是衬托主角的配角。"
  summary: |
    不要执着于"产品被一直使用"。用户使用或不使用都是他的自由；
    产品存在的意义是让他的人生更美好，不能抢夺他的时间来证明自己。
  tags: [maxim, product, humility]

- id: p84
  title: 刻意设计"让体验停止"（回归日常的情节）
  type: principle
  source_chapter: 第5章 · 应用4 设计/产品设计
  source_quote: |
    "这里需要的是，在了解惊喜设计原理和效果的基础上，刻意让体验停止的体验设计。通过回归日常的情节设计，将用户从产品中抽离。"
  summary: |
    会"结束"的体验才不吞噬用户人生：在体验收尾处刻意不用惊喜设计（不再延长体验），
    用回归日常的宁静情节（动画片结尾的夕阳堤坝）宣告"体验结束了"，让用户心情愉快地离开。
  tags: [principle, stopping, ethics]

- id: p85
  title: 提供作弊选项，让用户自由选择
  type: principle
  source_chapter: 第5章 · 应用4 设计/产品设计
  source_quote: |
    "提供作弊选项，让用户自由选择。……所谓产品设计，或许就是设计出用户的使用自由。"
  summary: |
    给用户保留"跳过、作弊、随时停止"的选项。每次自由选择都在确认"这是我自己决定的"，
    这份自由反而是用户反复回来的力量。产品设计的本质是设计用户的使用自由。
  tags: [rule, freedom]

- id: p86
  title: 命令和指示无法让人行动，必须重新设计体验
  type: principle
  source_chapter: 第5章 · 应用5 培养/管理
  source_quote: |
    "用一个命令就让孩子动起来，这种想法本身就太天真了。要想让孩子按照父母的意志行动起来，父母就必须改变自己的做法。"
  summary: |
    对方不行动时，换一句命令没有用。命令和指示本身就制造不出"想做"的心情；
    唯一出路是重新设计他经历的过程（让他自发假设→尝试→高兴）。
  tags: [principle, teaching, management]

- id: p87
  title: 先假定对方没有恶意，问题出在自己的命令和指示上
  type: principle
  source_chapter: 第5章 · 应用5 培养/管理
  source_quote: |
    "我可以百分之百地相信她们并没有恶意。这样想的话，有问题的就是我的命令和指示了。"
  summary: |
    对方不配合时先排除"他故意作对"的解释：假定对方无恶意，那么不行动必有合理理由——
    然后去找那个理由（多半是信息缺失或厌倦），而不是加压。
  tags: [rule, management, mindset]

- id: p88
  title: 确认对方能否用具体的固有名词想起任务
  type: principle
  source_chapter: 第5章 · 应用5 培养/管理
  source_quote: |
    "确认能否用具体的固有名词想起任务。……孩子不会收拾玩具的原因，绝对不是因为他们本身没有干劲，而是'因为他们对场所没有记忆'。"
  summary: |
    "不行动"常常不是没干劲，而是无法具体想起"做什么、放哪里"。
    下达任务前自检：对方能否用具体固有名词（"木架第二层"）想起它？不能就先给具体提示或提问。
  tags: [rule, instruction]

- id: p89
  title: 故意试错/体验错误，让人感到平时的效果
  type: principle
  source_chapter: 第5章 · 应用5 培养/管理
  source_quote: |
    "故意试错/体验错误。……我认为有必要用错误的方法刷牙，以体验平时刷牙的效果。"
  summary: |
    天天做、看不见效果的事必然厌倦。故意让对方（或自己）用错误方式做一遍，
    "错了！不行！"的瞬间反而让人体会到平时的效果，重新认真起来。
  tags: [rule, learning, trial-error]

- id: p90
  title: 教的一方与被教的一方一起体验未知的事情
  type: principle
  source_chapter: 第5章 · 应用5 培养/管理
  source_quote: |
    "教的一方和被教的一方一起体验未知的事情。……我准备了自己没读过的书和包含我不知道的东西的图画书。'哦！''真有趣！'我一边感叹一边阅读。"
  summary: |
    教的人完全知道答案时，双方都无聊。选自己也不知道的内容一起探索，
    你的真实感叹会传染——听的人变得乐意，教的人也乐在其中。
  tags: [rule, teaching]

- id: p91
  title: 教与被教双方都要成长
  type: principle
  source_chapter: 第5章 · 应用5 培养/管理
  source_quote: |
    "其实，在做父母的同时，我们也应该学习父母的正确行为方式。孩子作为孩子，父母作为父母，各自成长，正因如此，亲子共同生活的一系列体验才会变得丰富多彩。"
  summary: |
    别只盯着对方的成长指标。管理者/父母自己也要处于学习和成长中——
    双方都是"发现、惊喜、寻找意义"的体验主体，关系中的体验才会丰富。
  tags: [principle, growth, management]
```
