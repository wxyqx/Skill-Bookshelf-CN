# Scanner C（第4-5章）候选

## 第一部分：章节 digest

### 第四章 自力更生：游击营销和增长黑客

本章核心论点：创业早期不要急于追逐风险投资，应先用自有资金验证商业模式。过早拿到大钱会掩盖问题、扼杀创新，把公司从探索模式推向扩张模式（创业基因报告：70%的创业公司至少在一个维度上过早扩张）。作者给出自力更生的具体路径：选择不需要大额前期投入的业务；用兼职、全职工作或休假养活公司（耐克奈特、GitHub、FUBU、贝尼奥夫）；融资时机的原则是"先验证、后融资"。营销侧提供了一套低成本获客工具箱：与媒体建立关系（研究Upworthy的标题A/B测试流程、把自己定位成记者的数据源和领域专家、写客座文章）；游击营销（15个战术案例加12条规则，核心是与众不同、激发情感反应、鼓励分享）；集客营销（内容+SEO，4个起步问题+15条推广策略，目标是填补内容空白、追求实用而非新奇）；价值观品牌（Soma、Ritual、bkr，与客户的内心对话）；投资视频制作（美元剃须俱乐部用4500美元视频撬动10亿美元品牌）；故事营销（12种叙事类型，故事必须匹配品牌、强化核心信息、引起受众共鸣）。最后讲增长黑客：肖恩·埃利斯2010年提出，以业务增长为目标的快速实验过程，贯穿"获客—激活—收入—推介—留存"五阶段漏斗。结论：自力更生的公司发展慢，但最终回报同样可观，关键是解决真实问题。

### 第五章 独角兽猎人：找到未来的赢家

本章以投资人（"独角兽猎人"）视角讲解如何区分赢家与输家。评估顺序：先看团队——CEO领导力是对领导能力的第一项测试，能仅凭言语和股权聚拢顶尖人才的人才有"神奇魔力"；警惕名校与头衔两个筛选陷阱，只有个人品质才是最重要的。再看市场规模——小市场像"玻璃缸里养鲸"，必须有清晰通往更大市场的道路，否则风险投资不会参与。然后看客户认知——CEO必须明确说清客户具体是谁，用数据（DAU/MAU、留存率、参与模式）而非感觉验证市场。产品要顺应趋势并尽早介入、成为社区核心；必须追求"卓越"而非"优秀"，因为业务越可扩展越是赢家通吃。撬开市场只有两条路：产品好出很多个数量级，或者与其他人截然不同（iPhone、谷歌、Skype、Slack、Affirm）。商业模式归结为两类（客户付费/广告），四种变现方式（订阅、易耗品、升级收费、平台），强调可持续收入与客户锁定；照搬他人商业模式前必须逐一核对其成立要素（"优步化"倒闭潮）。专利对多数初创公司无价值（Jawbone坐拥专利仍破产，对比WhatsApp无专利却以190亿美元被收购）；不要硬套热门技术；早期设计创新重于技术创新（戴森）。媒体关注是低成本放大器，但需真实势能支撑（Yo应用失败）。最后讲尽调透明原则与"真正独特的元素"——团队成员间的情感纽带与企业文化。

## 第二部分：五类 YAML 原始候选

### 1. frameworks

```yaml
- id: fc01
  title: 游击营销12条规则
  type: framework
  source_chapter: 第四章
  source_quote: |
    "这里是策划成功的游击营销活动的12条规则：（1）活动的形式要有创意。（2）问问你自己为什么这样做很重要。（3）在活动中挑战你的受众。（4）让活动变得有趣和诙谐。（5）尽可能地简化你想要传播的信息。（6）寻找合适的人群。"
  summary: |
    作者在15个游击营销案例后总结出的策划清单：创意形式、明确活动意义、挑战受众、有趣诙谐、简化信息、找对人群、尽早让有影响力的人参与、允许离谱、利用走红视频照片、允许受众参与并分享、善用社交平台、绝不复制他人。用作策划低成本品牌活动的检查表。
  tags: [marketing, guerrilla-marketing, checklist]
- id: fc02
  title: 增长黑客五阶段营销漏斗
  type: framework
  source_chapter: 第四章
  source_quote: |
    "增长黑客的营销漏斗从上至下分别为：（1）客户获取——最优化在线客户的获取。（2）客户激活——与访问你的网站的客户进行互动。（3）收入增长——增加首次和重复销售。（4）产品推介——让客户分享你的产品。（5）客户留存——建立客户忠诚度。"
  summary: |
    增长黑客的标准工作框架：把业务拆成获客、激活、收入、推介、留存五个环节，对每个环节分析用户行为数据，设计创造性实验，实验后马上调整并重新设计，直到指标最优。适合预算紧张的创业公司在早期获得上升势头。
  tags: [growth-hacking, funnel, experiment]
- id: fc03
  title: Upworthy标题A/B测试四步法
  type: framework
  source_chapter: 第四章
  source_quote: |
    "（1）为每一篇文章批量制作25个可用的标题。（2）选择其中最出色的4个标题作为候选。（3）把它们放在推特或者其他的社交网络上，然后测试相应的点击量。（4）选出表现最好的标题，不要管它是否符合你的口味。"
  summary: |
    用数据代替直觉做标题决策的流程：先批量写25个标题，人工筛出4个候选，放到社交网络测点击量，最后选数据最优者而非个人偏好者。可迁移到任何需要吸引点击的场景（邮件、落地页、新闻稿）。
  tags: [ab-testing, copywriting, media]
- id: fc04
  title: 集客营销起步四问
  type: framework
  source_chapter: 第四章
  source_quote: |
    "你可以从询问自己如下4个问题来开始你的集客营销活动：（1）你所在行业的人会在网上点击什么？（2）有哪些信息是他们有需要但还没有获得的？（3）你如何通过一种更有效的方式把这些信息传递给他们？（4）有哪些东西是你能提供而其他人无法提供的？"
  summary: |
    启动内容营销前的定位框架：先弄清目标受众的点击习惯，找到信息缺口，规划更高效的传递方式，明确自己独有的增值点。配合"研究竞争对手高流量内容→提取关键词→写出更好的新版本"的操作路径使用。
  tags: [inbound-marketing, content, positioning]
- id: fc05
  title: 集客营销内容推广策略清单
  type: framework
  source_chapter: 第四章
  source_quote: |
    "每天都有数百万篇的博文被上传到互联网上，所以你不能指望人们能神奇地找到你发布的内容，你需要积极地去推广。下面是一些你可以采用的策略：（1）从第一天起就建立你的邮件列表……（2）创建用户画像。"
  summary: |
    15条内容推广策略：建邮件列表并给注册回报、创建用户画像、参加目标客户活动、出现在客户聚集的社区并遵守其潜规则、用Hubspot等工具分析数据、SEO争取关键词顶部位置、站内测验互动、动员全员分享、动态表单收集信息、实时聊天降跳出率、建引流站点、跨媒体改写内容、结构化FAQ、买量引流、语音商务平台占位。
  tags: [inbound-marketing, seo, distribution]
- id: fc06
  title: 12种品牌叙事类型
  type: framework
  source_chapter: 第四章
  source_quote: |
    "每一家企业都能构建出很多种不同类型的故事。在这里我列出了一些最受欢迎的故事类型……◎ 成功的故事……◎ 你自己的故事……◎ 涉及因果的故事……◎ 让人担心的故事……◎ 利用数据的故事……◎ 企业成长的故事……◎ 趋势的故事……◎ 关于未来的故事……◎ 弱者的故事……◎ 灾难的故事……◎ 古怪的故事……◎ 丑恶的故事"
  summary: |
    可供企业试验的12种故事类型：草根成功、创始人亲身经历、公益因果、恐惧防范、专有数据、高速成长、社会趋势、未来想象、以弱胜强、灾难逆转、古怪猎奇、丑恶吸睛。用法是多种类型并行实验，选出能匹配品牌、强化核心信息、引起共鸣的那一种。
  tags: [storytelling, branding, framework]
- id: fc07
  title: 10分钟MBA：两种根本商业模式
  type: framework
  source_chapter: 第五章
  source_quote: |
    "实际上只有两种真正行得通的商业模式：（1）客户直接付钱给你；（2）广告商付钱给你。所有其他的商业模式都是这两种模式的子集。"
  summary: |
    把所有商业模式压缩为两大类：客户付费（要求生命周期平均支付显著高于获客成本加货物成本）与广告模式（要求海量用户加高参与度）。所有具体模式都是这两者的子集。用于快速审视一家公司"钱从谁来、能否规模化"。
  tags: [business-model, framework]
- id: fc08
  title: 四种用户变现方式
  type: framework
  source_chapter: 第五章
  source_quote: |
    "真正重要的是这家公司是否能深度地将用户变现。下面让我们先来看一下四种非常受欢迎的将用户变现的方式：订阅、易耗品的销售、产品功能升级收费、平台。"
  summary: |
    投资人偏好的四种可持续收入模式：订阅（可预测收入、低门槛试用）；易耗品（复购，尤其是与高价一次性产品捆绑，如打印机与墨盒）；功能升级收费（仅适合升级空间近乎无限的产品，如卡牌游戏）；平台（按交易抽成，网络效应使其难以复制、最强大）。
  tags: [business-model, monetization, recurring-revenue]
- id: fc09
  title: 优步模式成立要素清单
  type: framework
  source_chapter: 第五章
  source_quote: |
    "共享模式能如此成功，不仅因为它能给用户带来方便，还因为它有着如下这些特征：◎ 有经常性收入流。◎ 客户会反复多次地使用该产品，并且客户的参与度非常高。◎ 客户的生命周期价值要比获客成本与服务本身的成本之和更高。"
  summary: |
    拆解优步成功的8个要素：经常性收入流、高频高参与、生命周期价值大于获客成本加服务成本、司机与客户配对形成的平台网络效应、难以绕过平台直联、服务优于传统出租车、客户可轻易反馈、良好用户体验。用途：照搬任何商业模式前，逐项核对自己所在行业是否具备这些前提要素。
  tags: [business-model, uberization, checklist]
- id: fc10
  title: 客户访谈八问
  type: framework
  source_chapter: 第五章
  source_quote: |
    "（1）你为什么需要这款产品？（2）为什么贵公司需要这款产品？（3）购买这款产品需要获得谁的批准？（4）你的企业有哪些利益相关者？（5）在从1到10的衡量范围里，你会如何标注这款产品对于你们的重要程度？……（8）你是否愿意现在就下订单？"
  summary: |
    B2B客户深访的问题清单，覆盖需求动机、决策链、利益相关者、重要度评分、竞争对比、替代品与下单意愿。作者建议把访谈录像录音，积极的记录还可作为市场需求真实存在的早期证据展示给投资人。
  tags: [customer-interview, b2b, validation]
- id: fc11
  title: 广告模式成立的两个基本条件
  type: framework
  source_chapter: 第五章
  source_quote: |
    "广告模式想要能行得通一般需要符合两个基本条件：第一个条件是大量的用户……第二个条件是用户的高参与度，用户的留存率越高，在网站上停留的时间越长，企业的营业收入就越高。"
  summary: |
    判断广告模式是否适用的两个硬条件：数百万级活跃用户（在线广告单价低）+高参与度与留存（用户每周多次使用）。低频应用（如每两周用一次）不适合广告模式，适合者通常是大众媒体与社交媒体类公司。
  tags: [business-model, advertising, criteria]
- id: fc12
  title: 独角兽猎人的评估流程
  type: framework
  source_chapter: 第五章
  source_quote: |
    "我会向你解释在管理团队中哪些品质才是最重要的，如何判断某个商业模式是否能够实现规模化，以及如何发现一家真正做好了融资准备的公司。"
  summary: |
    作者的初创公司评估顺序：团队（CEO领导力与成员纽带）→市场规模（增长天花板与退出潜力）→客户认知与数据验证（DAU/MAU、留存率）→是否顺应趋势→产品是否卓越→独特"秘诀"→商业模式与变现→客户锁定能力→软硬件结构→专利价值→设计→媒体潜力→尽调透明度→团队文化。可作为早期项目尽调的完整检查路径。
  tags: [investing, due-diligence, unicorn]
- id: fc13
  title: 专利价值评估四问
  type: framework
  source_chapter: 第五章
  source_quote: |
    "这项专利是否真正构成了进入壁垒？如果想在市场上开展业务，这项专利是否是必需的？这项专利是否可以被用来阻挡你的竞争对手，或者向对方收取专利许可费？如果想要绕开这项专利，在具体的操作上会有多难？"
  summary: |
    判断专利是否真正有价值的四个问题：是否构成进入壁垒、开展业务是否必需、能否阻挡对手或收取许可费、绕开难度多大。结论是大多数软件初创的专利无价值，只有半导体、制药、新材料等资本密集核心技术领域才值得早期投入。
  tags: [patent, ip-strategy, investing]
- id: fc14
  title: 有效标题的十条建议
  type: framework
  source_chapter: 第四章
  source_quote: |
    "（1）描述清晰。（2）使用对话的语气。（3）与恐惧相关的词汇才是你的朋友，例如担心错过、害怕灾难的发生、对犯罪的恐惧等。（4）读者都喜欢逐条罗列事实的文章风格……（5）不要在标题中泄露所有的信息。"
  summary: |
    Upworthy总结的标题写法：描述清晰、对话语气、善用恐惧相关词汇、罗列体（"10种……的最佳方法"）、不泄露全部信息、不带强烈个人意见、无性别暗示、不过于复杂、不玩双关、不令人不快。配合A/B测试流程使用。
  tags: [copywriting, headline, media]
- id: fc15
  title: 团队"独特元素"观察法
  type: framework
  source_chapter: 第五章
  source_quote: |
    "这就是为什么我会对每个团队成员的身体语言予以特别的关注。这些人是真的喜欢在一起吗？他们看起来真诚吗？或者他们在一起工作只是为了钱吗？这个团队的动力是什么？"
  summary: |
    评估团队情感纽带的观察框架：看成员身体语言与互动是否真诚，带团队外出散步或参加团队活动（极限飞碟、彩弹对抗、峡谷漂流）观察互助与沟通。依据是伯克利研究：运动队队友间友好身体接触次数与比赛成绩直接相关。用于识别无法从财报上看到的"赢的团队"。
  tags: [team, culture, investing]
- id: fc16
  title: 投资人尽调交叉面谈法
  type: framework
  source_chapter: 第五章
  source_quote: |
    "他们会提出与你的团队中最重要成员单独面谈。通常他们会向你的管理团队中的每一个成员提出相同的问题，然后对会谈的笔记进行比较，以确保所有他们听到的故事在逻辑上都是一致的。"
  summary: |
    投资人发现企业隐患的方法：对管理团队每位成员单独提出相同问题，比较会谈笔记以检验故事是否逻辑一致。对应地，创业公司应提前让全员口径一致，避免因沟通失误让投资人起疑。反向可迁移为管理上的信息一致性检查。
  tags: [due-diligence, investing, consistency]
- id: fc17
  title: 投资人深挖创始人的提问清单
  type: framework
  source_chapter: 第五章
  source_quote: |
    "我想要知道，这个创业者是否提出过原创的想法……他又是如何说服他的同事并管理他的团队的？在推进并实现这些想法的过程中他曾经遇到过什么障碍，他是如何克服这些障碍的？他所做的某个决定是否曾经导致了失败？他从这些挫折中学到了什么？"
  summary: |
    评估CEO的深挖式提问：是否提出过原创想法、如何说服同事与管理团队、推进中遇到的障碍及克服方式、是否有导致失败的决定及教训。另外追问CEO如何认识共同创始人、如何说服员工放弃六位数薪水选择股权。目的在于检验真实领导力而非简历光鲜度。
  tags: [ceo, evaluation, investing]
- id: fc18
  title: 锁定客户的判定标准
  type: framework
  source_chapter: 第五章
  source_quote: |
    "锁定客户的一个常见判定标准是你是否能让客户把他们的时间投资在你的产品或服务上。对于软件产品，用户通常会首先花时间学习如何使用它，然后再对其进行定制，接着就是让这款软件与他们的工作流程和生活成为一体。"
  summary: |
    判断一家公司是否具备客户锁定能力：看客户是否把时间与资源投入产品（学习、定制、上传内容、装插件、集成工作流）。投入越多，转换成本越高，离开越痛苦。社交网络、WordPress、Hubspot、SAP等均符合。高锁定带来高利润率与长期增长。
  tags: [lock-in, switching-cost, moat]
- id: fc19
  title: 游击营销15个战术原型
  type: framework
  source_chapter: 第四章
  source_quote: |
    "最好的游击营销活动并不一定需要花很多钱，相反，以上所有的案例都是利用了某些能够引起人们共鸣的想法。它们激起了人们的情感反应，创造出了一种对话的氛围，并鼓励人们进行分享。"
  summary: |
    15个战术原型：失眠聊天机器人、会场游戏引流、基因检测+免费旅行、猎奇产品视频（搅拌机）、报纸包装证明新鲜度、AI创意总监、体温扫描广告牌、广告牌变司机休息站、免费中转停留、罚单英雄推广App、制造悬念现场（金刚脚印）、给地标穿内裤、CEO公开社保号、巧克力蚱蜢邮寄、冰桶挑战式全民参与。共性：花小钱、激发情感、制造对话、鼓励分享。
  tags: [guerrilla-marketing, cases, low-budget]
- id: fc20
  title: 价值观品牌塑造框架
  type: framework
  source_chapter: 第四章
  source_quote: |
    "这已经和产品无关，这里所涉及的实际上是你和这些产品打交道时所产生的感觉，它们正在把普通的消费品转变成一种对生活方式的选择。你在购买这些产品时所做的决定定义了你是谁以及你关心的是什么。"
  summary: |
    把普通消费品升维为生活方式选择的品牌框架：赋予品牌一种价值观或使命（Soma的清洁饮水人权、Bouqs的可持续花艺与快乐承诺、Ritual的成分透明与女性专属、bkr的美学使命），让购买行为成为消费者自我表达。策略要点是"与客户的内心而不是头脑对话"。
  tags: [branding, values, positioning]
- id: fc21
  title: 与媒体建立关系的操作框架
  type: framework
  source_chapter: 第四章
  source_quote: |
    "首先你必须站在新闻记者的立场来看问题，他们在为哪种刊物撰写稿件？他们的读者希望能看到哪些类型的故事？为什么你的故事对他们很重要？对于不同的出版物你需要兜售完全不同的故事。"
  summary: |
    低成本公关框架：设计吸引眼球的标题（研究Buzzfeed/Upworthy）→通过活动和会议私下结识记者→按不同出版物量身定制故事→主动提供有用数据成为记者的"御用名单"成员→把团队定位成某领域专家→写客座文章建立粉丝群。核心是先理解记者心理再开口。
  tags: [pr, media, networking]
- id: fc22
  title: 增长黑客五类实验案例集
  type: framework
  source_chapter: 第四章
  source_quote: |
    "增长黑客的实验过程首先会对用户如何使用产品进行仔细的分析，然后会尝试采用不同的创造性方法来提高产品度量指标的表现。在每一个这样的实验完成后，你应该马上进行相关的调整，然后再重新设计实验，直到获得最优的结果。"
  summary: |
    按漏斗五阶段对应的经典实验：获客（爱彼迎借Craigslist导流）、激活（推特让新用户关注至少5个账户）、收入（Ticketmaster购票倒计时）、推介（Dropbox推荐送存储空间）、留存（YouTube连续播放）。方法论：分析用户行为→创造性改进指标→调整→重做实验直到最优。
  tags: [growth-hacking, experiment, cases]
```

