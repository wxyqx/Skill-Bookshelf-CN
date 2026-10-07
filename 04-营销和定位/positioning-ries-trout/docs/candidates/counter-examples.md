# 反例池（去重合并后）

来源：《定位：有史以来对美国营销影响最大的观念》（里斯 & 特劳特）。由 scannerA/B/C/D 四个章节扫描器的 counter_example 候选跨章去重合并而成；`origin` 保留原始候选编号以便回溯。

```yaml
- id: e01
  title: FWMTS陷阱：忘记成功之道
  type: counter_example
  source_chapter: 第4章
  source_quote: |
    "每当一家公司打赢了一场漂亮的定位战后，它往往会掉进我们所谓的FWMTS陷阱：'忘记成功之道。'（Forgot what made them successful, FWMTS.）"
  summary: |
    定位成功后的典型失败模式：不甘于既有位置，转而宣传愿望而非事实。安飞士改打"安飞士要当第一"
    （心理与战略双错——潜在顾客会想"不，你才不是呢"）、七喜宣称"美国人人喝七喜"，都放弃了使它们成功的
    定位（关联第二/非可乐），市场份额随之下滑。教训：位置就是资产，离开自己的位置等于清零重来；
    成功定位必须始终如一，数年如一日。
  tags: [fwmts, wishful-thinking, trap, consistency]
  origin: [A-ce01]

- id: e02
  title: 「我能行」精神与自我导向型营销人
  type: counter_example
  source_chapter: 第5、22章
  source_quote: |
    "美国在越南的经历是美国人'我能行'精神的一个典型例子。只要足够努力，任何事情都可能办到。但是，无论我们怎样努力……这个问题都无法通过外力解决。"
  summary: |
    相信只要足够努力、投入足够金钱，任何目标都能实现——越战、RCA攻IBM、55岁副总裁等提拔皆是此病。
    第22章进一步刻画其人格化版本"自我导向型营销人"：成群参加鼓劲大会，深信有了合适的动力没有办不到的事，
    用意志、决心、努力和内部资源清单替代对潜在顾客心智与竞争对手的分析，理解不了"在潜在客户心智中定位"的本质。
    教训：位置不对时，越努力只会越快耗尽资源；先判断位置是否可达，再谈投入。
  tags: [can-do-spirit, self-orientation, effort-fallacy, mindset]
  origin: [A-ce02, D-fx09]

- id: e03
  title: "什么都卖得掉"的60年代与跟风产品
  type: counter_example
  source_chapter: 第3章
  source_quote: |
    "令人兴奋的'什么都卖得掉'的年代是一次营销的狂欢。……如杜邦公司的可发姆人造皮革；加布林格（Gablinger's）公司的啤酒；Convair牌880型汽车、Vote牌牙膏、Handy Andy牌吸尘器等。"
  summary: |
    时代性失败模式：60年代公司相信有钞票魔力和聪明人才，任何营销项目都能成功，结果沉船残骸接连冲上海滩
    （可发姆、加布林格、Convair 880、Vote牙膏、Handy Andy吸尘器等）。大量跟风产品指望"出色的"广告扭转乾坤，
    货架塞满"半成功"品牌。教训：市场噪音已太大，"好产品+好计划+好创意=成功"的前提——市场本身——已经变了。
  tags: [me-too-product, 1960s, advertising-failure]
  origin: [A-ce03]

- id: e04
  title: 雪佛兰的十个车型名：命名混乱稀释认知
  type: counter_example
  source_chapter: 第2章
  source_quote: |
    "这些容易混淆的名称使得雪佛兰的地位落到了福特之后而屈居第二。雪佛兰车是世界上广告最多的产品。"
  summary: |
    产品爆炸下的品牌混乱案例：Camaro、Caprice、Chevette、Corvette、Impala等十个车型名令顾客无从分辨，
    雪佛兰跌居福特之后——尽管它是世界上广告最多的产品（每年1.3亿美元以上）。与第13章"试图满足所有人"
    互为表里：多车型共用一个品牌名且命名混乱，只会稀释认知。教训：广告量无法替代清晰的心智位置。
  tags: [chevrolet, naming-confusion, model-explosion]
  origin: [A-ce04]

- id: e05
  title: 康纳利：根深蒂固的认知无法用金钱改变
  type: counter_example
  source_chapter: 第2章
  source_quote: |
    "约翰・康纳利（John Connally）花了1100万美元才得了一张选票……'这个认知太根深蒂固了，'他的竞选战略顾问说，'谁也不可能改变。'"
  summary: |
    政治传播失败案例：康纳利在1980年大选初选花1100万美元只换来一张选票，因为"独断专行"的认知已根深蒂固，
    谁也无法改变。与杰里·布朗（新闻报道铺天盖地，公众仍只记得四件事）共同说明：过度传播社会中第一印象
    几乎不可更改，对抗既有认知的传播无论砸多少钱都必然无效。
  tags: [connally, politics, entrenched-perception]
  origin: [A-ce05]

- id: e06
  title: 米狮龙：成功后偏离定位（FWMTS实例）
  type: counter_example
  source_chapter: 第3、7章
  source_quote: |
    "不幸的是，米狮龙因提出'夜晚属于米狮龙'这样的话而丧失了'一流'的地位。这太糟糕了。要不然它有可能跻身两三种最畅销的国产品牌之列。"
  summary: |
    米狮龙靠"堪称一流"的高价国产啤酒定位广告（作者称为有史以来最出色的定位广告之一）大获成功后，
    先后改用"夜晚属于米狮龙""周末是为米狮龙创造的"之类与定位无关的空洞诗意诉求，结果丧失"一流"地位，
    错失跻身最畅销国产品牌的机会。两处章节讲述同一教训：空位战略不是一次性动作，放弃定位概念等于亲手
    拆除自己占据的位置；定位一旦建立必须持续强化。
  tags: [michelob, fwmts, drift, inconsistency]
  origin: [A-ce06, B-xb05]

- id: e07
  title: 正面进攻领导者必败
  type: counter_example
  source_chapter: 第5、7、22章
  source_quote: |
    "NCR公司没有抵挡住诱惑，与IBM正面作战，最后几乎一蹶不振。"
  summary: |
    跨章反复出现的失败模式：向心智中地位稳固的领导者发起正面进攻。NCR本拥有现金出纳机的强大心智位置，
    却与IBM正面作战几乎一蹶不振（后靠"计算机化现金出纳机"定位才恢复元气）；DEC花了很长时间企图
    "在个人电脑上超过IBM"，结果错过开发台式计算机的机会，最终被康柏收购；布利斯特-麦尔斯连打四场正面战——
    Fact挑战佳洁士（500万美元后放弃）、Resolve挑战Alka-Seltzer（1100万美元后放弃）、Dissolve挑战拜耳、
    Datril挑战泰诺，全部花钱买烦恼。教训：决不与稳固的领导者正面交锋，绕过障碍或另立新品类。
  tags: [frontal-attack, leader, failure]
  origin: [A-ce07, B-xb11, D-fx12]

- id: e08
  title: 感觉超载与心智容量不足
  type: counter_example
  source_chapter: 第2章
  source_quote: |
    "对人脑敏感性的研究发现，存在一种'感觉超载'的现象。科学家发现，人只能接受有限的感觉。超过某一极限，脑子就会一片空白，失去正常的功能。"
  summary: |
    警告性事实：心智是"容量不足的容器"，信息超过极限大脑即一片空白（牙医以此原理用噪声压制痛觉）。
    广告量增加8倍而心智接受量不变——奢求更多等于忽视心智容量有限的事实。这是"多则是少"、必须简化信息的
    生理学根据，也是一切过度传播策略必然失效的底层原因。
  tags: [sensory-overload, capacity, evidence]
  origin: [A-ce08]

- id: e09
  title: 喜力弃用领导地位诉求
  type: counter_example
  source_chapter: 第6章
  source_quote: |
    "像喜力啤酒这样的领导者很可能要经常做广告宣传其领导地位。不幸的是，喜力弃用了'美国进口啤酒第一品牌'这句话，而最后把领导地位拱手让给了科罗娜。"
  summary: |
    领导者停止对新进入市场的消费者宣传领导地位，等于把位置让给后来者——喜力弃用"美国进口啤酒第一品牌"
    这句话，最后把领导地位拱手让给科罗娜。教训：总有一部分消费者不知道谁是第一，领导地位诉求需要持续重复，
    "正宗货"式的正统性宣传不可中断。
  tags: [heineken, leadership, advertising]
  origin: [B-xb01]

- id: e10
  title: 宝丽莱把柯达赶出市场
  type: counter_example
  source_chapter: 第6章
  source_quote: |
    "宝丽莱犯了一连串的错误，控告柯达并且把它赶出了一次成像照相机市场。结果两败俱伤。"
  summary: |
    领导者试图消灭跟随者：宝丽莱诉讼柯达并把它赶出一次成像市场，结果两败俱伤——宝丽莱并未实现垄断，
    柯达只拿到很小份额却损失了传统相机业务。教训：是跟随者造就了品类，领导者需要跟随者来形成品类，
    把对手赶出市场是双输。
  tags: [polaroid, kodak, litigation]
  origin: [B-xb02]

- id: e11
  title: 多元化陷阱：定位与多元化南辕北辙
  type: counter_example
  source_chapter: 第6、14、22章
  source_quote: |
    "定位和多元化这两个概念南辕北辙。"
  summary: |
    离开核心定位搞多元化、追变化，是全书跨章反复出现的失败模式。施乐误以为企业实力可复制，进入计算机业务
    损失几十亿美元，还把台式激光打印机先机让给惠普；胜家做家庭用品、RCA做计算机、通用食品开快餐店，
    "为跟上变化而仓促上马的项目"尸横遍野，同期坚持本位的美泰克、迪斯尼、雅芳全部巨大成功；把多元化当
    公司定位主题同样失败——ITT最终分成三家独立公司，Kaiser控股解体后股东每股拿到21美元（市价仅12美元）。
    背后是"万物恒变"错觉与"企业实力产生于企业规模"的实力错觉。教训：实力只存在于心智定位之内，
    强大定位建立在重大成就而非宽泛产品线上。
  tags: [diversification, focus, change-illusion]
  origin: [B-xb03, C-cx12, D-fx08, D-fx11]

- id: e12
  title: Advent品牌延伸破产
  type: counter_example
  source_chapter: 第7章
  source_quote: |
    "米歇尔先生做出决定说：'让我们把Advent及其分支业务从老路上带出来，打进家庭娱乐中心行业。'不出所料，Advent最后上了破产法院。"
  summary: |
    Advent发明投影式电视机并建立了定位，却嫌份额不够，携同一品牌闯入家庭娱乐中心行业，最终破产。
    教训：在既有定位上建立的品牌名不能覆盖新业务，品牌延伸过度是空位战略的常见死法。
  tags: [advent, brand-extension, bankruptcy]
  origin: [B-xb04]

- id: e13
  title: Luke晚到20年与Eve跟风失败
  type: counter_example
  source_chapter: 第7章
  source_quote: |
    "唯一的不足的是选错了时机，晚了大约20年。Luke的确来得太缓慢，罗瑞拉德公司只好放弃了它。"
  summary: |
    罗瑞拉德的Luke男性化香烟（名字、包装、广告俱佳）因比万宝路晚约20年而失败；Eve模仿维珍妮的女性化
    路子同样失败。教训：性别空位只属于第一个占据者，同样的定位第二做无效——时机和次序比创意质量更重要。
  tags: [luke, eve, timing]
  origin: [B-xb06]

- id: e14
  title: Aim放弃孩子定位
  type: counter_example
  source_chapter: 第7章
  source_quote: |
    "Aim公司放弃了这个定位于孩子的战略后，其10%的市场份额也落到了0.8%。"
  summary: |
    曾在佳洁士与高露洁割据的牙膏市场辟出10%份额的儿童定位，被公司自己放弃后份额崩塌至0.8%。
    教训："好东西不用就会失去"，定位不是取得一次就终身有效的资产，必须持续经营。
  tags: [aim, positioning, neglect]
  origin: [B-xb07]

- id: e15
  title: 《全国观察家报》填补工厂空位
  type: counter_example
  source_chapter: 第7章
  source_quote: |
    "于是，你会听到有人说，让我们出一份周报来填补这个空位吧，这样就能免费使用那些成本昂贵的日报印刷设备了。但是，潜在客户心智里的空位在哪里？"
  summary: |
    道·琼斯公司为利用《华尔街日报》闲置印刷设备推出全国性周报，从生产端看是"完美"逻辑，
    但读者心智已被《时代》《新闻周刊》等占满。教训：工厂空位（产能、产品线缺口）不等于心智空位，
    以内部逻辑找位必败。
  tags: [national-observer, factory-gap, dow-jones]
  origin: [B-xb08]

- id: e16
  title: 技术陷阱：心智里没有的空位
  type: counter_example
  source_chapter: 第7章
  source_quote: |
    "Frost8/80和第一份白色啤酒透明米勒（Miller Clear）或第一份白色可乐水晶百事（Crystal Pepsi）一样，都以失败而告终。"
  summary: |
    一系列"技术上第一"的产品——干白威士忌Frost 8/80、透明米勒啤酒、水晶百事、绿色番茄沙司——全部失败，
    因为它们要求消费者推翻心智中根深蒂固的颜色/类别认知。教训：实验室里的第一不是心智里的第一，
    技术优势无法对抗既有认知；判断标准是"在人们心智中是不是第一"，而非"在瓶子里是不是第一"。
  tags: [technology-trap, crystal-pepsi, perception]
  origin: [B-xb09]

- id: e17
  title: 满足所有人需求陷阱
  type: counter_example
  source_chapter: 第7、13、21章
  source_quote: |
    "公司犯的最大的错误就是试图满足所有人的需求，即人人满意陷阱。"
  summary: |
    不想被定位束缚、想"什么都能做"的公司和个人在竞争中难以取胜。雪佛兰20年不断推新品种（在售车型超过
    福特），成了"既大又小、既便宜又昂贵"的车，把领导地位让给福特；麦凯恩竞选失败同此理——乔治·布什是
    "有同情心的保守派"，麦凯恩代表什么没人说得出；Rheingold啤酒为纽约各民族分别制作"自己人"版广告
    想吸引所有人，结果什么人也没吸引到、市场萎缩（同城的Schaefer聚焦"重度饮用者"则成功）。
    教训：参与竞争者太多，不树敌、人人满意的策略在传播过度的社会里行不通；必须做出取舍、开辟明确定位，
    即使有所损失。检验问句："它是什么？"答不出来即已稀释。
  tags: [everyone-trap, trade-off, positioning-drift]
  origin: [B-xb10, C-cx07, D-fx04]

- id: e18
  title: 拜耳反驳泰诺适得其反
  type: counter_example
  source_chapter: 第8章
  source_quote: |
    "潜在顾客会这样想：'既然拜耳的阿司匹林这么担心泰诺，居然花百万美元打广告反驳对方这些说法，那么阿司匹林会造成胃出血的观点肯定有一定的道理。'"
  summary: |
    拜耳面对泰诺的重新定位攻击（阿司匹林伤胃）时选择花百万美元广告反驳，潜在顾客反而推论：
    "既然拜耳这么担心，这说法肯定有道理。"教训：对重新定位的错误防御比不防御更糟；
    被重新定位时应以事实和品类教育回应，而非情绪化否认。
  tags: [bayer, tylenol, repositioning-defense]
  origin: [B-xb12]

- id: e19
  title: 红牌退缩送掉领先地位
  type: counter_example
  source_chapter: 第8章
  source_quote: |
    "它不再提自己的俄罗斯背景，打出的广告对其俄罗斯传统避而不提，结果给绝对牌伏特加以可趁之机。后者打入伏特加市场后抢占了领先地位，并且保持至今。"
  summary: |
    红牌伏特加因阿富汗危机羞于俄罗斯定位、广告回避俄罗斯传统，绝对牌趁虚抢占"俄式正宗"心智位置并保持
    领先至今。教训：定位的完整性经不起时机性羞怯；放弃自己占据的词，就是把它送给对手。
  tags: [stolichnaya, absolut, retreat]
  origin: [B-xb13]

- id: e20
  title: 品客进入"失败者惩罚箱"
  type: counter_example
  source_chapter: 第8章
  source_quote: |
    "在人类心智中某个小小的角落里，有一个写着'失败者'的惩罚箱。你的产品一旦被放进那个箱子里，就没戏了。"
  summary: |
    宝洁花1500万美元推出品客，一度占18%市场，被智慧薯片当众朗读成分标签重新定位为"化工合成品"后跌至10%，
    虽以"全天然"、包装卖点反击，仍无法实现预期。教训：心智中的"失败者惩罚箱"一旦入箱，修补无效，
    正确做法是推出新产品从头再来。
  tags: [pringles, failure, p&g]
  origin: [B-xb14]

- id: e21
  title: 莱特啤酒的通用名灾难
  type: counter_example
  source_chapter: 第9章
  source_quote: |
    "莱特的巨大优势在于它是第一个进入人们心智的淡啤品牌，可是这个通用性名字最后成了一个巨大的劣势。"
  summary: |
    米勒"莱特"（Lite）是第一个进入心智的淡啤，但名字与通用词"light beer"同音，公众与新闻界把它叫成
    "米勒淡啤"，米勒失去"淡啤/Lite"商标专用权，被迫改名米勒莱特并节节败退，最终百威淡啤成为第一。
    教训：名字不能"过头"成通用名称，否则为整个品类做嫁衣；定位成功不等于品牌资产安全。
  tags: [lite-beer, generic-name, miller]
  origin: [B-xb15]

- id: e22
  title: 门侬E、Breck One与高露洁100
  type: counter_example
  source_chapter: 第9章
  source_quote: |
    "门侬E牌除臭剂尽管花了1000万美元做广告，但它注定要失败。问题就出在名字上。"
  summary: |
    一系列含义怪异或无意义的名字：维生素E除臭剂（"维生素E竟成了除味剂"）、Breck One、高露洁100，
    砸重金推广仍失败。教训：行业内专业术语和数字代号在潜在客户心智中毫无意义；产品差别微不足道时，
    好名字意味着数百万美元的销售差距。
  tags: [mennen, naming, meaningless]
  origin: [B-xb16]

- id: e23
  title: 健怡可乐扼杀Tab
  type: counter_example
  source_chapter: 第9章
  source_quote: |
    "公司只把天冬甜素用在健怡可乐里，这样做恰恰把Tab这个品牌送上了绝路。"
  summary: |
    可口可乐已有销量领先低糖百事32%的低热量品牌Tab，却推出含义过于露骨的健怡可乐（Diet Coke），
    自相残杀且销售下滑，把Tab送上绝路。教训：拥有领导地位时不要用延伸产品攻击自己的定位；
    低热量命名过分暴露好处反把顾客赶跑（对比"每次必喝的Tab"的坦然）。
  tags: [diet-coke, tab, cocacola]
  origin: [B-xb17]

- id: e24
  title: 大陆集团与大陆公司混淆
  type: counter_example
  source_chapter: 第9章
  source_quote: |
    "企业为什么要放弃'罐头'和'保险'这两个词，却喜欢用'集团'和'公司'这两个不说明问题的词呢？"
  summary: |
    价值39亿美元的"大陆集团"（罐头）与31亿美元的"大陆公司"（保险）互相混淆，曼哈顿电话簿里有235个
    带"大陆"的名称。教训：放弃说明业务的词、追求中性"集团/公司"之名无法建立身份；两家最终都失去
    独立地位，大陆集团还得改回"大陆罐头"。
  tags: [continental, naming, confusion]
  origin: [B-xb18]

- id: e25
  title: 首字母缩写陷阱
  type: counter_example
  source_chapter: 第10章
  source_quote: |
    "该公司找了一条简便的出路，把自己的名字改成USM公司，从此以后便在市场上销声匿迹了。"
  summary: |
    为逃避过时旧名或追求"现代感"而启用缩写的公司大多消亡：联合鞋业机器→USM销声匿迹，
    史密斯-科罗纳-马钱特→SCM、玉米产品→CPC同样失去市场存在感——人们记不住缩写背后是什么。
    GAF谐音gaffe（失态）；环球航空TWA广告费年3000万美元高于美航、联航，愿意选择的旅客却只有对手一半，
    1992年申请破产。教训：缩写不是逃逸旧名的捷径，既无含义又可能带负面谐音，靠广告费堆不出缩写的含义；
    只有广为人知之后缩写才有意义，颠倒因果则加速遗忘。
  tags: [abbreviation, naming, failure]
  origin: [B-xb19, B-xb20]

- id: e26
  title: 欧文斯-康宁改错名字
  type: counter_example
  source_chapter: 第9章
  source_quote: |
    "1992年，欧文斯-康宁玻璃纤维公司接受我们的建议，给公司换了个名字。不幸的是，他们用的新名字恰好和我们的建议相反。"
  summary: |
    公司接受了"应该改名"的建议，却去掉最有价值的"玻璃纤维"、改成不说明业务的"欧文斯-康宁公司"。
    教训：改名的关键是把名字与顾客购买的理由（品类词）连接，去掉品类词的改名比不改更糟。
  tags: [owens-corning, renaming, category]
  origin: [B-xb21]

- id: e27
  title: 由内而外的思维
  type: counter_example
  source_chapter: 第12章
  source_quote: |
    "这纯粹是明确而又固执的由内而外的思维结果，大体可以描述如下：'我们生产的Dial牌肥皂是市场上销量最大的洗衣皂。顾客一看到Dial牌除味剂就知道它很了不起'"
  summary: |
    决策从公司内部视角出发——"我们的顾客信任我们、会跟着买我们的延伸产品"，逻辑全部成立，结果全部失败
    （Dial除味剂份额极小、"不含阿司匹林的拜耳"、JC彭尼电池均如此）。关键句式识别：决策理由中出现
    "我们的名字顾客都知道/用我们的名字他们更容易接受"，即为由内而外。它是搭便车与品牌延伸决策的共同病根
    （第12章："由内而外的思维方式是通往成功的最大障碍"）。纠正工具：由外而内，先问名字在顾客心智中代表什么。
  tags: [inside-out, mindset, failure-pattern]
  origin: [C-cx01]

- id: e28
  title: 品牌延伸短期像兴奋剂
  type: counter_example
  source_chapter: 第13章
  source_quote: |
    "酒精是一种兴奋剂还是抑制剂？在短时间里，酒精是兴奋剂，从长期来看，它是一种抑制剂。品牌延伸的作用与酒精基本相同。"
  summary: |
    品牌延伸靠短期数据自我强化——延伸名与原名有联系（"啊，对，无糖可口可乐"），上市初期销量猛增、
    零售商被迫进货，前6个月业绩可观；但一旦没有再次订购，情况急转直下。短期优势正是它持续流行的原因，
    也是它最危险之处：用短期销售数据验证长期战略，样本本身就是错的。
  tags: [brand-extension, short-term, alcohol-metaphor]
  origin: [C-cx02]

- id: e29
  title: 名字是橡皮筋
  type: counter_example
  source_chapter: 第13章
  source_quote: |
    "它可以拉长，但不能超出某个极限。此外，你把名字延伸得越长，它就变得越脆弱（这也许与你想象的恰好相反）。"
  summary: |
    把名字当无限弹性的资产反复拉伸（产品线拉长、品类拉远、档次拉高拉低），每个延伸都在拉长橡皮筋，
    拉得越长越脆弱——与直觉相反。判据：既看经济学（单一品类多品种共用名字未必不划算），
    也看判断力（对手是否专注、定位是否重要）；都乐若延伸做香蕉，菠萝这头就会弹回来。
  tags: [rubber-band, naming, elasticity]
  origin: [C-cx03]

- id: e30
  title: 自己放弃地位最悲惨
  type: counter_example
  source_chapter: 第11章
  source_quote: |
    "要是有人企图抢占你的地位，那就够糟糕的了。要是你自己放弃了它，那就太悲惨了。"
  summary: |
    品牌地位最大的威胁不是对手，而是持有者自己把它让出去。施乐不仅是名字，而是与舒洁、亨氏、凯迪拉克一样
    "有着巨大、长远价值的地位"；施乐拿它去做计算机、亨氏拿它去做番茄沙司（泡菜第一让给Vlasic），
    都是自己松开跷跷板的一头。教训：评估任何延伸动作时，先计算将让渡的地位价值。
  tags: [position, self-sabotage, see-saw]
  origin: [C-cx04]

- id: e31
  title: 品牌延伸症：潜伏多年、掏空成空壳
  type: counter_example
  source_chapter: 第13章
  source_quote: |
    "品牌延伸之所以祸害无穷，是因为这种疾病潜伏好多年才会发作，是一个缓慢而不易被发现的过程。"
  summary: |
    延伸的恶果不在当期报表上：舒立滋低度啤酒、Pall Mall超柔型、杰根斯特干燥这类名字进入和退出心智都不费力，
    "来得快，去得也快"，等份额下滑显现时定位已被侵蚀多年、回天乏术。病理比喻：品牌像过度膨胀的星球，
    靠不断延伸把"营销体积"越做越大，心智中的含义却被掏空——规模巨大却不堪一击，如燃烧殆尽的空壳。
    观测样本：Scott从卫生纸第一跌到第三；卡夫"什么都是，又什么也不是"，在任何品类都不是头号品牌。
    教训：不能用延伸产品前几年的销售数据判断延伸成败。
  tags: [brand-extension, latency, dilution]
  origin: [C-cx05, C-cx06]

- id: e32
  title: 沃尔沃：四个定位加在一起不比一个强
  type: counter_example
  source_chapter: 第13章
  source_quote: |
    "功能越多越好玩这一点并不适用于定位。四个定位加在一起不比一个强。"
  summary: |
    认为把多个好属性叠加会更有竞争力是错觉。沃尔沃放弃豪华、速度、可靠性，只强调"安全"一个词时销量上升
    （年销40万辆）；后来叠加豪华、跑车、保安车、两用车，成为"可靠、豪华、安全、开起来很好玩"的车，
    销量随即下降。对照：宝马坚持"终极驾驶机器"单一概念则成功。教训：产品功能可以叠加，心智定位不能叠加。
  tags: [volvo, concept-stacking, single-position]
  origin: [C-cx08]

- id: e33
  title: 在错误的对象上做精细定位
  type: counter_example
  source_chapter: 第15章
  source_quote: |
    "它实施的是传统的航空公司战略：宣传食品和服务。……世界上所有的美食也不会吸引你去乘坐不飞往你目的地的航班。"
  summary: |
    比利时航空的问题是"没人要去比利时"（国家在心智的国家阶梯上位居倒数几层），它却效仿同行宣传美食与服务。
    教训：当需求侧的根子（心智中的位置）没解决时，供给侧任何卖点都不成立；定位要诊断真正的问题所在，
    而非在错误的对象上做精细定位。
  tags: [sabena, misdirected-positioning, airline]
  origin: [C-cx09]

- id: e34
  title: 本地人看不见自己的资产
  type: counter_example
  source_chapter: 第15章
  source_quote: |
    "你如果走进全欧洲最漂亮的广场—四面金碧辉煌的大广场（The Grand Place），会发现广场的整个中央地带竟然是停车场"
  summary: |
    本地人对自家资产的认知与外来者完全错位：比利时人自认不是旅游胜地（布鲁塞尔机场标牌自曝"每年220天下雨"），
    全欧洲最漂亮的大广场中央被当成停车场；纽约人看不见自由女神像，游客却年年来1600万。
    教训：定位资产要以外来者（潜在顾客）的眼睛盘点；本地人视角的战略（转机便利）恰恰是最差方案。
  tags: [perception-gap, tourism, grand-place]
  origin: [C-cx10]

- id: e35
  title: 半途换人毁掉定位项目
  type: counter_example
  source_chapter: 第15章
  source_quote: |
    "上述的电视节目正在制作时，比利时航空公司内部发生了人事结构变化。新的管理层对该项目并不热心"
  summary: |
    定位项目败于组织而非战略：比利时项目电视片制作中管理层更迭，新班子不热心，总部要求"通往欧洲的门户"
    战略时立即默许；旅游局出于政治原因要求塞进非三星级城市。教训：全员必须对战斗目标有统一认识，
    负责人不长期投入、抗拒不了复杂化压力，再好的定位概念也会搁浅；"美丽的比利时"本可成为有力的旅游定位。
  tags: [organization, persistence, sabena]
  origin: [C-cx11]

- id: e36
  title: 董事长否决"大嘴"：战略死于个人好恶
  type: counter_example
  source_chapter: 第16章
  source_quote: |
    "可惜的是，该公司的董事长不喜欢大嘴这个形象，竟然把这个项目取消了。"
  summary: |
    奶球"耐吃"定位的电视广告已扭转销量下滑并创下销售纪录，却因董事长个人不喜欢"大嘴"形象被取消，
    奶球"又回到了电影院里"。教训：定位决策被内部审美而非心智事实支配，是"自我导向"压倒"他人导向"的
    微缩样本；定位方案要预先解决向最高管理层推销的问题。
  tags: [internal-politics, ego, failure]
  origin: [D-fx01]

- id: e37
  title: "快速信件"：销量涨了，心智反而失守
  type: counter_example
  source_chapter: 第17章
  source_quote: |
    "在宣传快速信件的城市里，对邮递电报的认识程度实际上反而下降了。从27%降到了25%。"
  summary: |
    与"低价电报"对照的失败候选：快速信件定位在13周试销后，认识度从27%降到25%，业务增长只来自
    已有认知者的提醒式复购，缺乏可持续性。教训：当期销量可以掩盖心智建设的失败；验证定位必须同时测量
    销量与认识度，且以认识度趋势为长期判据。
  tags: [test-market, metrics, failure]
  origin: [D-fx02]

- id: e38
  title: 西部联盟拒绝更名Westar，终至破产
  type: counter_example
  source_chapter: 第17章
  source_quote: |
    "后来，我们拼命劝说西部联盟更名为Westar公司，他们拒绝了。再后来，他们就破产了。"
  summary: |
    咨询方力劝西部联盟趁邮递电报业务上升期把公司更名为Westar，被拒绝，公司最终破产。
    教训：当公司名承载的旧认知（老式电报）与新业务方向冲突时，拒绝换"容器"（名字）等于押注旧认知永生；
    改个名字有时真有用。
  tags: [naming, legacy-brand, failure]
  origin: [D-fx03]

- id: e39
  title: 组织拒绝显而易见的方案
  type: counter_example
  source_chapter: 第19章
  source_quote: |
    "人们倾向于崇尚复杂的东西、不屑于显而易见的东西，认为它们太简单了。"
  summary: |
    "福音教师"定位方案对天主教会有完整的诊断、圣经依据与实施路径，却因主教们认为"过于显而易见"而
    全盘被拒，结果毫无结果；许多教士反而推崇杜勒斯"教会要扮演六种角色"的复杂定义——全面却无法在心智中
    存储（多概念定义的传播力为零）。教训：定位工作寻找的正是显而易见的东西，但组织决策者崇尚复杂、不屑简单；
    再正确的方案，绕不过"向内推销"这一关就等于零。
  tags: [obviousness, complexity, adoption-failure]
  origin: [D-fx05, D-fx06]

- id: e40
  title: 劳斯莱斯思维方式
  type: counter_example
  source_chapter: 第22章
  source_quote: |
    "这种情况也许能称做是'劳斯莱斯思维方式'。'我们是本行业里的'劳斯莱斯''，这话在当下的商界里经常能听到。"
  summary: |
    以成为"行业里的劳斯莱斯"为荣的定位观：劳斯莱斯每年只卖几千辆，凯迪拉克年销近50万辆——都是豪华车，
    市场却天壤之别。定位上成功了（独一无二），销售上却失败了（需求狭小）。
    教训：独一无二的定位必须与较大的市场需求平衡，孤高定位是自嗨。
  tags: [niche-error, balance, failure]
  origin: [D-fx07]

- id: e41
  title: "我们有最好的员工"错觉
  type: counter_example
  source_chapter: 第22章
  source_quote: |
    ""我们有最好的员工"很可能是所有错觉当中最大的一个。"
  summary: |
    相信一对一比较中本公司员工强于对手，是他人导向营销人很快摆脱的错觉。事实是单个士兵战斗力差别不大，
    人数一多固有能力就持平；除非以数量换质量的高工资（未必是优势），雇几百人的公司平均能力与对手不会有差别，
    胜负取决于将军（战略）而非士兵。教训：以人的因素为成功关键的信念，是回避战略思考的遮羞布。
  tags: [talent-myth, strategy, illusion]
  origin: [D-fx10]

- id: e42
  title: 小弗兰克·西纳特拉：个人版品牌延伸
  type: counter_example
  source_chapter: 第20章
  source_quote: |
    "听到小弗兰克・西纳特拉这个名字，听众会想：'他不会像他父亲唱得那样好。'"
  summary: |
    "小"字辈名字在入行时就带来两次打击：听众先入为主认定小弗兰克·西纳特拉不如父亲，他果然唱得不行；
    小威尔·罗杰斯同样无助于自己。对照莉莎·米奈丽弃用母亲的姓（迦兰）反而声名超过母亲。
    教训：依附强势名字是个人版品牌延伸——借来的预期同时是枷锁，独立形象必须从独立名字开始。
  tags: [brand-extension, naming, personal-brand]
  origin: [D-fx13]

- id: e43
  title: "我是达拉斯最好的律师"：自我定义的泡沫
  type: counter_example
  source_chapter: 第20章
  source_quote: |
    ""我是达拉斯最好的律师。"是吗？假如我们在达拉斯法律界做一次调查，你的名字会被提到多少次？"
  summary: |
    大多数人没有信心为自己确立一个概念，犹豫不决、指望别人给自己下定义；敢于自我标榜者又常把内心认定
    当心智事实——"是吗？假如我们在达拉斯法律界做一次调查，你的名字会被提到多少次？"
    教训：个人定位与产品定位同律，你的定位不在自我评价里，而在他人心智中能被验证的位置里；
    两头都不做的人，就交由市场随意定义。
  tags: [self-definition, personal-brand, illusion]
  origin: [D-fx14]

- id: e44
  title: 麦克斯·凯里被遗忘：不敢犯错者的下场
  type: counter_example
  source_chapter: 第20章
  source_quote: |
    "人们至今还记得泰・科布（Ty Cobb），他偷垒134次，成功了96次（70%的成功率），却忘了麦克斯・凯里（Max Carey），此人在53次偷垒中成功了51次（成功率高达96%）。"
  summary: |
    成功率96%的麦克斯·凯里无人记得，成功率70%的泰·科布名垂青史。教训：只做有把握之事的完美主义者，
    名声反不如屡败屡试者；害怕失败的人用"尽善尽美"为拖延辩护，结果是永远做不成。
    值得做的事值得一试，错误是定位试错的入场费。
  tags: [risk-aversion, reputation, career]
  origin: [D-fx15]

- id: e45
  title: 战略贴在广告背面：把设计图用反了
  type: counter_example
  source_chapter: 第22章
  source_quote: |
    "可是，广告应该简单到它自身就是战略的程度。这家广告公司犯了一个错误：它把设计图用反了。"
  summary: |
    某广告公司老板要求把营销战略贴在每份广告设计的背面，客户问广告目的时翻过来念。
    教训：广告应简单到自身就是战略；战略若不能内化为显而易见的表达，说明战略还不够简单——
    复杂战略配创意执行，最终只剩创意没有战略。
  tags: [simplicity, execution, failure]
  origin: [D-fx16]
```

