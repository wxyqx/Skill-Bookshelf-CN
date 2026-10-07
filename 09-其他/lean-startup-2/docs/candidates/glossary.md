# 候选清单：术语（glossary-extractor 产出）

> 提取器视角：作者反复使用/明确定义/用法异于常识的概念词。串行降级模式执行。
> 每条含 author_definition / key_distinction / why_it_matters 字段。

```yaml
- id: g01
  term: 创业管理（entrepreneurial management）
  type: term
  source_chapter: 第 5 章（行 1659）
  author_definition: |
    "创业管理是针对 21 世纪特有的不确定性的领导框架。创业管理不能代替传统管理。"
  key_distinction: |
    ≠ 创业公司专属的管理风格；≠ 灵活/扁平/自由。
    = 与一般管理并列的第二套严谨体制，专管极端不确定性；两者的组合即"组合式管理"。
  why_it_matters: |
    下游 skill 若把创业管理理解为"氛围轻松"，会漏掉其核心：责任制、核算、问责与
    一般管理同等严格。全书一切机制都建立在这一定义上。
  tags: [term, core-concept]
```

```yaml
- id: g02
  term: 创业部（缺失的部门）
  type: term
  source_chapter: 第 2 章（行 691-707）
  author_definition: |
    "监管公司的'创业基因'——将创业心智模式和技巧传达给公司全体员工，不断投资下一代创新。"
  key_distinction: |
    ≠ 创新实验室/研发部/臭鼬工厂（项目集合）；= 职能性部门（像财务部制定标准与流程，
    不直接替团队做资源决定），负责创业者培养、方法推广、把关政策留口。
  why_it_matters: |
    混淆两者会把"创业部"做成又一个创新秀场；作者明确反对"仅仅是再建一个创新实验室"。
  tags: [term, org-design]
```

```yaml
- id: g03
  term: 创业团队（基本工作单元）
  type: term
  source_chapter: 第 2 章（行 713-716）
  author_definition: |
    "内部创业团队必须同时拥有研发部门的科学精神与严谨性；销售与营销部门以用户为中心的
    原则；以及工程部门井然有序的规范。"
  key_distinction: |
    ≠ 临时项目组/跨部门委员会/特别工作组（兼职、无独立核算、无转型权）。
    = 专职、跨职能、把项目当实验、可申请转型、直接向增长委员会汇报的小团队。
  why_it_matters: |
    是否满足此定义决定该团队适用哪套问责（传统 vs 创新核算）；套错问责是 ce12 类失败的根源。
  tags: [term, team, core-concept]
```

```yaml
- id: g04
  term: 自由岛 / 沙盒
  type: term
  source_chapter: 第 2 章（行 842-849）
  author_definition: |
    "可以为这些预先设置的约束建造一个'自由岛'或'沙盒'，帮助自主团队开展实验，
    但不用他们承担全部责任。"
  key_distinction: |
    ≠ 无监管的特区（ce22 独角兽团队那种"给了钱没问责"正是反面）；
    = 带明确约束与责任标准的有限责任实验空间，约束本身是方法的一部分。
  why_it_matters: |
    "自由"与"问责"必须同时设计；只给自由的沙盒会演变成 ce22 的失败。
  tags: [term, governance]
```

```yaml
- id: g05
  term: 企业重力（Corporate Gravity）
  type: term
  source_chapter: 第 2 章（行 743）
  author_definition: |
    "企业重力依然在发挥作用：大多数初创项目组都面临资源稀缺的问题，在财务上会要求更严格。"
  key_distinction: |
    ≠ 修辞性的"组织惰性"；= 把一切项目拉回旧体制轨道的具体力量：旧预算规则、
    旧审批链、旧考核矩阵。它对内部团队往往比对独立公司更严（外部初创反而资源约束清晰）。
  why_it_matters: |
    用重力解释失败可避免把中层当坏人（ce07）：该改的是施加引力的制度。
  tags: [term, organizational-behavior]
```

```yaml
- id: g06
  term: 计量供资（milestone-based capital）
  type: term
  source_chapter: 第 3 章（行 1067-1075）
  author_definition: |
    "硅谷在降低风险方面采取的做法——计量供资（这跟常见的企业预算方法正好相反）。"
  key_distinction: |
    ≠ 预算拨付；= 风投式分轮注资：已拨之钱自由支配，下一轮取决于验证式学习；
    团队承担全部成本、资金天然稀缺。
  why_it_matters: |
    全书资金机制的原型；企业版落地即 g08 里程碑式资金拨付 + g16 增长委员会。
  tags: [term, funding, core-concept]
```