### 2. principles

```yaml
- id: pr01
  title: 先验证商业模式，后拿大钱
  type: principle
  source_chapter: 第四章
  source_quote: |
    "那数百万美元的投资最好是在你已经验证了你的商业模式后再到你的账上，而不是在这之前，因为过早地获得融资可能会置你于死地。"
  summary: |
    融资时机的操作性原则：在盈利模式获得验证之前不要烧钱加速。验证了模式，投资人会排队上门；模式被否决则必须转向。风险投资擅长为已验证的模式做扩张，不擅长修正被否决的模式。
  tags: [fundraising, validation, timing]
- id: pr02
  title: 缺钱是创造力之源
  type: principle
  source_chapter: 第四章
  source_quote: |
    "缺钱会让一家创业公司自律，因为你不可能一路不断地烧钱，所以你必须表现出某种让人惊叹的创造力以及足够的智慧才有可能获得突破。"
  summary: |
    资金匮乏迫使公司自律、聚焦小而廉价的实验、避免奢华支出。Little Passports创始人直言"对风险投资的依赖就像依赖毒品"。把缺钱视为纪律约束而非纯粹劣势。
  tags: [bootstrapping, discipline, creativity]
- id: pr03
  title: 时间花在客户身上而不是投资人办公室
  type: principle
  source_chapter: 第四章
  source_quote: |
    "与其花好几个月的时间去融资，还不如花时间去接触你的客户。尽量把各种费用降到最低，并且投入尽可能多的时间去进行各种实验以验证或者否决你的商业设想。"
  summary: |
    早期创始人的时间分配原则：客户接触与实验的优先级高于融资路演。融资困难且耗时，尤其只有一个创意时；天使融资可以接受，但大额风投需要企业"能飞起来"的证据。
  tags: [customer, prioritization, fundraising]
- id: pr04
  title: 风险投资人并不喜欢冒险
  type: principle
  source_chapter: 第四章
  source_quote: |
    "绝大多数的风险投资人都不喜欢冒险，而且他们也不想承担任何风险。他们会对你说，他们会亲力亲为并且很乐意为你增添价值，但你绝不要指望他们会帮你想出任何解决方案。"
  summary: |
    对风投的清醒认知：他们只为"下一个真正重要的项目"下注，不帮你想解决方案，重活累活要自己扛；投资组合中绝大多数公司回报很低甚至为零。创业者不应把融资等同于成功。
  tags: [vc, expectation, fundraising]
- id: pr05
  title: 选择不需要大笔前期投资的业务
  type: principle
  source_chapter: 第四章
  source_quote: |
    "好的企业往往只需要你花费时间和积蓄在上面，就能逐渐成长起来并开始赢利。……合适的创意通常就是那些你只需用你的银行账户中的积蓄就可以开发的创意。你靠自己的钱能走得越远，你的处境也就会越好。"
  summary: |
    启动资金问题的两个答案：找工作存钱，或选择低前期投入的业务。微软、戴尔、Facebook都从宿舍起步。需要数百万启动资金的梦幻项目应搁置到有一两次成功经验之后再做。
  tags: [bootstrapping, idea-selection]
- id: pr06
  title: 用业余时间养活创业公司
  type: principle
  source_chapter: 第四章
  source_quote: |
    "很多创业公司在开始的时候也只不过是一个副业项目，而且有些项目在真正崭露头角前会有好几年一直维持这样的状态。"
  summary: |
    没有启动资金时的可行路径：兼职/全职工作养公司（奈特、FUBU的约翰、GitHub）、与雇主协商过渡期（胡佛）、请长假思考（贝尼奥夫）、甚至把雇主变成合作伙伴与出资人（多尔西与Odeo）。
  tags: [bootstrapping, side-project]
- id: pr07
  title: 成为新闻记者的数据源与领域专家
  type: principle
  source_chapter: 第四章
  source_quote: |
    "很多新闻记者的手上通常都会有一份人员名单，每当他们在文章中需要相关的数据并加以引用时，他们就会打电话给这些人。你应该努力成为这张名单中的一员。"
  summary: |
    低成本获取媒体报道的原则：先给记者提供有用的数据与事实，把自己的团队定位成某个特定领域的专家，让记者写相关题材时第一个想到你。帮助了记者，记者也会帮助你。
  tags: [pr, media, positioning]
- id: pr08
  title: 好故事价值抵得上1000次广告
  type: principle
  source_chapter: 第四章
  source_quote: |
    "我总喜欢这样对人说，一个好故事的价值抵得上1 000次广告。通过你自己的能力弄清楚什么样的故事会在网上火起来……这要比雇用一个6位数薪资的市场营销主管和昂贵的公关公司更能吸引那些新闻记者的眼球。"
  summary: |
    对预算紧张的创业公司，弄清什么故事会在网上火起来、如何利用它，是比雇营销高管和公关公司更聪明的投资。故事必须匹配品牌、强化核心信息、引起受众共鸣，三者缺一就无法激活客户。
  tags: [storytelling, marketing, low-budget]
- id: pr09
  title: 视频制作是入场券而非选项
  type: principle
  source_chapter: 第四章
  source_quote: |
    "如果你仔细地研究一下Indiegogo和Kickstarter这两个著名众筹网站的数据，你就会发现，在筹集到的资金数额与视频的质量之间存在直接的关联。对视频制作进行投资已经不再是一个选项，而是一张入场券。"
  summary: |
    视频是抓住客户、投资人、媒体想象力的最廉价方式，且具备病毒式传播能力。投资人看融资材料前会先看视频；业余观感的视频会直接导致否决。必须请专业人士制作。
  tags: [video, fundraising, marketing]
- id: pr10
  title: 游击营销唯一的规则是与众不同
  type: principle
  source_chapter: 第四章
  source_quote: |
    "游击营销的关键在于如何有效地利用资源，如何用某些替代的方式来建立你的品牌并获得客户。……这里唯一的规则就是你必须与众不同，你必须脱颖而出。"
  summary: |
    用独创性弥补资金缺口，靠引起共鸣的想法（而非预算或名人背书）让活动依靠自身力量传播。避免复制他人已做过的事——创意是所有成功活动的最基本要素。
  tags: [guerrilla-marketing, creativity]
- id: pr11
  title: 内容营销要填补空白、追求实用
  type: principle
  source_chapter: 第四章
  source_quote: |
    "你需要去发现在内容分类中还缺少些什么，然后用你的内容去填补其中的空白。……在这里，你的目标是实用而不是新奇。"
  summary: |
    集客营销的操作原则：研究竞争对手与高流量内容，找出信息缺口，写出增添了价值的新版本；内容必须对客户真正有用（教育或娱乐），个性化与针对性越强效果越好；清单体、可视化、简洁结构更易传播。
  tags: [inbound-marketing, content, seo]
- id: pr12
  title: 品牌要代表价值观，与内心对话
  type: principle
  source_chapter: 第四章
  source_quote: |
    "所以，如果你打算在当下这种体验式的商业时代中参与竞争，你就需要把你的游戏提升到一个全新的层次，去与你的客户的内心而不是与他们的头脑对话。"
  summary: |
    即使与竞品出自同一工厂，也可以靠价值观、使命与生活方式表达取胜（Soma、Bouqs、Ritual、bkr）。购买决定定义了消费者是谁、关心什么——营销的落点是情感与身份认同。
  tags: [branding, values, consumer]
- id: pr13
  title: 撬开市场只有两条路：好出数量级或截然不同
  type: principle
  source_chapter: 第五章
  source_quote: |
    "这两种方法是，要么你有比竞争对手好出很多个数量级的产品，要么你和其他人截然不同。如果这家创业公司没有按照这两者之一去做，它将永远无法取得成功。"
  summary: |
    市场存在巨大惯性，客户不愿改变习惯；让客户放弃现有产品的办法要么是价值高出数量级（iPhone、谷歌、Skype的免费长途），要么是提供别处无法获取的价值（Slack瞄准企业协作、Affirm的按月分期）。二者皆无则难以撬开品类。
  tags: [differentiation, product, strategy]
- id: pr14
  title: 目标必须是市场第一，否则退出
  type: principle
  source_chapter: 第五章
  source_quote: |
    "作为一个创业者，如果你的目标仅仅是成为市场上排名第三的企业，那么你还不如现在就放弃。你期望成为第三，如果你幸运的话，你也许会排在第七、第八或者第九的位置。"
  summary: |
    赢家通吃的世界里，可扩展业务的第一名获得远超对手的客户数量、品牌认知与网络效应；买折价后来者并不划算，领头羊会越跑越快。若不相信自己能做第一，就换一个真正能赢的赛道。
  tags: [market-leadership, winner-takes-all, strategy]
- id: pr15
  title: 尽早搭上趋势并成为社区核心
  type: principle
  source_chapter: 第五章
  source_quote: |
    "没有什么比你在一波浪潮刚开始的时候就乘上去，然后被这波浪潮推动着一路冲向成功的彼岸更酷的事情了。……聪明的创始人会把完全掌控整个趋势当作自己的使命。"
  summary: |
    顺应技术或消费趋势（AI、区块链、健康食品等）如同安装喷气引擎；早期介入者能成为事实上的社区核心与市场领跑者，发起活动、办会、建平台、引导趋势方向，后来者则被看成抄袭者，并获得大量免费媒体曝光。
  tags: [trend, community, timing]
- id: pr16
  title: 不要不加权衡地照搬商业模式
  type: principle
  source_chapter: 第五章
  source_quote: |
    "这就是为什么我要提醒创业者，不要简单地选择某一种商业模式，然后不加权衡地直接采用该模式来运营自己的公司。……你需要对市场以及形成该商业模式的所有因素进行深入的分析。"
  summary: |
    "我们就是X行业的瓦尔比派克"式叙事容易拿到融资，但每个品类有独有市场规则：缺失一个要素就会让整个模式崩塌。照搬前必须逐项分析原模式成立的要素（参考优步8要素清单）。
  tags: [business-model, imitation, analysis]
- id: pr17
  title: 优先选择可持续收入模式
  type: principle
  source_chapter: 第五章
  source_quote: |
    "独角兽猎人喜欢专注于那些拥有一个强大的可持续收入模式的创业公司。他们并不在乎你从事的是什么业务，你的业务可以是软件、硬件、食品、医药、交通，或者任何其他的行业。"
  summary: |
    一次性售卖对创业公司是次优模式：获客后客户不再付钱，且克隆品会快速以低价压市。订阅、易耗品、平台等模式能深度变现、可预测、可扩张。投资人在乎的不是行业，而是能否深度变现并赚取可观利润。
  tags: [recurring-revenue, business-model, monetization]
- id: pr18
  title: 专利策略：先验证模式，后做专利
  type: principle
  source_chapter: 第五章
  source_quote: |
    "我的建议是，没有新的核心技术且依赖自有资金的创业公司可以首先专注于验证并构建自己的商业模式，专利申请可以等到将来再说。"
  summary: |
    大多数早期初创的专利毫无价值：申请贵、生效慢、诉讼贵，公司破产时专利只会被贱卖。只有半导体、制药、生物科技等资本密集核心技术才值得早期投入；找到产品市场匹配并准备扩张后，再把专利纳入长期知识产权策略。
  tags: [patent, ip-strategy, prioritization]
- id: pr19
  title: 不要为融资硬套热门技术
  type: principle
  source_chapter: 第五章
  source_quote: |
    "除非去中心化的区块链在某些特定的任务中有更好的表现，或者可以让某种全新类型的服务成为可能，否则，采用这种新技术完全没有意义。"
  summary: |
    用流行语给企业做"美容"或把热门技术硬塞进不适用的商业模式，既不道德又徒劳。选择技术的唯一理由应是它最佳地满足客户需求，而非吸引融资的捷径。
  tags: [technology, hype, integrity]
- id: pr20
  title: 早期设计创新重于技术创新
  type: principle
  source_chapter: 第五章
  source_quote: |
    "在创业早期，设计创新往往比技术创新更重要。为什么会这样呢？这是因为开发一种新的核心技术往往需要花费大量的时间和金钱。……所以设计创新往往会成为全世界大多数成功的创业公司的核心。"
  summary: |
    多数创业公司没时间没金钱开发核心技术，必须尽快进市场；Dropbox、Facebook、Pinterest、Spotify等靠设计创新重新定义品类。设计不止是外观，还涉及对使用者心理与情感需求的理解。
  tags: [design, innovation, product]
- id: pr21
  title: 雇一个顶尖设计师是最佳投资之一
  type: principle
  source_chapter: 第五章
  source_quote: |
    "作为一家创业公司的创始人，雇用一个顶尖的设计师是你能做的最佳投资之一。如果你的公司没有很强的设计基因，现在是时候去外面找一个好的设计师了。"
  summary: |
    设计是独角兽成败的核心考量之一：从产品包装到网站、App、视频甚至名片都是产品的一部分。卓越产品与客户建立情感联系，人们使用时感到愉悦甚至上瘾。
  tags: [design, hiring, product]
- id: pr22
  title: 用软件连接硬件（特洛伊木马原则）
  type: principle
  source_chapter: 第五章
  source_quote: |
    "我认为硬件就像是特洛伊木马，如果它能够成功地说服客户把一款产品带进自己的家门，并且这款产品的内置软件还能够悄悄地接管客户的很多日常应用，这样的软硬件组合就必定能够赢得投资人的青睐。"
  summary: |
    单凭硬件难以锁定客户、无法变现和获得反馈；最佳方法是用软件把硬件和互联网连接起来。纯硬件公司利润易被抄袭者侵蚀，软硬件结合才能建立持续客户关系与扩张模式（工业物联网比消费物联网更有前景）。
  tags: [hardware, software, iot]
- id: pr23
  title: 个人品质重于名校与头衔
  type: principle
  source_chapter: 第五章
  source_quote: |
    "在这里我想说的是，只有个人的品质才是让一个人最终获得成功的最重要的因素。"
  summary: |
    投资人用名校和副总监头衔做筛选会武断过滤掉叛逆者、大器晚成者。数据（全国经济研究局）显示名校生与同分数段其他大学毕业生终生收入几乎无差别；聪明的投资人会深挖简历背后的决策类型与承担的责任，宁可选初级项目经理而非副总裁。
  tags: [hiring, evaluation, leadership]
- id: pr24
  title: 团队是CEO领导力的第一项测试
  type: principle
  source_chapter: 第五章
  source_quote: |
    "这就是为什么团队应该是对于CEO领导能力的第一项测试，如果一个CEO能够仅凭言语和公司的股权组建起一个成功的团队，他就拥有了实现目标的神奇魔力。"
  summary: |
    没有人能只靠自己建立独角兽；CEO是让所有人行动起来的催化剂。杰出领导者是人才磁铁，员工愿为其承受非理性风险。若CEO从一开始就组不起顶尖团队，公司前景通常只会越来越糟。
  tags: [ceo, team, leadership]
- id: pr25
  title: 尽调前尽早披露所有实质性信息
  type: principle
  source_chapter: 第五章
  source_quote: |
    "在你签署投资意向书之前，你应该披露所有实质性的东西，不要让人感到你有什么不可告人的秘密。……在融资刚刚开始的时候……此时披露负面的事情产生的影响，要比投资人即将对这笔交易做出承诺时再披露所产生的影响小很多。"
  summary: |
    透明原则：隐瞒等于说谎，所有细节最终都会浮出水面，越早披露代价越小。配套做法是在云文件夹中保存所有协议副本（股权结构表、章程、专利、商标、雇用协议），投资人索要时直接发送链接。
  tags: [due-diligence, transparency, fundraising]
- id: pr26
  title: 解决创始人自己碰到的真问题
  type: principle
  source_chapter: 第四章
  source_quote: |
    "上述企业都有一个共同点，那就是它们都解决了一个真正的问题，而且常常是它们的创始人自己碰到的问题。这就是为什么它们能够在最艰难的处境中存活下来，而且客户都很愿意为它们的产品付费。"
  summary: |
    自力更生公司（MailChimp、Shopify、ShutterStock等）的共同基因：解决真实且紧迫的需求，往往源自身边问题。犹豫不决时，"创造一件真正有价值的东西永远是答案；如果你能解决一项紧迫的需求，金钱自然会来"。
  tags: [problem, product, bootstrapping]
- id: pr27
  title: 产品定价宁高勿低（戴森教训）
  type: principle
  source_chapter: 第五章
  source_quote: |
    "不管你的产品多么优秀，市场也很重要。实际上并没有那么多的人想要购买手推车……戴森承认他应该为他的创新产品定一个更高的价格，而不是在价格上与其他的产品竞争，只不过在当时他不知道该怎么做。"
  summary: |
    再优秀的产品也受市场与定价约束：小品类+低定价=赚不到钱。创新产品应定更高价格而不是陷入价格竞争；同时警惕引入与愿景不合的外部投资人。
  tags: [pricing, market, lesson]
- id: pr28
  title: 疲惫时跑得更快：长跑者心态
  type: principle
  source_chapter: 第五章
  source_quote: |
    "戴森把他的成功归因于他有一种长跑运动员的心态，他坚定地相信，当你开始感到疲倦的时候，你就应该跑得更快，因为在这个时候其他人也都累了。如果你想赢，你就不能在这个时候放弃。"
  summary: |
    临界点处多数人会停下，再坚持一段时间就能获得突破。戴森40岁负债累累时才做出第一台吸尘器，5年做了5000多个原型；最好的产品终将在长期竞争中胜出。
  tags: [persistence, mindset, dyson]
```

