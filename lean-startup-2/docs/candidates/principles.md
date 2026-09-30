# 候选清单：原则（principle-extractor 产出）

> 提取器视角：原则 / 清单 / 规则 / 断言。串行降级模式执行。出处标注章节 + 行号。

```yaml
- id: p01
  title: 精益创业 2.0 五条指导原则
  type: principle
  source_chapter: 引言（行 273-283）
  source_quote: |
    "1.持续创新……2.作为一个基本工作单元的创业团队……3.设立缺失的部门……4.二次创业……
    5.持续转型：改写组织基因，应对新的、多样化的挑战的能力。仅仅转型一次是远远不够的。"
  summary: |
    全书的公理层：持续创新靠的是全层级持续产出而非一次性豪赌；创业团队是需要特殊组织
    结构支持的基本工作单元；要有一个与财务部并列的创业部；对组织结构的根本变革等于
    再次创业；转型的目标状态是能反复转型。后续一切机制（创业部、增长委员会、创新核算）
    都是这五条的展开。
  tags: [principle, axiom, book-framework]
```

```yaml
- id: p02
  title: 先价值后增长
  type: principle
  source_chapter: 第 4 章（行 1339-1341）
  source_quote: |
    "我会建议团队一开始先决定价值假设，再考虑增长假设。先保证有少量的用户需要你提供的产品
    或服务，再考虑扩大规模，这样比较恰当。"
  summary: |
    排序规则：在少量真实用户确认"用了会开心、愿意付出稀缺物"之前，任何获客投入都是浪费。
    适用于产品、内部服务、活动策划。对应反例：增长先行的团队把资源烧在不被需要的产品上。
  tags: [principle, sequencing, validation]
```

```yaml
- id: p03
  title: 假设越少越好，聚焦风险最大者
  type: principle
  source_chapter: 第 4 章（行 1318-1324）
  source_quote: |
    "必须想方设法避免分析瘫痪，一般来说，关注的假设越少越好，而不是越多越好
    （我合作过的一个团队，仅针对一个项目就想出了 100 多个假设）。"
  summary: |
    列假设清单时做减法：只测风险最大、与当下关系最近的假设；遥远的未来假设
    （行业趋势、多年路线图）可记录但不优先。判断依据：我们最不了解、最不舒服的环境
    恰恰是最需要测试的地方。
  tags: [principle, focus, anti-analysis-paralysis]
```

```yaml
- id: p04
  title: 看行为不看口头（显示性偏好）
  type: principle
  source_chapter: 第 4 章（行 1257-1259）
  source_quote: |
    "不要问用户有什么需求，而是要设计实验，从实验中观察他们的需求。"
  summary: |
    访谈、焦点小组、问卷都不算实验：人们以为自己知道自己要什么，结果往往不是。
    规则：把问题改造成能产生行为数据的实验（纸板样机、预售、试用选择），
    用显示性偏好代替表达性偏好。大学记分卡"没人愿意比较大学"即此规则的产物。
  tags: [principle, user-research, revealed-preference]
```

```yaml
- id: p05
  title: 优化 MVP 是为了学习，不是为了扩大规模
  type: principle
  source_chapter: 第 4 章（行 1374）
  source_quote: |
    "优化最小化可行产品是为了学习，不是为了扩大规模。这个道理有些人很难接受，因为他们
    一辈子都在为了生产而生产，不是为了学习而生产。"
  summary: |
    MVP 的评价标准是单位成本换来的学习量，不是完成度或可扩展性。
    判别规则："你可以定义什么是最小化，但什么可行得由用户说了算。"
    反向应用：凡以"规模/健壮性"理由加码 MVP 的，先问它增加了什么学习。
  tags: [principle, mvp, learning-vs-execution]
```

```yaml
- id: p06
  title: 领导者两问："你学到了什么？你是怎么知道的？"
  type: principle
  source_chapter: 第 4 章（行 1570-1575）
  source_quote: |
    "领导者要问的最重要的问题是：1.你学到了什么？2.你是怎么知道的？"
  summary: |
    领导者面对坏消息/偏离计划时的标准动作：先问学到了什么、怎么知道的，
    而不是"为什么没做到"。它把问责对象从"执行者"转到"假设"，
    适用于上下级、亲子、任何"计划遭遇现实"的对话。案例：高管把业绩电话按此重构。
  tags: [principle, leadership, questioning, learning-culture]
```