```yaml
- id: g07
  term: 按指定用途的资金拨付
  type: term
  source_chapter: 第 7 章（行 2769-2785）
  author_definition: |
    "这种体制我称为按指定用途的资金拨付……一旦上了台面，就成了大多数管理者所说的
    '水龙头'——不时有资金流出。"
  key_distinction: |
    = 年度预算制下项目立项即持续续命的体制；与 g06 恰为对偶。它产生延迟最优、
    继任者背锅、政治成本高三大副作用（ce11）。
  why_it_matters: |
    是作者认定的"根本"问题（"预算管理是根本"）；判断一个组织能否创新，
    先看它的钱怎么拨。
  tags: [term, funding]
```

```yaml
- id: g08
  term: 里程碑式资金拨付
  type: term
  source_chapter: 第 7、9 章（行 2787-2809、3688-3692）
  author_definition: |
    "里程碑式的资金拨付的原则是：钱你随便花，但要争取更多资金就必须达到极其严格的标准，
    关键是看你验证式学习的结果怎么样。"
  key_distinction: |
    ≠ 分阶段预算（阶段=日历时间）；= 阶段=学习里程碑。配七项好处与一条铁律
    （不能证明学习就休想再拿一分钱）。
  why_it_matters: |
    它是"给自由"与"防僵尸"的兼容解；企业转型第二阶段的标志物。
  tags: [term, funding, core-concept]
```

```yaml
- id: g09
  term: 领先性指标 / 虚荣指标
  type: term
  source_chapter: 第 3 章（行 1044-1050）
  author_definition: |
    "跟踪性指标（总收入、利润、投资回报率、市场份额等）不同于领先性指标（用户契合、
    满意度、单位经济效益、重复使用、转换率等），领先性指标可以预测公司未来是否成功。"
  key_distinction: |
    领先性=行为性、因果可指认、单位用户可比；虚荣=总量性、随投入自增、无法行动。
    转型期追加三个组织级领先指标：生产周期、用户关系变化、团队士气。
  why_it_matters: |
    指标选择错误时一切核算失效（ce05/ce15）；3A（可操作/可访问/可审计）是其质检标准。
  tags: [term, metrics, core-concept]
```

```yaml
- id: g10
  term: 信仰飞跃假设（leap-of-faith assumption）
  type: term
  source_chapter: 第 4 章（行 1252-1259）
  author_definition: |
    "在传统的商业计划书里，这些假设代表公司目前对未来的猜想……精益创业要求我们把假设
    一条条说清楚，这样才能尽早发现哪些是对的，哪些是错的。"
  key_distinction: |
    ≠ 一般风险清单；= 计划成立所"必须为真"的最小假设集，且当前无证据支撑。
    最优先的是那些最不舒服、最不了解的。
  why_it_matters: |
    "等一等"案例（c29）：假设不被显性化就会作为隐形前提运行两年。
  tags: [term, assumptions, core-concept]
```

```yaml
- id: g11
  term: 最小化可行产品（MVP）
  type: term
  source_chapter: 第 4 章（行 1359-1374）
  author_definition: |
    "最小化可行产品是新产品的早期模型，团队通过这个实验，可以对用户需求进行最大限度的
    验证式学习。"
  key_distinction: |
    ≠ 粗糙产品/内部演示/公测版。判断标准引大卫·布兰德："你可以定义什么是最小化，
    但什么'可行'得由用户说了算"——必须面对真实用户、产生行为数据、绑定假设。
  why_it_matters: |
    把 MVP 理解为"产品雏形"是业界最常见误读；它本质是实验载体（纸板手机、
    改标发动机、一页纸文件皆可）。
  tags: [term, mvp, core-concept]
```

```yaml
- id: g12
  term: 验证式学习（validated learning）
  type: term
  source_chapter: 第 4 章（行 1424-1441）
  author_definition: |
    "本来可以用那个简单网页了解（但实际上没有）的信息我们称为验证式学习。"
  key_distinction: |
    ≠ 学到的感想/调研结论；= 从真实用户行为变化中做出的科学推理，
    以"价值交换"（用户愿放弃的稀缺物）为锚，是初创公司的"进展单位"。
  why_it_matters: |
    它是创新核算的记账单位；增长委员会拨款铁律（f08）验证的就是它。
  tags: [term, learning, core-concept]
```