### 3. cases

```yaml
- id: ca01
  title: Little Passports：被75位投资人拒绝后自力更生
  type: case
  source_chapter: 第四章
  source_quote: |
    "创始人埃米·诺曼和斯特拉·马先后向75个投资人推介了自己的创业公司，但被连续拒绝了75次。……8年后，Little Passports每年已经有了3 000万美元的销售收入……'你对风险投资的依赖，就像依赖毒品一样。'"
  summary: |
    两母亲创业者2009年以每月10.95美元订阅制邮寄地理主题活动包，仅想融50万美元被拒75次。被迫节俭运营、聚焦小型廉价实验，后花3万美元投Facebook定向广告见效，8年后做到3000万美元年收入。结论：没拿到风投反而迫使严格财务纪律，成就了公司。
  tags: [bootstrapping, subscription, fundraising-refusal]
- id: ca02
  title: GitHub：四年不融资的副业项目
  type: case
  source_chapter: 第四章
  source_quote: |
    "GitHub的创始人在东拼西凑了数百美元后创立了他们的公司，在接下来的4年时间里，他们开发了在线版本的控制平台，并没有进行过任何形式的融资。……接着微软开始介入，并且以75亿美元的价格收购了他们的公司。"
  summary: |
    创始人靠咨询工作和全职薪水支付账单，4年无融资开发产品，盈利后再拿风投扩张，最终被微软以75亿美元收购。证明副业起步+自筹资金可以走到顶级退出。
  tags: [bootstrapping, github, exit]
- id: ca03
  title: FUBU：白天端盘子晚上做品牌
  type: case
  source_chapter: 第四章
  source_quote: |
    "我在运营这家公司的同时还在红龙虾餐厅当了5年的服务员。……最开始我每周有40个小时会在红龙虾餐厅，有6个小时在FUBU。之后……30个小时在红龙虾餐厅，20个小时在FUBU。"
  summary: |
    戴蒙德·约翰在红龙虾餐厅当5年服务员养活服装品牌FUBU，随收入增长逐步把时间转移到公司，最终做成价值60亿美元的时尚品牌。业余时间创业可行性的典型样本。
  tags: [side-project, fubu, bootstrapping]
- id: ca04
  title: 贝尼奥夫休假想出Salesforce
  type: case
  source_chapter: 第四章
  source_quote: |
    "当时他已经为甲骨文公司工作了10年，并且感到有些疲惫，所以他获准休假6个月。在这期间，他周游世界，同时思考软件行业在未来几年将会如何发生改变，这激发了他关于云计算和Salesforce的想法。"
  summary: |
    马克·贝尼奥夫通过6个月长假构思云计算与Salesforce，返回后向甲骨文CEO埃里森分享概念，获得200万美元启动资金。展示了"休假创业"与"把雇主变成出资人"两种路径。
  tags: [salesforce, bootstrapping, sabbatical]
- id: ca05
  title: Upworthy：数据驱动的标题工厂
  type: case
  source_chapter: 第四章
  source_quote: |
    "让人感到惊讶的是，当面向读者进行测试时，新闻记者最喜欢的那些标题往往表现得不尽人意。依靠直觉的日子已经过去了……数据分析才是如今的专业人士使用的方法。例如，Upworthy就会对它的所有标题进行A/B测试。"
  summary: |
    Upworthy对每篇文章批量制作25个标题、选出4个候选、在社交网络测点击、选数据最优者。结论：直觉选出的标题往往表现不佳，标题生产必须数据化。其"清晰描述+对话语气+恐惧词汇+罗列体"的10条建议成为标题方法论。
  tags: [ab-testing, headline, upworthy]
- id: ca06
  title: Casper：失眠聊天机器人Insomnobot3000
  type: case
  source_chapter: 第四章
  source_quote: |
    "Casper希望客户不光把它看成一家床垫公司，所以它推出了一个叫作Insomnobot3000的聊天机器人。这个机器人是专门为失眠症患者设计的。每当客户无法入睡时，他们都可以和Casper的人工智能聊天。"
  summary: |
    床垫品牌Casper用专门服务失眠人群的AI聊天机器人制造话题与品牌差异化，是游击营销中"用创意替代预算"的代表案例，让品牌超越产品品类本身。
  tags: [guerrilla-marketing, casper, chatbot]
- id: ca07
  title: Foursquare：SXSW操场游戏
  type: case
  source_chapter: 第四章
  source_quote: |
    "就在会议大厅的前面，Foursquare组织了一场四方格游戏，这是一种很像小孩在校园操场上玩的游戏。游戏只用了Foursquare的一些粉笔和两只皮球，却将平均签到人数从25万增加到了35万。"
  summary: |
    在SXSW大会门口用粉笔和皮球组织四方格游戏，以近乎零成本把大会平均签到人数从25万提升到35万。证明游击营销的核心是创意与场景选择而非预算。
  tags: [guerrilla-marketing, foursquare, event]
- id: ca08
  title: Blendtec：《能把它们搅拌在一起吗？》
  type: case
  source_chapter: 第四章
  source_quote: |
    "他提出为什么不在YouTube上拍一系列名为《能把它们搅拌在一起吗？》的视频呢？……把一些乱七八糟的东西，比如耙子柄、可乐罐、巨无霸套餐或者iPhone等一起塞进搅拌机……在它达到了数百万的浏览量之后，该品牌的搅拌机自然地成了市场营销界的传奇。"
  summary: |
    低关注度产品（搅拌机）通过猎奇系列视频获得数百万浏览量，品牌跻身营销传奇。案例要点：为平庸产品设计一个让人"我就是想知道"的内容载体。
  tags: [video, viral, blendtec]
- id: ca09
  title: Momondo×AncestryDNA：基因寻祖营销
  type: case
  source_chapter: 第四章
  source_quote: |
    "如果它通过分析你的基因向你提供寻找你的祖先的免费服务呢？如果你能赢得一次前往你的原籍地的免费之旅呢？丹麦旅行平台Momondo与基因检测公司AncestryDNA合作运营了这场活动，结果不但在全世界引起了轰动，还广受大众的欢迎。"
  summary: |
    机票比价平台用基因检测+免费寻祖之旅制造情感冲击，全球轰动。要点：把品牌与用户的身份认同、情感故事绑定，形成自发传播。
  tags: [guerrilla-marketing, momondo, emotional]
- id: ca10
  title: 冰桶挑战：250万个标签视频
  type: case
  source_chapter: 第四章
  source_quote: |
    "这项活动的概念很简单：通过拍摄某个人将一大桶冰水倒在自己的头上来唤起人们对这种疾病的认识。最终有超过250万个贴有标签的视频在Facebook上传播，这也推动了人们针对这种疾病的捐赠金额急剧地增加。"
  summary: |
    参与式挑战机制+社交平台标签传播，超250万个视频形成全民连锁，捐款激增。是"允许受众参与并鼓励分享"这条游击营销规则的极致样本。
  tags: [viral, participation, als]
- id: ca11
  title: Betabrand：粉丝社区驱动的游击品牌
  type: case
  source_chapter: 第四章
  source_quote: |
    "林德兰德的品牌与他一手建立起来的社区有着千丝万缕的联系，他一直在询问社区成员对于产品的反馈……如果有某个视频无法通过他的猫咪视频测试，他就不会发布这个视频。……帮他获得了价值数百万美元的免费媒体报道以及在网上的病毒式传播。"
  summary: |
    Betabrand用礼服运动裤、迪斯科连帽衫等话题性产品做博客诱饵，以粉丝社区提供创意与模特，用"猫咪视频测试"筛选内容，没有大预算却获得数百万美元价值的免费媒体报道。
  tags: [community, betabrand, pr]
- id: ca12
  title: 反人类卡牌：黑色星期五"反销售"
  type: case
  source_chapter: 第四章
  source_quote: |
    "在黑色星期五，他们进行了一次'反销售'的活动，他们声称：'仅在今天！反人类卡牌的售价会上涨5美元。不要错过！'很莫名其妙的是，卡牌的销量却呈直线上升，而不是下降。"
  summary: |
    Cards Against Humanity第一年销售额1200万美元，靠一系列荒谬噱头（涨价反销售、挖"假日深洞"、买边境空地）维持病毒式传播。启示：统一的、毫无敬意的幽默人格本身就是品牌资产。
  tags: [viral, cards-against-humanity, stunt]
- id: ca13
  title: 本特利大学：一篇SEO文章招生的MBA
  type: case
  source_chapter: 第四章
  source_quote: |
    "这所大学想为它的MBA项目招生，所以相关人员撰写了一篇内容极其丰富的文章叫作《在MBA的面试中你会被问到的12个问题》。在谷歌的关键词短语'MBA面试问题'的搜索结果中，这篇文章被排在了第一位，并且从那以后，每个月都有成千上万的访问量。"
  summary: |
    针对目标客户搜索意图生产"12个MBA面试问题"长文，占据关键词搜索结果首位，每月带来成千上万访问量。集客营销"回答客户最紧迫问题"的教科书案例。
  tags: [seo, inbound-marketing, bentley]
- id: ca14
  title: 美元剃须俱乐部：4500美元视频撬出10亿美元品牌
  type: case
  source_chapter: 第四章
  source_quote: |
    "迈克尔·迪宾只花了4 500美元就制作了他的第一个视频，然后他把这个视频放在了YouTube上。……'是的，我们的刀片太他妈的好用了。'……在获得了超过2 500万次的浏览量之后，这个视频不但把他的公司推到了大众的面前，而且还让他的品牌在千禧一代的心目中牢牢地扎下了根。"
  summary: |
    4500美元的不加修饰、诙谐幽默视频获2500万+浏览量，配合订购模式低价刀片（对标吉列涨价），最终以10亿美元卖给联合利华。同时是视频营销与"瓦尔比派克模式成功者"的双重案例。
  tags: [video, dollar-shave-club, subscription]
- id: ca15
  title: 西捷航空：行李转盘上的圣诞奇迹
  type: case
  source_chapter: 第四章
  source_quote: |
    "当飞机抵达目的地，所有人都去取行李的时候，在行李转盘上出现了一排用五颜六色的圣诞纸包装的礼品。乘客们惊喜地收到了仅仅在几个小时前他们希望获得的礼物。这个非常简单的视频在Youtube上有超过4 000万次的浏览量。"
  summary: |
    M工作室为西捷航空制作"问乘客圣诞愿望→送达实物"的视频，4000万+浏览量让品牌腾飞。证明一段投注真实情感的视频比广告投放更能建立品牌。
  tags: [video, westjet, emotional]
- id: ca16
  title: Young & Reckless：故事即品牌
  type: case
  source_chapter: 第四章
  source_quote: |
    "他曾支付15万美元请一个名人来穿他的服装，但最后的结果是浪费了很大一笔钱。'这样做你没有什么故事可讲。'……普法夫最后在Facebook、Instagram以及YouTube上收获了350万粉丝……它的营业收入已经达到了3 000万美元。"
  summary: |
    滑板手出身的普法夫用"年轻和鲁莽"的生活方式故事（从六楼跳窗、瘫痪车手达赖厄斯的抗争视频）激活受众，做到3000万美元营收、3000+门店分销。反面教训：没有故事的名人代言和商标棒球衫都失败了。
  tags: [storytelling, young-and-reckless, brand]
- id: ca17
  title: 爱彼迎攻击Craigslist获客
  type: case
  source_chapter: 第四章
  source_quote: |
    "爱彼迎实际上是通过对Craigslist进行黑客攻击，从而将流量导向了它当初还没有真正成长起来的市场的。……这一策略尽管不是很道德，却为爱彼迎带来了它起步时所需要的大量关键用户。"
  summary: |
    增长黑客"客户获取"经典案例：用机器人刺探Craigslist用户并引导其跨站发布房源，借大平台流量冷启动。展示增长黑客不拘泥规则（甚至不道德）的一面，可作伦理边界讨论素材。
  tags: [growth-hacking, airbnb, acquisition]
- id: ca18
  title: 推特：新用户关注5人激活
  type: case
  source_chapter: 第四章
  source_quote: |
    "推特利用数据分析得出了一个结论，即如果在新用户完成注册的时候你没有给他安排任何关注对象，他就几乎不太可能会参与以后的互动，而那些从一开始就已经关注了不少于5个对象的新用户则有更大的可能性再次访问他们的网站。"
  summary: |
    增长黑客"客户激活"案例：数据发现新用户关注≥5个账户才可能留存，于是注册流程强制推荐热门账户。方法论：找到与留存相关的行为拐点并把它产品化。
  tags: [growth-hacking, activation, twitter]
- id: ca19
  title: Ticketmaster：购票倒计时
  type: case
  source_chapter: 第四章
  source_quote: |
    "这家公司发现，在用户购票时增加一个简单的倒计时功能，能极大地提高销售量。这个计时器让用户感到，如果他们不立刻做出决定买下门票，他们就很有可能错过这场表演。"
  summary: |
    增长黑客"收入增长"案例：一个倒计时组件利用损失厌恶（怕错过演出）极大提升售票转化。说明漏斗环节的小改动即可带来显著收入变化，不需要大预算。
  tags: [growth-hacking, revenue, ticketmaster]
- id: ca20
  title: Dropbox与YouTube：推介与留存实验
  type: case
  source_chapter: 第四章
  source_quote: |
    "云文件托管服务供应商Dropbox发现，如果他们给予成功推介朋友进行注册的用户额外的免费云存储空间，他们网站的热度就会增加。……YouTube通过实验发现，在其视频中增加连续播放的功能可以提高客户的忠诚度以及他们在网站上停留的时间。"
  summary: |
    增长黑客"产品推介"与"客户留存"案例：Dropbox用双向免费存储激励推荐；YouTube用自动连播拉长停留时长。两者都以产品机制（而非广告）驱动漏斗指标。
  tags: [growth-hacking, referral, retention]
- id: ca21
  title: 自力更生群像：MailChimp、Shopify、Braintree、SurveyMonkey、ShutterStock、Grammarly等
  type: case
  source_chapter: 第四章
  source_quote: |
    "今天，他的创业公司已经有接近5亿美元的营业收入和超过500名的员工。但最棒的是实现这一切他没有依靠任何来自风险投资公司的资金。……Shopify已经是一家市场规模达到了160亿美元的上市公司。"
  summary: |
    MailChimp靠设计咨询副业工具做到近5亿美元营收零风投；Shopify自筹6年后上市（160亿美元市值）；Braintree靠收入运营4年后被贝宝8亿美元收购；SurveyMonkey熬11年才融资；ShutterStock从个人3万张照片起步上市；Grammarly自力更生近十年后融1.1亿美元；AppLovin、Wistia、CoolMiniOrNot等也均低成本起步。共同点：解决创始人自己碰到的真实问题。
  tags: [bootstrapping, mailchimp, shopify]
- id: ca22
  title: Tuft and Needle：6000美元对抗数亿美元融资对手
  type: case
  source_chapter: 第四章
  source_quote: |
    "当这家非常活跃的创业公司进入在线床垫市场的时候，创始人的手上只有6 000美元的种子资金。尽管面临着像Casper这种已经筹集了数亿美元风险投资且体型庞大的捣蛋鬼的挑战，Tuft and Needle依然做得相当不错。……它还始终保持了盈利的状态。"
  summary: |
    以6000美元种子资金进入在线床垫市场，控制成本、守住盈亏底线，销售收入超1亿美元且持续盈利，与巨额融资但烧钱的对手形成对照。证明自力更生者可以与资本充裕者正面竞争。
  tags: [bootstrapping, profitability, tuft-and-needle]
- id: ca23
  title: Tough Mudder：预收注册费造赛道
  type: case
  source_chapter: 第四章
  source_quote: |
    "从7 000美元的种子资金开始，他把这家创业公司发展成一家营业收入超过1亿美元的企业。他的秘密是预先收取参加比赛的注册费，然后再用到手的钱来制作那些疯狂的障碍赛道。"
  summary: |
    威尔·迪安用7000美元起步，靠"先收报名费后建障碍"的负现金流模式做成营收超1亿美元的极限赛事公司。要点：客户预付费可以作为初创的免费融资渠道。
  tags: [cashflow, tough-mudder, bootstrapping]
- id: ca24
  title: RXBAR：1万美元起家的成分透明蛋白棒
  type: case
  source_chapter: 第五章
  source_quote: |
    "当时拉哈勒和他的合作伙伴贾里德·史密斯用他们手中仅有的1万美元创立了这家公司，并开始手工制作健康蛋白棒。……在一根标准的蛋白棒的外包装上，他们会用大号的粗体字印刷上其中包含的所有成分：'3个蛋白、6个杏仁、2个腰果、2颗大枣，没有任何其他添加剂。'"
  summary: |
    创始人听从父亲"先卖掉1000根蛋白棒再说"，用PowerPoint做包装、免费铺货本地咖啡店，搭上健康蛋白棒趋势，把手机号印在包装上收集反馈，最终被家乐氏以6亿美元收购。趋势+极简成分透明化是成功关键。
  tags: [trend, rxbar, transparency]
- id: ca25
  title: Snapchat：避开Facebook锋芒切入移动青少年
  type: case
  source_chapter: 第五章
  source_quote: |
    "Snapchat把它的重点放在了移动通信上。在2010年，Facebook在移动市场上还不是一个占主导地位的玩家……Snapchat把目光瞄准了青少年……另外，Snapchat有一个独有的功能，即它可以让某些信息在一段时间后自动消失。"
  summary: |
    在桌面社交已被Facebook垄断时，选择移动+青少年+阅后即焚的差异化定位，2017年上市首日股价涨44%、市值280亿美元。案例展示"与其更好、不如不同"与选对战场的重要性。
  tags: [differentiation, snapchat, positioning]
- id: ca26
  title: Slack：与个人即时通信错位竞争
  type: case
  source_chapter: 第五章
  source_quote: |
    "Slack当时使用的技术和其他的玩家并没有什么不同，但是它向客户提供了完全不同的价值。Slack从一开始就不是一款个人即时通信工具，它瞄准的是企业用户，并且从底层开始就被设计成一种业务协作的工具。"
  summary: |
    在Messenger、WhatsApp等主导的个人通信市场，Slack靠"商务协作工具"这一完全不同的核心价值存活并成为顶级独角兽，两年内零大型营销活动、无CMO，靠早期媒体接触与好文转发增长。是"截然不同"路径与媒体策略的双重案例。
  tags: [slack, differentiation, media]
- id: ca27
  title: Affirm：把贷款做成优雅的分期付款
  type: case
  source_chapter: 第五章
  source_quote: |
    "Affirm是如何撬开这个市场的呢？它向消费者提供了一种所有其他的竞争对手从来没有想到过的选项——一种非常简单而优雅的支付方式，即当你在线购物时，你可以选择按月分期付款。"
  summary: |
    支付市场看似饱和（维萨、万事达、贝宝），Affirm以"在线购物按月分期、利息内含于支付计划"这一全新选项切入，成长为健康独角兽。证明"与众不同"可在红海中开新价值维度。
  tags: [affirm, fintech, differentiation]
- id: ca28
  title: Skype：用免费长途击败垄断者
  type: case
  source_chapter: 第五章
  source_quote: |
    "它并不是VoIP技术的发明者……当时它提供的长途电话的通信质量要比那些传统的通信公司的差很多……那么Skype是如何获胜的呢？它通过提供免费长途电话服务赢得了最后的胜利。"
  summary: |
    Skype产品体验全面落后（质量差、需专用软件、要用电脑），但"免费越洋长途"对需要省话费的客户而言价值高出数量级，几乎没有遭遇竞争阻力。说明客户愿意为关键价值忍受劣势。
  tags: [skype, value-proposition, disruption]
- id: ca29
  title: 瓦尔比派克：颠覆陆逊梯卡垄断的眼镜直销
  type: case
  source_chapter: 第五章
  source_quote: |
    "眼镜市场一直被陆逊梯卡眼镜制造及销售跨国集团主导……这种近乎垄断的状态使得陆逊梯卡公司的产品能够获得相当高的溢价。瓦尔比派克眼镜公司在向客户提供同样时尚的产品的同时大幅降低了价格，此举颠覆了原来的市场。"
  summary: |
    低价直销眼镜打破垄断溢价，更低价格鼓励消费者每年换镜从而增加经常性收入。成功依赖品类特有条件（垄断溢价空间、高频复购）；照搬此模式的数百家抄袭者大多失败。
  tags: [warby-parker, d2c, disruption]
- id: ca30
  title: 客户锁定群像：WordPress、Hubspot、微软、SAP
  type: case
  source_chapter: 第五章
  source_quote: |
    "一旦客户选择了Wordpress.com，他们就会开始上传内容并建立自己的页面。……他们使用Wordpress.com上的插件越多，最后离开的难度也越大……微软用它的Windows操作系统做到了这一点；思爱普用它的企业资源规划以及商业服务来做到了这一点。"
  summary: |
    WordPress靠内容与插件生态锁定博主；Hubspot与企业工作流深度集成后迁移困难；Windows、SAP、甲骨文把软件嵌入业务流程与组织架构，解开捆绑的代价大于竞品好处，从而长期维持高利润率。锁定能力是独角兽的共同特征。
  tags: [lock-in, wordpress, hubspot]
- id: ca31
  title: 戴森：5127个原型与被踢出公司后的逆袭
  type: case
  source_chapter: 第五章
  source_quote: |
    "在制作了超过5 000个原型之后，他终于成功地做出一台功能齐全的旋风真空吸尘器。……这笔交易加上他在美国赢得的专利侵权诉讼，最终把戴森从破产中拯救了出来。……现在他的身价大约是60亿美元，拥有公司100%的股权。"
  summary: |
    戴森从设计平底船学全流程（设计、焊接、销售），球轮手推车因定价过低几乎不赚钱；做吸尘器时被外部投资人踢出公司，负债中做5000+原型，靠日本授权与美国专利诉讼起死回生，两年成为英国销量第一，后亲拍广告征服美国。启示：卓越设计+市场判断+长期坚持+保持股权。
  tags: [dyson, design, persistence]
- id: ca32
  title: 亚马逊Echo：从点歌盒到Alexa平台
  type: case
  source_chapter: 第五章
  source_quote: |
    "不过亚马逊的智能音箱Echo却成为一款真正获得突破的智能家居产品，它原本只是一款声控音乐点播盒，但现在它已经扩展成为一个被称作Alexa的家庭语音平台，并且还拥有了一个由应用和相关开发人员组成的完整的生态系统。"
  summary: |
    在Nest等消费物联网普遍失败背景下，Echo靠语音控制全网内容的真实重要价值突破，并扩展为有开发者生态的平台。是"硬件作为特洛伊木马+软件生态"的成功样本，反衬大多数物联网设备学习成本高、价值不足。
  tags: [echo, iot, platform]
- id: ca33
  title: WhatsApp：零专利卖出190亿美元
  type: case
  source_chapter: 第五章
  source_quote: |
    "当这家即时通信创业公司被Facebook以高达190亿美元收购的时候，所有人都震惊了……更让人惊讶的是，WhatsApp并没有给Facebook带来什么专利。……只有快速地增长才会有更高的估值，而WhatsApp的创始人从未将他们关注点从这一点上挪开。"
  summary: |
    WhatsApp把100%精力投入产品开发、完全不做专利保护，以190亿美元被收购，估值源于增长与市场地位而非知识产权。是"专利对多数初创无价值"论断的最有力证据。
  tags: [whatsapp, patent, growth]
- id: ca34
  title: Boxed：用真金白银买员工忠诚
  type: case
  source_chapter: 第五章
  source_quote: |
    "他承诺用他的个人资产为员工的孩子支付大学学费。他真的说到做到了……Boxed还实施了另一项政策，即员工可以为自己生活中的重大事件，比如婚礼，而申请报销相关的费用，报销的金额最高可达2万美元。"
  summary: |
    批量电商Boxed省去乒乓球桌和免费午餐，把资金投向员工子女大学学费（CEO个人出资）与婚礼报销（最高2万美元），4年后员工超200人而自愿离职者不到10人。展示"独特元素"（文化与忠诚）如何转化为留任与产品气质。
  tags: [culture, boxed, loyalty]
- id: ca35
  title: 西南航空与L.L.Bean：文化即护城河
  type: case
  source_chapter: 第五章
  source_quote: |
    "西南航空公司以其工作积极且幽默风趣的员工而闻名。这也是它的客户服务要比其他航空公司好很多的原因。……其员工流动率只有3%，这在零售行业是极其罕见的。更让人感到惊讶的是，L.L.Bean这个品牌已经有超过100年的历史。"
  summary: |
    西南航空靠员工热爱工作实现40多年最赚钱航空公司之一；L.L.Bean以培养员工赢得百年品牌与3%的员工流动率。说明"真正独特的元素"（文化）不止适用于初创公司，也是长期业绩的来源。
  tags: [culture, southwest, llbean]
- id: ca36
  title: Oculus VR与Nest：媒体宠儿的巨额退出
  type: case
  source_chapter: 第五章
  source_quote: |
    "媒体很喜欢报道有关创业者的新闻，这就是为什么每当一家创业公司在媒体上获得了大量的报道，投资人往往也会紧随其后。这样的事情就曾发生在Oculus VR和Nest这两家媒体的宠儿身上，它们在媒体的追捧下，最终以数十亿美元的价格被收购。"
  summary: |
    两家公司借助媒体大量正面曝光带动投资人跟进，最终以数十亿美元被收购。说明媒体关注度是初创公司脱颖而出的关键指标，媒体能以近乎零成本在几个月内建立起全国性品牌认知。
  tags: [media, oculus, nest]
- id: ca37
  title: 爱彼迎CEO切斯基：50美元出租自家沙发
  type: case
  source_chapter: 第五章
  source_quote: |
    "爱彼迎的CEO布赖恩·切斯基也非常痴迷于社区和关系的建立。在他创业的早期，他尤其注重亲自拜访在爱彼迎网站上注册的房东，并与他们建立紧密的关系。他甚至把他自己家里的沙发以每晚50美元的价格租了出去。"
  summary: |
    创始人亲自拜访房东、出租自家沙发，把社区关系作为公司的"独特元素"。创始人的投入姿态成为品牌与趋势之间的纽带，帮助公司在趋势早期成为社区核心。
  tags: [airbnb, community, founder]
```