```yaml
- id: p07
  title: 提前排期转型/坚持会议
  type: principle
  source_chapter: 第 4 章（行 1519-1521）
  source_quote: |
    "如果我们早就知道公司必须转型，为什么要等到最后一分钟才考虑这个问题？
    我建议：提前安排关于转型还是坚持的会议。把它列入公司日程。"
  summary: |
    规则：转型讨论应发生在还有余力的时候，而不是房顶着火、明天见董事会的绝境。
    节奏约束：约一个半月一次，一月不超过一次、一季度不少于一次。
    开会≠承认失败，只是问"有什么证据证明目前策略让我们更接近愿景"。
  tags: [principle, cadence, decision-hygiene]
```

```yaml
- id: p08
  title: 公开创新，不偷偷摸摸
  type: principle
  source_chapter: 第 6 章（行 2291）
  source_quote: |
    "'要保护创业团队不受居心不良的母公司伤害'，这其实是一种落后的思想……
    偷偷摸摸搞创新很少能传来捷报。要想实现整个公司的转型改造，唯一的办法就是公开创新。"
  summary: |
    规则：内部实验必须公开透明地置于高层视野内（实验严谨+无极端责任风险），
    依靠特事特办与支持者清障，而不是玩地下项目。
    例外张力：马汉冰箱案显示"转入地下"有时是项目存活的实际路径——
    但作者将其解释为"公开争取到支持者"后的胜利，地下只是过渡。
  tags: [principle, transparency, politics]
```

```yaml
- id: p09
  title: 只要有一个团队成功就是胜利
  type: principle
  source_chapter: 第 6 章（行 2131）
  source_quote: |
    "我说：'恕我直言，只要有一个团队成功就是胜利。'对企业来说，要求 100% 的成功率
    会带来很大的压力。这种思维跟创业思维也是背道而驰的。"
  summary: |
    对试点组合的期望管理规则：第一批试点要按组合评估（有失败是常态），
    高层若要求全胜，团队就会表演成功、隐藏失败。与"僵尸项目"治理互为镜像：
    既要容忍失败，又要诚实终止。
  tags: [principle, portfolio, expectation-setting]
```

```yaml
- id: p10
  title: 跨职能团队必须专职
  type: principle
  source_chapter: 第 6 章（行 2075-2084）
  source_quote: |
    "要说服领导者不只是建立一个真正的跨职能团队，而且要团队成员专职投入，
    这是我在和很多家公司打交道时常常碰到的一大难题。"
  summary: |
    规则：创业团队成员必须全职投入（或自愿的义务投入），职能没有正式代表时宁可请
    "义工"坐进团队（设计师搬桌子案例），也不要让兼职委员会凑数。
    补充：业务/销售人员应在早期加入团队（西班牙电信经验），保证商业化时"产品跟自己有关"。
  tags: [principle, team-design, cross-functional]
```

```yaml
- id: p11
  title: 培训要覆盖"能喊停的人"
  type: principle
  source_chapter: 第 7 章（行 2627-2633）
  source_quote: |
    "公司某些职能部门可以叫停。如果你是一个职能部门的负责人，你可以说，'我们没有预算'
    或者'我担心不合规'……你还要制止那些妨碍这项运动的人。"
  summary: |
    培训对象规则：只培训实践者不够，必须把法务、财务、HR、IT 等拥有否决权的部门负责人
    拉进同一间教室，否则团队学到的新方法会在下一个审批口被原制度击毙。
  tags: [principle, training, stakeholder-coverage]
```

```yaml
- id: p12
  title: 教练立场："假定你们是对的，我是错的"
  type: principle
  source_chapter: 第 7 章（行 2658-2676）
  source_quote: |
    "我始终告诉参加培训的团队：对于你们的计划，我将假定你们是对的，我是错的。
    我们来设计实验证实这一点。"
  summary: |
    说服固执团队的方法：不要求他们"走出去和用户交流"，而是帮他们设计一个
    能证明自己正确的实验（预测封入信封→展会后开箱）。
    让现实而非教练完成说服；额外好处——有时团队真的是对的。
  tags: [principle, coaching, persuasion, experiment-design]
```