```yaml
- id: g13
  term: 价值假设 / 增长假设
  type: term
  source_chapter: 第 4 章（行 1337-1347）、第 9 章（行 3521-3538）
  author_definition: |
    "一个是价值假设，要验证一种产品或服务一旦为用户所用就能让他们开心；另一个是增长假设，
    要验证如果已经有了一些用户，怎样才能赢得更多用户。"
  key_distinction: |
    二者不可混测：价值看留存/重复使用/愿多付；增长看新用户是否源于老用户行为
    （黏性/付费/病毒三引擎）。顺序固定：先价值后增长。
  why_it_matters: |
    商业案例仪表板必须同时覆盖两者，缺增长面板是 L1 常见错误。
  tags: [term, assumptions]
```

```yaml
- id: g14
  term: 转型（pivot）
  type: term
  source_chapter: 第 4 章（行 1486-1511）
  author_definition: |
    "转型，愿景不变策略变。"
  key_distinction: |
    ≠ 放弃/推倒重来（愿景是不可讨价还价的部分）；≠ 无据漂移（每次转型生成一批
    新假设进入下一循环）。转型是主动的结构化调整，通常发生在预排期的会议上而非绝境。
  why_it_matters: |
    没有 vision 的团队无法 pivot（只会漂移）；转型/坚持会议节奏是防"最后一分钟
    才转型"的制度设计。
  tags: [term, core-concept, decision]
```

```yaml
- id: g15
  term: 创新核算制度（Innovation Accounting, IA）
  type: term
  source_chapter: 第 9 章（行 3414-3441）
  author_definition: |
    "创新核算制度（IA）是成熟企业衡量工作进度的方法，它能在传统指标……完全失效时发挥作用。"
  key_distinction: |
    ≠ "创新型会计"（作者特意撇清：那种会计会让人坐牢）；≠ 财务预测。
    = 把学习换算成美元的三层次体系（仪表板/商业案例/NPV）+ 创新场定位
    （0→IA 值→权益值→梦想计划）。
  why_it_matters: |
    它让财务从把关者变成建设者；同时其 NPV 层在非量化部门（HR/文化）的适用性
    是本书未证实的边界（见 BOOK_OVERVIEW 批判）。
  tags: [term, finance, core-concept]
```

```yaml
- id: g16
  term: 增长委员会（growth board / 增长委员会）
  type: term
  source_chapter: 第 9 章（行 3637-3706）
  author_definition: |
    "增长委员会就是纯粹的公司内部创业委员会……'增长委员会就是可运作的风险资本基金会。'"
  key_distinction: |
    ≠ 评审会/阶段门径（过关式、敌对式）；= 创业团队的唯一问责点 + 信息中央交换所 +
    里程碑拨款把关人，当场决策、以证据为据、不出席不投票。
  why_it_matters: |
    它同时解决 ce06（危机没收创新资源）、ce11（僵尸项目）、ce12（ROI 杀种子）三类失败。
  tags: [term, governance, core-concept]
```

```yaml
- id: g17
  term: 增长引擎（黏性/付费/病毒式）
  type: term
  source_chapter: 第 9 章（行 3530-3536）
  author_definition: |
    "可持续增长定律：新用户的增长源自老用户的行为。"
  key_distinction: |
    三引擎判据各异：黏性=口碑>流失；付费=用户收入可覆盖获客；病毒式=正常使用自带传播。
    "产品与市场匹配"不再是玄学，而是所选引擎下可计算的具体数字门槛。
  why_it_matters: |
    为"增长假设"提供量化工具；错配引擎（如用付费引擎逻辑做病毒式产品）会导致错误的
    匹配判断。
  tags: [term, growth]
```

```yaml
- id: g18
  term: 貌似合理的承诺（plausible promise）
  type: term
  source_chapter: 第 9 章（行 3377）
  author_definition: |
    "承诺你的项目会产生多大影响，要大到能引起投资人的兴趣，但也不能太大，
    让人以为你这个创业者异想天开。"
  key_distinction: |
    ≠ 说谎/夸大；= 融资叙事的校准艺术：数字要"不大不小刚刚好"（同一笔 2500 万美元
    新业务在不同公司眼里意义完全不同）。
  why_it_matters: |
    它解释了为什么学习必须可审计（ce19）：承诺层面的博弈无法靠诚信解决，
    只能靠创新核算改变信息结构。
  tags: [term, fundraising, narrative]
```