### 4. counter_examples

```yaml
- id: ce01
  title: Fab.com：3.1亿美元融资烧穿公司
  type: counter_example
  source_chapter: 第四章
  source_quote: |
    "其中最出名的案例就是Fab.com，这是一款非常时髦的闪购应用，它拿到了高达3.1亿美元的投资。曾经有一段时间，它差不多每个月要烧掉1 400万美元，却没有想任何办法去留住客户。那些钱只起到了掩盖所有问题的作用。最终，它耗尽了所有的资金，然后被贱卖出去。"
  summary: |
    过早拿到太多投资的典型死亡样本：月烧1400万美元却不解决客户留存问题，资金只是掩盖深层问题，最终资金耗尽被贱卖。警告：盲目的烧钱加速等于"汽车冲下悬崖时还在踩油门"。
  tags: [overfunding, fab, failure]
- id: ce02
  title: 过早扩张：70%创业公司的通病
  type: counter_example
  source_chapter: 第四章
  source_quote: |
    "创业基因发布的报告中提到，过早扩张是创业公司业绩表现不佳的最为常见的原因。这份报告提供的数据表明，70%的创业公司至少在一个维度上过早地进行了扩张，包括招聘过快、产品产量过剩，以及在市场营销和客户获取上投入了过多的资金。"
  summary: |
    数据警告：70%的创业公司至少在一个维度过早扩张（招聘过快、产量过剩、营销获客投入过多）。在未弄清客户需求前匆忙扩张"等同于被判处了死刑"。过早融资正是过早扩张的主要诱因。
  tags: [premature-scaling, data, failure]
- id: ce03
  title: Lifelock CEO：公开社保号反被盗
  type: counter_example
  source_chapter: 第四章
  source_quote: |
    "Lifelock是一家从事身份信息防盗服务的供应商。这家公司的CEO为了向用户展示他对于Lifelock服务的信心，专门拍摄了一系列大胆的电视广告。在广告中他公布了自己真实的社会保险号码……但最后他自己成了身份信息失窃的受害者，以另一种方式付出了代价。"
  summary: |
    营销噱头走到极端的反讽案例：CEO公布真实社保号宣战身份窃贼以展示服务信心，获得大量免费宣传，但自己最终成为身份盗窃受害者。警示：大胆游击营销需要评估现实风险。
  tags: [lifelock, stunt, risk]
- id: ce04
  title: Young & Reckless：15万美元名人代言打水漂
  type: counter_example
  source_chapter: 第四章
  source_quote: |
    "他曾支付15万美元请一个名人来穿他的服装，但最后的结果是浪费了很大一笔钱。'这样做你没有什么故事可讲。'普法夫说道，'没有不顾一切的故事可以讲给我的受众听。这次推广不仅损失了一大笔钱，还损害了品牌。'"
  summary: |
    没有故事支撑的名人代言既烧钱又损害品牌；同样的钱花在"从六楼跳窗""瘫痪车手抗争"等真实故事上则销量飙升。教训：代言与推广必须嵌入品牌叙事。
  tags: [celebrity, storytelling, waste]
- id: ce05
  title: Tillys棒球衫：没有故事的贴牌
  type: counter_example
  source_chapter: 第四章
  source_quote: |
    "当Tillys表示要出售他们的棒球衫的时候，普法夫又一次搞砸了。'我们把商标放在了棒球衫上。'普法夫说道，'但这根本没用。我们没有关于为什么会生产棒球衫的故事。'"
  summary: |
    把商标贴到零售渠道要求的产品上、没有产品故事支撑，市场毫无反应。与品牌核心主题无关的扩张不会激活客户，再次验证"故事必须匹配品牌并引起共鸣"。
  tags: [product-extension, storytelling, failure]
- id: ce06
  title: "优步化"模仿倒闭潮
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "很快就出现了共享洗衣、共享洗车、共享家政、共享停车以及共享按摩，甚至还有共享冰激凌。……不幸的是，这些创业公司中的绝大多数现在都倒闭了。……为个体提供服务而获得的经济效益根本无法支撑公司的运营。"
  summary: |
    优步成功后数月内涌现的共享洗衣、洗车、家政、停车、按摩、冰激凌等公司大多倒闭：家政与按摩存在漏单和留存问题，低单价个体服务经济效益撑不起运营。教训：缺少原模式任一成立要素，照搬即崩塌。
  tags: [uberization, imitation, failure]
- id: ce07
  title: 瓦尔比派克模仿者们的集体失败
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "数百家抄袭者试图将同样的模式用在销售箱包、家具、珠宝、牙刷、胸罩、袜子、卫生棉等产品上。……经营其他品类的创业公司就没有这么幸运了，它们中的大多数到现在还在挣扎求存，或者已经倒闭了。"
  summary: |
    数百家"X品类的瓦尔比派克"中只有美元剃须俱乐部等少数成功。失败原因：内衣、牙线等品类货架上已有数十种价位产品、缺乏垄断溢价与复购结构，"简单地添加另一个选项并不会起什么作用"。
  tags: [warby-parker, imitation, failure]
- id: ce08
  title: 广告模式套在低频应用上必然崩溃
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "曾经有一位创业公司的创始人这样对我说：'我打算采用广告模式。'但是当我问他一个普通的用户使用他的应用的频率是多少时，这个创始人估算了一下说大概每两周一次。我不得不告诉他这个模式应该不适合他的公司。"
  summary: |
    用户每两周才用一次的应用无法靠广告模式发展成大型企业。广告模式只适合拥有海量用户且高参与度的媒体/社交类公司，其他创业公司强行采用注定失败。
  tags: [advertising, business-model, failure]
- id: ce09
  title: 硬件众筹：融得到钱、交不出货
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "这就是为什么我们在Kickstarter和Indiegogo这两个众筹平台上可以看到有那么多的硬件项目正在进行融资，但几乎看不到有哪个项目最后发布了它的产品。那些毫无经验的创始人常常低估了他们所需要的时间、金钱以及项目的复杂程度。"
  summary: |
    硬件创业陷阱：一旦投产成本上升，一次失误就足以让缺现金的公司倒闭；创始人普遍低估时间、金钱与复杂度。众筹平台上大量硬件项目融资成功却几乎无一下线交付。
  tags: [hardware, crowdfunding, failure]
- id: ce10
  title: Jawbone：9亿美元融资+数百项专利仍破产
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "它从投资人那里拿到了9亿美元的融资，并且还拥有涉及面相当广泛的专利组合。尽管它是这个市场的早期参与者，而且还申请了数百项专利，但最终因为质量控制问题、生产问题以及糟糕的产品设计而破产了。"
  summary: |
    可穿戴公司Jawbone坐拥巨额融资与数百项专利，仍因质量、生产与设计问题破产；试图靠起诉蜚比（Fitbit）自救也失败。证明"想拯救一艘正在沉没的船，仅仅依靠专利几乎是不可能的"。
  tags: [jawbone, patent, failure]
- id: ce11
  title: Nest：32亿美元收购后的期望落空
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "甚至连Nest也没有达成谷歌当初的期望，它在市场上的业绩一直表现不佳，对客户的深度变现以及与客户的互动也从来没有真正实现。"
  summary: |
    谷歌32亿美元收购的智能恒温器Nest未实现"互联家庭门户"的期望：业绩不佳、无法深度变现、客户互动从未实现。消费物联网的大多数投资"蛋最后都烂了"——因为用户不想与面包机恒温器建立持续关系。
  tags: [nest, iot, overexpectation]
- id: ce12
  title: 消费物联网订阅模式失灵
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "让人们为订阅或消耗品付费并不是一件简单的事。你不可能简单地把这两种模式应用在联网的设备上。……谁会愿意为了使用真空吸尘器、智能门锁或者智能吹风机而按月支付订阅费呢，更不用说只是为了使用能够互联在一起的电灯泡或者马桶了。"
  summary: |
    把订阅/易耗品模式硬套到联网电灯泡、马桶等设备上没有意义：订阅的前提是价值随时间累积，而多数智能家电无法提供。物联网炒作之下成功故事相对稀少的结构性原因。
  tags: [iot, subscription, mismatch]
- id: ce13
  title: 区块链硬塞进在线租赁平台
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "'我应该用区块链来创建我们的在线租赁平台吗？'……'这项技术能够为用户带来额外的价值吗？''不一定。'……'事实上，它会让项目的实施变得更加困难。'……这个创业者根本就没有想清楚。"
  summary: |
    区块链狂热期，创业者为融资把不适用的技术硬塞进商业计划：既不增加竞争优势，也不带来用户价值，反而增加实施难度。作者称之为"糟糕且不道德"，如同"用电钻把钉子钉入墙体"。
  tags: [blockchain, hype, ethics]
- id: ce14
  title: AI流行语"美容"骗投资
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "当人工智能（AI）成为网上的一个热搜词时，每一家拥有某种算法和数据库的创业公司都会突然间开始拼命地向投资人、客户甚至媒体推销其人工智能技术。……它们只是利用这些最新的流行语给自己的企业做了一次快速的'美容'。"
  summary: |
    每次炒作周期顶部都有公司靠流行语重新包装自己，而业务实质未变；单纯的投资人在未理解技术与基本面的情况下跟风投资。创业公司与投资人双向的短视警示。
  tags: [ai, hype, investors]
- id: ce15
  title: Yo应用：150万美元买的教训
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "有一款社交应用被称作Yo，它唯一能做的就是让用户给他们的朋友发送'哟！'这个词。正是这个极其愚蠢的想法，引起了每个人的注意……一些天真的投资人跟风而行，向那家创业公司投入了150万美元，意料之中的是，这只火鸡根本就飞不起来。"
  summary: |
    只能发送"哟！"的社交应用凭噱头登顶应用商店、获得大量报道与150万美元投资，但毫无价值支撑，注定失败。警告：媒体热度本身不等于成功，必须有团队、产品与愿景配合。
  tags: [yo, media-hype, failure]
- id: ce16
  title: 戴森被投资人踢出公司
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "他的投资人很恼火。……'如果这是一个极其出色的创意，那么为什么胡佛公司或者伊莱克斯公司不那样做呢？'……所以当戴森坚持要推进他自己的想法时，投资人感到非常不安，最终他们把他直接踢出了公司。"
  summary: |
    戴森因坚持做无袋旋风吸尘器与外部投资人冲突，被踢出自己创立的公司，一度身无分文。教训：引入与愿景不合的投资人可能失去公司控制权；"大企业没做=不可行"的推理会误杀真正的好创意。
  tags: [dyson, investors, control]
- id: ce17
  title: 投资人的常春藤联盟陷阱
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "有太多的投资人都掉进了常春藤联盟这个陷阱，他们把大学的名字和成功等同了起来，这使得他们对于某些最重要的东西视而不见。……还会让你很武断地过滤掉一些非常有意思的性格类型，比如叛逆者、追求精神自由的人以及大器晚成者。"
  summary: |
    用CEO就读大学做筛选会错过马云、乔布斯、戴尔、布兰森这类未上名校的成功者；名校录取看的是考试与课外活动而非领导力。全国经济研究局数据显示名校生终生收入与同分数段其他学校毕业生几乎无差别。
  tags: [ivy-league, bias, investing]
- id: ce18
  title: 简历与头衔的迷惑性
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "CEO曾经在一家世界级的企业里工作这当然很不错，但是这并不意味着这个人肯定能成为一个出色的创业公司的创始人。……甚至有些高管什么也不用做，只需要玩弄办公室政治就能坐稳他们的位置。"
  summary: |
    谷歌6万员工、微软12.5万员工中大多数只是适合在大公司工作；副总裁可能只是优秀的执行者甚至办公室政治玩家而非冒险家。仅凭大公司履历和头衔下注会选错创始人。
  tags: [resume, title, bias]
- id: ce19
  title: CEO把核心知识产权藏在自己名下
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "这家公司的CEO将核心知识产权归在了他个人的名下，而且并没有将这件事告诉任何人。事实上他误导了我们，这几乎等同于欺诈了。我对这个创业者失去了所有的尊重，拒绝将他介绍给投资人，并切断了和这家公司的所有联系。"
  summary: |
    作者尽调中发现CEO私自把公司核心IP登记到个人名下并隐瞒，等同欺诈，直接断绝合作。教训：隐瞒关键信息一旦在尽调中暴露，失去的不仅是一笔交易而是声誉与全部融资渠道。
  tags: [due-diligence, fraud, ip]
- id: ce20
  title: 文件散落各处弄丢了融资
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "我曾经看到一笔失败的交易就是因为创业公司将其所有的书面文件分散地放在很多不同的地方。这家创业公司的文件有很多被存放在了一台很旧的笔记本电脑里，其他的甚至已经遗失了。……几家原本感兴趣的公司已经转移了目标。"
  summary: |
    协议文档分散、部分遗失，创始人花数周才补齐材料，等待期间原本感兴趣的投资人已转向别处。教训：应把全部协议副本集中存放在云文件夹，随取随用；投资人是出了名的善变。
  tags: [due-diligence, documents, failure]
- id: ce21
  title: 投资意向书拖延与临时改条款
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "当我为我的第二家创业公司进行融资的时候，我们花了整整4万美元的律师费，但投资人在最后一刻修改了针对我们的条款，交易也因此泡汤了。当时我真的很希望在我们的投资意向书中有相应的条款可以应对这样的情况。"
  summary: |
    无约束力意向书的陷阱：投资人借此锁定交易、排除竞争者后拖延甚至临时改条款退出，公司白付4万美元律师费且蒙上"被领投放弃"的阴影。应对：在意向书中设定尽调时间表与补偿条款（尽管多数顶级风投不会同意）。
  tags: [term-sheet, fundraising, trap]
- id: ce22
  title: 一次性售卖硬件被克隆品压死
  type: counter_example
  source_chapter: 第五章
  source_quote: |
    "一家创业公司花了一年或更长的时间进行创新，推出了一款非常酷的新产品……然后它把这款产品放在了Kickstarter或者Indiegogo上进行融资……但最后发现抄袭者在很短的时间里就以一个更低的价格在市场上开始销售同样的东西。"
  summary: |
    一次性售卖+硬件的组合双重脆弱：消费电子领域低成本复制品不断压低价格，几个月内克隆品就会出现，创业公司利润被侵蚀后无线打造品牌。没有专利壁垒或高进入壁垒时，此模式难以存活。
  tags: [hardware, copycat, one-time-sale]
- id: ce23
  title: 广告标题：记者直觉不敌数据
  type: counter_example
  source_chapter: 第四章
  source_quote: |
    "让人感到惊讶的是，当面向读者进行测试时，新闻记者最喜欢的那些标题往往表现得不尽人意。依靠直觉的日子已经过去了，那不过是一种对标题做出判断的古老方式，数据分析才是如今的专业人士使用的方法。"
  summary: |
    专业记者凭直觉最喜爱的标题在真实读者测试中往往表现不佳。反例说明内容决策不能依赖个人口味（哪怕是专家口味），必须用A/B测试数据说话。
  tags: [headline, intuition, ab-testing]
```