```yaml
- id: p13
  title: 没有制约的创新不是好创新
  type: principle
  source_chapter: 第 7 章（行 2777）、第 2 章（行 849）
  source_quote: |
    "没有制约的创新不是好的创新——资金过剩的项目往往有很高的创业死亡率。"
  summary: |
    自觉设置约束（人、钱、时间盒："钱只够一个半月"）是创业方法的一部分而非敌人：
    稀缺强迫专注、暴露真实优先级、对抗范围蔓延。组织给创新团队的不是越多越好，
    而是有限但可靠的资源+严格的下轮门槛。
  tags: [principle, constraints, resource-discipline]
```

```yaml
- id: p14
  title: 审计对照过去，不对照梦想计划
  type: principle
  source_chapter: 第 9 章（行 3629）
  source_quote: |
    "审计的关键不是拿临时进展（通常没什么起色）跟商业案例中的梦想计划比较，
    而是跟前面取得的成绩比较。这样就能体现团队在一段时期内的进步。"
  summary: |
    创新项目评估基准规则：用"环比学习进步"而非"对照最初预测"做审计，
    否则所有早期项目都注定看起来失败。配套：早期团队只需 3-5 个学习指标的仪表板，
    投资额越大才要求越完整的商业案例。
  tags: [principle, audit, evaluation-baseline]
```

```yaml
- id: p15
  title: 增长委员会铁律：不能证明学习就不再拨款
  type: principle
  source_chapter: 第 9 章（行 3692）
  source_quote: |
    "增长委员会必须有一条不可撼动的原则：如果钱给了你却不能证明你在进行验证式学习，
    就休想再拿一分钱。"
  summary: |
    里程碑拨款的执行底线：续命条件不是进度、不是故事、不是关系，而是可审计的验证式学习。
    针对两类失败：团队的不撞南墙不回头，和高管"心软+被巧舌下属说服"反复花冤枉钱。
  tags: [principle, funding, accountability]
```

```yaml
- id: p16
  title: 教练不是领导，也不是间谍
  type: principle
  source_chapter: 第 7 章（行 2680、2646-2648）
  source_quote: |
    "顾问起的是教练的作用，他不是间谍，不是领导，不是主管，更不可能取代董事会成员。"
  summary: |
    内部教练的角色边界：提供方法与实验设计，不掌握人事权、不向上汇报团队隐私、
    不替代决策。教练本身需要被严格培训、被视为正式岗位（否则出现教练流失、
    积极者离职、特长片面三种病）。
  tags: [principle, coaching, role-boundary]
```

```yaml
- id: p17
  title: 用本公司语言重述方法，不照搬复制
  type: principle
  source_chapter: 第 6 章（行 2338-2341）
  source_quote: |
    "'我们问：我们能复制什么？'该怎么回答？第一句话我总是说：'你无法复制。你们要自己做
    实验，把所有做法用到自己的流程中。'"
  summary: |
    移植规则：FastWorks/Design for Delight/USDS 各不相同，因为它们反映母组织的文化与性格；
    学习者应把外部方法当实验材料改造为本公司的语言与工具（丰田连"精益生产"都不叫），
    而不是购买咨询模板直接套用。
  tags: [principle, adaptation, localization]
```

```yaml
- id: p18
  title: 大处着眼，小处着手，迅速扩大
  type: principle
  source_chapter: 第 3 章卷首语（行 925）、第 1 章（行 619）
  source_quote: |
    "这些团队的口号是：'大处着眼，小处着手，迅速扩大。'"
  summary: |
    愿景与行动的耦合规则：以宏大愿景定向（否则无法判断转型方向），
    以最小实验起步（控制每次下注），验证后快速加注（给胜利者下双倍赌注）。
    它同时否定了两种病：没有愿景的小步乱试，和只有愿景的大项目豪赌。
  tags: [principle, strategy, scaling]
```