```yaml
- id: g19
  term: 创新期货 / 创新场
  type: term
  source_chapter: 第 9 章（行 3431-3439）
  author_definition: |
    "可以把初创公司或创新项目视为正式的金融工具，或者'创新期货'……0→现在的创新核算制度值
    →权益值→梦想计划。"
  key_distinction: |
    ≠ 期权/衍生品交易；= 把在投创新项目形式化为金融头寸的隐喻：IA 值是当前价格，
    学习推动其向"梦想计划"端移动；估值三变量=资产、成功概率、成功量级。
  why_it_matters: |
    为"给信息定价"提供概念接口；也提示组合层面可比性（油气集团的增长命题适配）。
  tags: [term, valuation]
```

```yaml
- id: g20
  term: 二次创业
  type: term
  source_chapter: 第 8 章（行 2869-2873）、第 10 章（行 3942）
  author_definition: |
    "二次创业是指公司发展的一个阶段，是公司从一个新组建的组织向持续发展的机构的转变。"
  key_distinction: |
    ≠ 再开一家公司；= 成熟组织为重建创业基因而进行的结构性再造；
    作者断言"公司转型——对公司现有结构进行彻底整治就是创业"，与初创是"一枚硬币的两面"。
  why_it_matters: |
    该词把组织转型纳入创业定义，是第 10 章"统一的创业理论"的枢纽。
  tags: [term, transformation, core-concept]
```

```yaml
- id: g21
  term: 把关部门 / 赋能部门
  type: term
  source_chapter: 第 8 章（行 2950-2953）
  author_definition: |
    "把关部门总是因为审查制度、官僚体制和僵化的规则降低其他部门的办事效率；
    而赋能部门则在帮助团队提高工作效率。"
  key_distinction: |
    区分标准不是部门名称而是运作方式：同一法务部可以是把关（默认禁止）
    也可以是赋能（预批参数+红黄绿清单）。转变路径=把本部门当创业团队经营。
  why_it_matters: |
    B 段边界来源：任何"流程改造"类 skill 都必须先诊断目标部门当前处于哪一侧。
  tags: [term, functional-transformation]
```

```yaml
- id: g22
  term: 高层发起人 / 高层支持者 / 教练（三层支持结构）
  type: term
  source_chapter: 第 6-7 章（行 2287-2295、2552、2646-2648）
  author_definition: |
    发起人=日常贴近团队、特事特办的清障者；支持者="保证那些有意变革的人有资源排除
    他们自己、他们的教练以及管理者都不能排除的障碍"；教练=非领导非间谍的方法顾问。
  key_distinction: |
    三角色不可互相替代：发起人保项目、支持者保工作法、教练保学习。
    常见错误是只有发起人（人走政息）或只有教练（无权清障）。
  why_it_matters: |
    内部创业者的生存结构图；设计转型时应按三层配齐并明确各自边界。
  tags: [term, sponsorship, roles]
```

```yaml
- id: g23
  term: 增长命题（growth thesis）
  type: term
  source_chapter: 第 9 章（行 3715-3721）
  author_definition: |
    "为每个组合列出增长命题，然后评估不同项目和命题的适配程度……要有一个增长命题——
    证明'这个项目与组合是否合适'。"
  key_distinction: |
    ≠ 项目商业案例（单项目层面）；= 组合层面的战略过滤器，回答"我们为什么投这类项目"。
    GE 油气集团在委员会议程实验失败后引入它。
  why_it_matters: |
    防止增长委员会退化为逐项目投票；是把风投模式嫁接到企业战略的关键中间层。
  tags: [term, portfolio, strategy]
```

```yaml
- id: g24
  term: 无代表权税收（taxation without representation）
  type: term
  source_chapter: 第 9 章（行 3808）
  author_definition: |
    "现有公司部门希望实施'无代表权税收'。他们通常希望掌控项目……但又不想投资。"
  key_distinction: |
    ≠ 普通部门摩擦；= 权责不对称的制度化：管控权与投入义务分离。
    是克里斯坦森创新者窘境在组织内部的具象化。
  why_it_matters: |
    诊断创新项目死因的快速检验：查它是否在"被管辖但无人出资"的状态。
  tags: [term, politics, governance]
```