### 去重统计

- 原始条目：57 条（scannerA 8 条、scannerB 21 条、scannerC 12 条、scannerD 16 条）
- 合并后：45 条（e01–e45）
- 合并组共 8 组（20 条 → 8 条）：
  1. 「我能行」精神 + 自我导向型营销人：A-ce02 + D-fx09 → e02
  2. 米狮龙偏离定位（第3、7章同一品牌同一教训）：A-ce06 + B-xb05 → e06
  3. 正面进攻领导者（NCR/DEC/布利斯特-麦尔斯）：A-ce07 + B-xb11 + D-fx12 → e07
  4. 多元化陷阱（施乐/ITT/胜家等，含"万物恒变"错觉）：B-xb03 + C-cx12 + D-fx08 + D-fx11 → e11
  5. 满足所有人需求陷阱（定义+雪佛兰/麦凯恩+Rheingold）：B-xb10 + C-cx07 + D-fx04 → e17
  6. 首字母缩写陷阱（USM/SCM/CPC + GAF/TWA）：B-xb19 + B-xb20 → e25
  7. 品牌延伸症潜伏/空壳（晚期品牌延伸症两喻）：C-cx05 + C-cx06 → e31
  8. 组织拒绝显而易见方案（主教拒方案 + 六角色复杂定义）：D-fx05 + D-fx06 → e39
- 保留为独立条目的近邻主题（失败场景不同，未合并）：FWMTS 总陷阱（e01）与其各实例——米狮龙（e06）、Aim（e14）、喜力停止宣传（e09）、红牌退缩（e19）、自己放弃地位（e30）；技术陷阱（e16）、工厂空位（e15）、命名混乱家族（e04/e21/e22/e24/e25/e26/e38）等。