### 5. terms

```yaml
- id: tm01
  title: 增长黑客（Growth Hacking）
  type: term
  source_chapter: 第四章
  source_quote: |
    "增长黑客是一个以业务增长为目标而展开的快速实验的过程，整个过程将贯穿你的营销漏斗、产品开发、销售以及所有其他的相关环节。肖恩·埃利斯（Sean Ellis）在2010年杜撰了这个词。"
  summary: |
    由肖恩·埃利斯2010年提出的概念：以增长为唯一目标的快速实验过程，贯穿营销漏斗、产品开发与销售；将创意营销、软件工程、自动化、测试与数据分析结合。与传统营销的区别在于更加别出心裁、不守成规，不需大量资金，特别适合预算紧张的早期公司。
  tags: [growth-hacking, term]
- id: tm02
  title: 游击营销（Guerrilla Marketing）
  type: term
  source_chapter: 第四章
  source_quote: |
    "游击营销的关键在于如何有效地利用资源，如何用某些替代的方式来建立你的品牌并获得客户。你有多少种创意，你就会有多少种类型的游击营销。"
  summary: |
    用非常规、低成本、高创意的方式建立品牌与获取客户的营销方法。唯一规则是与众不同、脱颖而出；用独创性弥补资金缺口，靠激发情感反应、创造对话氛围、鼓励分享来实现自发传播。
  tags: [guerrilla-marketing, term]
- id: tm03
  title: 集客营销（Inbound Marketing）
  type: term
  source_chapter: 第四章
  source_quote: |
    "集客营销是一种让顾客自己找上门的营销策略，也是一种'关系营销'或'许可营销'。营销者以自己的力量赢得顾客的青睐，而非通过传统的广告方式去拉客。这个概念诞生于2008年。（译者注）"
  summary: |
    通过创造有价值的内容与SEO让客户主动找上门的营销策略（概念诞生于2008年）。前提是内容必须对目标客户有价值（教育或娱乐），核心是搜索引擎优化：为业务关键关键词争取搜索结果顶部位置。
  tags: [inbound-marketing, term]
- id: tm04
  title: 病毒式传播与病毒式增长
  type: term
  source_chapter: 第四章
  source_quote: |
    "我们都听说过所谓的病毒式增长，但是在现实中，很少有产品能够像病毒一样增长。在企业发展的某个时间节点，几乎每一家创业公司都必须拿出一笔相当大的市场营销预算。"
  summary: |
    内容或产品像病毒一样借助用户自发分享扩散的现象（如冰桶挑战250万个标签视频）。作者同时泼冷水：现实中很少有产品能真正病毒式增长，几乎每家公司最终都需要可观的市场预算来扩张到早期用户之外。
  tags: [viral, term]
- id: tm05
  title: 独角兽（Unicorn）
  type: term
  source_chapter: 第五章
  source_quote: |
    "如果一家创业公司无法提供真正卓越的产品，或者做到与众不同，那么想要撬开某个品类的市场，并成长为独角兽企业将会是一件非常困难的事情。"
  summary: |
    书中指估值达到十亿美元级别的顶级初创公司（如Slack、Affirm、Dropbox）。独角兽的共同特征：市场领导地位、可扩展性、锁定客户的长期关系、深度变现能力、强大的团队纽带；其估值与是否拥有专利无关。
  tags: [unicorn, term]
- id: tm06
  title: 独角兽猎人（Unicorn Hunter）
  type: term
  source_chapter: 第五章
  source_quote: |
    "风险投资公司又是如何在一家独角兽企业还没长出犄角之前就找到它的呢？……独角兽猎人总是在搜寻那些能够比所有其他人更早发现某个新趋势，并准备利用这一趋势的企业。"
  summary: |
    作者对在独角兽"长出犄角之前"识别未来赢家的顶尖投资人的称呼。他们的工作方式：解构创业公司、评估商业模式、以团队→市场→客户→趋势→卓越→秘诀→模式→锁定→设计→媒体→文化的顺序过滤交易。
  tags: [unicorn-hunter, investing, term]
- id: tm07
  title: 生活方式企业（Lifestyle Business）
  type: term
  source_chapter: 第四章
  source_quote: |
    "风险投资人通常会把这一类的企业称为'生活方式'企业，因为它们通常会在某个节点停止增长，这就使得风险投资公司很难退出。"
  summary: |
    风投对年收入数百万美元且能盈利、但在某节点停止增长的企业类别称呼。因其难以退出而无法满足风投模式，但对创业者本身可以是相当不错的成就（年赚百万美元以上）——前提是没有拿要求持续扩张的风投资金。
  tags: [lifestyle-business, vc, term]
- id: tm08
  title: A/B测试
  type: term
  source_chapter: 第四章
  source_quote: |
    "例如，Upworthy就会对它的所有标题进行A/B测试，这种做法更加科学。"
  summary: |
    将多个版本（标题、页面等）同时投放给真实受众、以实际数据（点击量）而非直觉判断优劣的方法。书中以Upworthy的"25个标题→4个候选→社交网络测试→选数据最优"为标准操作流程。
  tags: [ab-testing, term]
- id: tm09
  title: 用户画像（Buyer Persona）
  type: term
  source_chapter: 第四章
  source_quote: |
    "创建用户画像。这是对一个标准客户非常细致的描述。一旦你能清晰地定义你的买家，你就不会把那么多的时间浪费在那些永远也无法产生转化的销售线索上。"
  summary: |
    对标准客户非常细致的描述。用途：清晰定义买家后，不再把时间浪费在永远无法转化的销售线索上；是集客营销推广策略的组成部分，也是第五章"谁是你的客户"追问的对应工具。
  tags: [persona, marketing, term]
- id: tm10
  title: 跳出率（Bounce Rate）
  type: term
  source_chapter: 第四章
  source_quote: |
    "网站跳出率是对网站进行分析的最基本度量之一，网站跳出率=只浏览一个页面的访问量/整个网站所有的访问量。（译者注）"
  summary: |
    网站分析基本度量：只浏览一个页面的访问量除以总访问量。降低手段包括实时聊天、聊天机器人、网络研讨会等让用户参与和反馈的机制；体验越个性化，参与度和转化率越高。
  tags: [bounce-rate, analytics, term]
- id: tm11
  title: DAU / MAU（日/月活跃用户）
  type: term
  source_chapter: 第五章
  source_quote: |
    "我会特别关注DAU（日活跃用户）、MAU（月活跃用户）、客户留存率、客户参与模式、产品在网上的传播能力以及业务的增长状况。"
  summary: |
    投资人审查在线创业公司时关注的核心数据指标组：日活、月活、留存率、参与模式、网络传播力与增长状况。作者要求创始人开放数据分析平台全部权限以便直接复核；没有数据意味着"凭感觉做事"，是危险信号。
  tags: [dau, mau, metrics]
- id: tm12
  title: 最小可行性产品（MVP）
  type: term
  source_chapter: 第五章
  source_quote: |
    "无论你是建立一个视频背景的登录页面，还是发布一款最小可行性产品，你都能从用户那里挖掘数据，评估他们的反应模式，然后利用这些信息来确保你自己没有偏离正确的轨道。"
  summary: |
    用最小成本把产品雏形（或仅为视频登录页）推向真实用户，从中挖掘数据、评估反应模式以验证方向。是客户"说一套做一套"时靠行为数据而非访谈判断需求的手段。
  tags: [mvp, validation, term]
- id: tm13
  title: 订阅模式（Subscription）
  type: term
  source_chapter: 第五章
  source_quote: |
    "订阅模式被客户接受之后，这实际上能为企业提供一个稳定的、可预测的收入来源。投资人很喜欢这种模式，因为他们能够很容易地从过去的数据中推断并预测未来的增长。"
  summary: |
    按月/按年收费的可持续收入模式：初期付费低甚至免费（低风险试用），累计总收入远超一次性大额购买；收入可预测，投资人易于外推增长。企业级例：Zendesk、GitHub；消费级例：Netflix、美元剃须俱乐部。
  tags: [subscription, recurring-revenue, term]
- id: tm14
  title: 平台与网络效应（Platform / Network Effect）
  type: term
  source_chapter: 第五章
  source_quote: |
    "平台通常会从每一笔交易中抽取一个很小比例的提成……更妙的是，这种模式不容易被复制。……这意味着在平台上进行交易的买家和卖家越多，这个平台对于每个人的价值就越大。"
  summary: |
    从每笔交易抽取小比例提成的模式，随交易量累积成"提款机"；网络效应指买家卖家越多平台价值越大，一旦亚马逊、淘宝、爱彼迎等取得支配地位，竞争对手几乎无法追赶。作者称之为最强大、最适合规模化且最难被复制的商业模式。
  tags: [platform, network-effect, term]
- id: tm15
  title: 客户锁定与转换成本（Lock-in / Switching Cost）
  type: term
  source_chapter: 第五章
  source_quote: |
    "独角兽企业有一个共同特征，那就是它们都拥有把客户锁定在长期关系中的能力。这种关系越牢固，竞争对手抢走它们的客户的难度也就越大，从而带来更高的利润率以及长期的增长。"
  summary: |
    让客户把时间与资源投入产品（邀请好友、上传内容、定制、集成工作流），使其离开时要承担高昂转换成本。这是大型软件公司高利润率的根源（Windows、SAP、甲骨文），也是竞争对手面临的进入壁垒。
  tags: [lock-in, switching-cost, term]
- id: tm16
  title: 品类杀手（Category Killer）
  type: term
  source_chapter: 第五章
  source_quote: |
    "卓越的产品会是一个品类杀手，它们会吞下其他人的午餐。这就是为什么谷歌会在搜索上占据主导地位，并且还比与其最接近的竞争对手在公司的市值上高出很多倍。"
  summary: |
    指卓越到足以主导整个品类的产品。配套现象是"品牌等同品类"：想到CRM就是Salesforce、想到数据库就是甲骨文、想到电子签名就是DocuSign——占有品类通用名称的领头羊获得认知、媒体、信任与网络效应叠加的巨大进入壁垒。
  tags: [category-killer, market-leadership, term]
- id: tm17
  title: 设计思维（Design Thinking）
  type: term
  source_chapter: 第五章
  source_quote: |
    "设计思维是一个完整的过程，包括定义问题、研发、形成想法、设计原型以及测试。卓越的设计团队中不但会有工程师和产品设计师，而且还会有心理学、人种学、文化人类学、人体工程学、认知和感知等领域的专家。"
  summary: |
    完整过程：定义问题→研发→形成想法→设计原型→测试；团队除工程师与产品设计师外还包括心理学、人种学、人体工程学等领域专家。乔布斯式定义：设计不只是好看的外观，而是产品如何表达其功能、如何与使用者情绪互动。
  tags: [design-thinking, term]
- id: tm18
  title: 投资意向书（Term Sheet）
  type: term
  source_chapter: 第五章
  source_quote: |
    "为了在一笔热门的交易中排除可能会出现的竞争者，很多投资人会要求创业者签署一份没有约束力的投资意向书。……接下来就是一个等待的游戏了。"
  summary: |
    无约束力的投资意向文件：投资人用它锁定交易、排除竞争者，之后可随时找借口退出；签署后公司必须告知其他投资人，势头即断。应对：在意向书中设定尽调时间表与截止日期（及可能的补偿条款），且签署前披露所有实质性信息。
  tags: [term-sheet, fundraising, term]
- id: tm19
  title: 尽职调查（Due Diligence）
  type: term
  source_chapter: 第五章
  source_quote: |
    "在尽职调查的过程中，聪明的投资人不会只阅读你交给他们的文档。他们会提出与你的团队中最重要成员单独面谈。……他们就是用这种方式来发现你的企业中可能存在的问题的。"
  summary: |
    投资人在承诺投资前对公司的深入核查：审阅文档（IP转让协议、股权结构表等）、与管理团队逐一单独面谈并交叉比对答案、核查数据平台权限。创业公司应对原则：不隐瞒任何事、团队口径一致、文档集中存放于云文件夹。
  tags: [due-diligence, investing, term]
- id: tm20
  title: 特洛伊木马（硬件比喻）
  type: term
  source_chapter: 第五章
  source_quote: |
    "我认为硬件就像是特洛伊木马，如果它能够成功地说服客户把一款产品带进自己的家门，并且这款产品的内置软件还能够悄悄地接管客户的很多日常应用，这样的软硬件组合就必定能够赢得投资人的青睐。"
  summary: |
    作者对理想硬件角色的比喻：硬件是进入客户家庭的载体，内置软件随后接管客户日常应用、建立持续关系与变现通道。解决了纯硬件"卖完即失联"的缺陷，是软硬件组合获得投资人青睐的结构。
  tags: [hardware, trojan-horse, term]
- id: tm21
  title: 赢家通吃（Winner-Takes-All）
  type: term
  source_chapter: 第五章
  source_quote: |
    "因为这是一个赢家通吃的世界。业务的规模越是容易扩大，拥有最佳产品的公司也就越容易主导整个市场，这是因为每个人都会被卓越的东西所吸引。"
  summary: |
    可扩展性越强的业务，市场越向第一名集中：卓越产品吸引绝大多数客户，领头羊更易融资、享有规模经济与网络效应，起点的小领先会迅速放大为巨大领先。推论：创业公司"优秀永远不够"，必须卓越或截然不同。
  tags: [winner-takes-all, scalability, term]
- id: tm22
  title: 猫咪视频测试
  type: term
  source_chapter: 第四章
  source_quote: |
    "他总是问自己一个简单的问题：虽然有那么多可爱的猫咪视频可以用来分享，但是为什么还会有人愿意转发我的视频呢？所以，如果有某个视频无法通过他的猫咪视频测试，他就不会发布这个视频。"
  summary: |
    Betabrand创始人林德兰德的内容筛选标准：发布前自问"为什么有人愿意转发我的视频"，通不过就不发布。可迁移为任何内容营销的传播性自检——在社交媒体语境中与猫咪视频争夺注意力。
  tags: [content, viral, term]
```

## 自检说明

- 全部候选均出自 ch04.txt / ch05.txt 原文，每条附原文引用且不超过150字。
- 每条至少1个 tag；未做筛选，两章中可识别的框架、原则、案例、反例、术语均已提取。
- 数量：frameworks 22 条、principles 28 条、cases 37 条、counter_examples 23 条、terms 22 条。
- 注：书中未出现"病毒系数（viral coefficient）"的明确定义，故术语仅收录"病毒式传播/病毒式增长"及其实操含义，未杜撰。