```yaml
- id: g25
  term: 临界规模（critical mass）
  type: term
  source_chapter: 第 6 章（行 2020-2029）
  author_definition: |
    "然后，我们开始培训更多的团队。开始时一次培训 1 个，后来一次 4 个，再后来一次 8 个……
    这一临界规模最终在全公司引发了一系列变革反应。"
  key_distinction: |
    ≠ 全面铺开；= 覆盖足够多样的部门/区域/职能的最小试点组合，使"新方法在本机构可行"
    从主张变成内部证据。GE 用冰箱/婴儿培育箱/ERP/IT/HR 等异质团队达成。
  why_it_matters: |
    转型一阶段的完成判据；试点同质化（只挑友好部门）永远到不了临界。
  tags: [term, scaling, transformation]
```

```yaml
- id: g26
  term: 舞动宝剑（剑，the sword）
  type: term
  source_chapter: 第 6 章（行 2124-2129）
  author_definition: |
    "很多'无法解决的'问题只要用上我所谓的'宝剑'就能迎刃而解，因为一剑下去，
    官僚制度就会土崩瓦解。"
  key_distinction: |
    ≠ 高层滥用权威改流程；= 过堂会上团队与高层的条件交换：成果承诺换一次性清障
    （政策支持/专职人员/免干预），成本极低且把高层变成当事人。
  why_it_matters: |
    转型一阶段最被低估的杠杆；解释了为何试点团队"很少要钱，要的是清障"。
  tags: [term, executive-power, negotiation]
```

```yaml
- id: g27
  term: 宾果卡（bingo card）
  type: term
  source_chapter: 第 9 章（行 3587-3614）
  author_definition: |
    "显示了实验开展的情况，不仅涉及从团队到公司的三个不同范围，而且涉及项目进展的
    四个阶段：实施、行为变化、用户影响及财务影响。"
  key_distinction: |
    ≠ OKR/记分板（评估绩效）；= 聚焦工具与诊断矩阵：每格是下一格的领先性指标，
    用法是逐格问到不满意处、回退一格做变革。
  why_it_matters: |
    把创新核算从团队层扩展为组织层的通用问责语言；跳格使用会产生噪声结论（ce15）。
  tags: [term, metrics, diagnostic]
```

```yaml
- id: g28
  term: 职业资产净值（career equity）
  type: term
  source_chapter: 第 8 章（行 2911）
  author_definition: |
    "成功之后怎么办？大家不免会问一些问题，采用这种新工作法会对他们的职业资产净值
    ——绩效评估、晋升渠道、同行评价有何影响。"
  key_distinction: |
    ≠ 薪酬；= 员工在组织内积累的评估、晋升与声誉资产。新工作法若威胁这一净值，
    理性员工必然抵制（ce09 的深层原因）。
  why_it_matters: |
    提醒变革设计者：不调整考核与晋升就要求行为改变，等于要求员工自减资产。
  tags: [term, careers, incentives]
```

```yaml
- id: g29
  term: 作战室三规则（war room rules）
  type: term
  source_chapter: 第二部分引言（行 1830-1834）
  author_definition: |
    "规则 1：作战室和会议是用来解决问题的。规则 2：谁最了解情况谁发言，而不是谁的官大
    谁发言。规则 3：我们必须关注最紧急的问题。"
  key_distinction: |
    ≠ 一般敏捷站会模板；= 危机场景下的最小文化与流程规则集，第一条针对推卸责任、
    第二条针对层级发言权、第三条针对范围失焦。
  why_it_matters: |
    可迁移的危机管理微制度；医保网两个月逆转的直接治理工具。
  tags: [term, crisis, culture]
```

```yaml
- id: g30
  term: 交易日（trading day，花旗）
  type: term
  source_chapter: 第 9 章（行 3777-3781）
  author_definition: |
    "每个增长委员会每 6~8 周开一次会，开会当天被称为'交易日'……公司内部几乎每周都有
    交易日活动。"
  key_distinction: |
    ≠ 年度创新大赛；= 高频、常态化的内部资本集市：委员会当场拨小额资金继续/终止实验，
    无固定周期与固定额度，完全视项目进展。
  why_it_matters: |
    展示增长委员会在 GE 模式之外的另一种节拍；"验证费只需几千美元"是其可复制要点。
  tags: [term, governance, cadence]
```