```yaml
- id: p19
  title: 奖励有益的失败，让项目由创业者自己终止
  type: principle
  source_chapter: 第 1、4、5 章（行 649-651、1561、1749-1751）
  source_quote: |
    "现代企业奖励有益的失败，这种失败能让公司明智地改变方向，为公司提供有用信息。"
  summary: |
    制度规则：终止项目的叙述权应属于创业者本人（"项目失败由项目创始人负责"），
    及时证伪的团队应被奖励（液体膨胀机团队获全员奖励与公开表扬）；
    反之，靠中层当"刽子手"砍项目会催生红绿灯表演与项目僵尸化。
  tags: [principle, failure, accountability, incentives]
```

```yaml
- id: p20
  title: 技术只是手段：先改行为与文化，再上工具
  type: principle
  source_chapter: 第 8 章（行 3131-3137）
  source_quote: |
    "我们不再把技术当作绩效考核的中心，而是把技术仅仅当作推动绩效考核的手段。"
  summary: |
    规则：上线新工具（考核 app、协作软件、新系统）前先建立使用它的行为与文化环境，
    否则零反馈（PD@GE 两周实验教训）。检验顺序：小群体行为实验→证明行为改变→
    再迭代工具并扩大。
  tags: [principle, tools-vs-culture, sequencing]
```

```yaml
- id: p21
  title: 自愿参加是领先性指标
  type: principle
  source_chapter: 第 8 章（行 3151）
  source_quote: |
    "参不参与不强迫。各部门的新系统测试采取自愿原则。事实上，很多部门自愿参加测试，
    这本身就是一个成功的领先性指标。"
  summary: |
    推广新工作法/新系统时，把"自愿加入率"当作制度质量的测量仪：
    强制推广测不出真实需求（对应跳过关键问题的 IT 推广反例），
    自愿流入证明价值主张成立。日常 FastWorks 3 万人报名为正面案例。
  tags: [principle, adoption, metrics, voluntariness]
```

```yaml
- id: p22
  title: 过早触及深层机制等于自杀
  type: principle
  source_chapter: 第 8 章（行 2913）
  source_quote: |
    "过早触及公司深层机制等于自杀。只有在第一、第二阶段的工作中赢得了足够的政治资本、
    有了足够的成绩，负责人才可以触及深层机制。"
  summary: |
    变革时序铁律：改薪酬、考核、预算等深层制度前，必须先用边缘成功积累政治资本；
    反之，没有成绩背书的制度挑战会招致联合反攻。对应反面：回部门后"格格不入"
    （只培训个人、不改文化时组织会排异）。
  tags: [principle, timing, political-capital, sequencing]
```

```yaml
- id: p23
  title: 创业方法适用于非创业工作
  type: principle
  source_chapter: 第 2 章（行 792-798）、第 8 章（行 3303-3308）
  source_quote: |
    "他们只是粗略地接受过精益创业培训，后来把精益的一些技巧用于看似微不足道的项目上，
    比如帮老板做 PPT 这种不起眼的事，但是效果非常好。"
  summary: |
    规则：实验思维不只属于新产品团队——中等不确定性工作（内部提案、招聘、
    活动策划、PPT）同样可用。三大理由：工具在低不确定性下也有效；
    非创业者管理者必须理解这套语言；你无法预知谁是创业者（YC 经验）。
  tags: [principle, universal-applicability, culture]
```

```yaml
- id: p24
  title: 变革必须专人专责，不许放进权力真空
  type: principle
  source_chapter: 第 6 章（行 2344-2346）
  source_quote: |
    "坏方法不会自行修复。它们通常潜藏在权力真空中。一线员工无权变革，高层领导者对这些问题
    视而不见……安排专人负责很管用，即便不是领导，不是全职员工。"
  summary: |
    推动转型的组织规则：必须指名道姓地安排专人负责（森佩尔主动请缨全职负责 GE 转型），
    由内部人而非外部咨询公司驱动（"让外人推动组织变革注定会失败"）；
    无主的变革会在部门墙前自然死亡。
  tags: [principle, ownership, internal-change-agent]
```
