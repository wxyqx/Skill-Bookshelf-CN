# candidates/glossary.md — 术语提取器产出

> 提取器: glossary-extractor（串行降级执行，"干净视角"独立跑完：只找关键概念词典条目）
> 全书上下文: 见 BOOK_OVERVIEW.md；出处按 fulltext.txt 实际章节与行号标注。
> 本阶段不做筛选，宁错杀，交给阶段 1.5 三重验证。author_definition 尽量用书中原文；key_distinction 是最有价值字段。

```yaml
- id: g01
  term: 上瘾模型（Hook Model / 钓钩）
  type: term
  source_chapter: 前言（L176–216）；各章
  author_definition: |
    "一个供各大公司开发习惯养成类产品的四阶段模型……通过这个让用户对产品欲罢不能的
    连续循环模型，公司无须花费巨额广告费用……就能使用户在不知不觉中依赖上你的产品。"（L176）
  key_distinction: |
    ≠ "成瘾机制"：作者明确区分 hook（习惯）与 addiction（成瘾），模型目标是前者（L476）
    ≠ 运营增长漏斗：四阶段是循环而非线性漏斗，投入端回连触发端
    = 一个"将用户面临的问题与企业提供的应对策略衔接在一起"的设计闭环（L259）
  why_it_matters: |
    全书所有 skill 的总坐标系；若按字面理解成"让人上瘾的邪术"，下游所有单元的伦理定位
    与 B 段都会写错。
  tags: [term, core-concept]
```

```yaml
- id: g02
  term: 习惯（habit）
  type: term
  source_chapter: 前言（L136）；第1章（L289–299）
  author_definition: |
    "所谓习惯，就是一种'在情境暗示下产生的无意识行为'，是我们几乎不假思索就做出的举动。"（L136）
  key_distinction: |
    ≠ 爱好/忠诚/依赖：判据是"无意识"，不再是决策的结果
    ≠ 成瘾：习惯有好有坏，成瘾是长期被动依赖并走向自我毁灭（L476）
    = 大脑为省力而走捷径的产物，存储于基底神经节
  why_it_matters: |
    下游一切习惯类 skill 的验收标准是"无意识发生"，而不是"用户表示喜欢"；二者测量方式
    完全不同。
  tags: [term, core-concept]
```

```yaml
- id: g03
  term: 触发（trigger）与外部触发四类
  type: term
  source_chapter: 第2章（L560–628）
  author_definition: |
    "触发就是指促使你做出某种举动的诱因——就像是发动机里的火花塞。触发分外部触发和
    内部触发。"（L184–186）
  key_distinction: |
    ≠ 推送/广告的统称：外部触发四类（付费型/回馈型/人际型/自主型）成本结构与任务不同
    ——前三类拉新，自主型（用户许可后持续出现）驱动重复
    ≠ 任意提醒：外部触发必须"将下一个行动步骤清楚地传达给用户"
  why_it_matters: |
    混淆四类会导致把"买量"当"留存"；自主型触发的许可属性是伦理与效果的交汇点。
  tags: [term, core-concept]
```

```yaml
- id: g04
  term: 内部触发（internal trigger）
  type: term
  source_chapter: 第2章（L636–669）
  author_definition: |
    "当某个产品与你的思想、情感或是原本已有的常规活动发生密切关联时，那一定是内部触发
    在起作用。……你看不见，摸不着，也听不到，但它会自动出现在你的脑海中。"（L636–639）
  key_distinction: |
    ≠ 品牌心智/印象：特指情绪（尤其负面情绪）→产品的条件反射弧
    ≠ 使用场景描述：是"何时何地何种情绪下会想到你"的自动联想
    = 习惯的完成态标志；外部触发的服务对象
  why_it_matters: |
    下游触发类 skill 的目标函数：设计是否成功，看它是否在用户情绪波动时自动出现；
    5 问法是定位它的标准工具。
  tags: [term, core-concept]
```

```yaml
- id: g05
  term: 行动（action）
  type: term
  source_chapter: 第3章（L800–823）
  author_definition: |
    "触发之后就是行动，意即在对某种回报心怀期待的情况下做出的举动。"（L194）
  key_distinction: |
    ≠ 点击/转化等运营指标：是行为发生学的最小单元
    ≠ 任意动作：以"期待酬赏"为前提；复杂度越低重复可能性越大
  why_it_matters: |
    防止下游 skill 把"行动阶段"写成转化率优化；其内核是 B=MAT 三要素的乘法关系与
    "先补能力短板"的工程顺序。
  tags: [term, core-concept]
```

```yaml
- id: g06
  term: B=MAT（福格行为模型）
  type: term
  source_chapter: 第3章（L809–823）
  author_definition: |
    "B 代表行为，M 代表动机，A 代表能力，T 代表触发。要想使人们完成特定的行为，动机、
    能力、触发这三样缺一不可。"（L813）
  key_distinction: |
    ≠ 需求分析：是行为是否发生的诊断式（乘法关系，任一为零则全零）
    ≠ 说服理论：不解释偏好来源，只解释行动门槛（"行动线"）
  why_it_matters: |
    "手机响了为什么没接"的排查逻辑（能力/动机/触发三归因）是下游一切"用户为什么不
    行动"类 skill 的默认第一步。
  tags: [term, core-concept]
```

```yaml
- id: g07
  term: 动机（三组核心动机）
  type: term
  source_chapter: 第3章（L830–838）
  author_definition: |
    爱德华·德西："行动时拥有的热情。"（L830）福格："追求快乐，逃避痛苦；追求希望，
    逃避恐惧；追求认同，逃避排斥。"（L834）
  key_distinction: |
    ≠ 需求清单/用户画像标签：是三对趋避杠杆，任何行为同时受两端拉扯
    ≠ 人人通用：对一部分人有效的动机对另一部分人可能适得其反（L851）
  why_it_matters: |
    激励与文案类 skill 必须先选对杠杆（哪一组趋避）再谈强度；错组即失效。
  tags: [term, core-concept]
```

```yaml
- id: g08
  term: 能力（简洁性六要素）
  type: term
  source_chapter: 第3章（L908–926）
  author_definition: |
    "时间、金钱、体力、脑力、社会偏差、非常规性"——影响任务难易程度的 6 个要素；
    "设计人员在设计产品时，应该关注用户最缺乏什么"（L922）。
  key_distinction: |
    ≠ 易用性评分的泛称：是六项可逐项排查的摩擦源
    ≠ 平均优化：只补目标用户"最缺乏"的那一项，六要素因人因时而异
  why_it_matters: |
    "社会偏差"与"非常规性"两项是常识清单里最常被漏掉的；漏掉它们会误判"功能明明
    很简单为什么没人用"。
  tags: [term, core-concept]
```

```yaml
- id: g09
  term: 启发法（heuristics / 认知偏差）
  type: term
  source_chapter: 第3章（L1055–1119）
  author_definition: |
    "所谓启发，是指我们的大脑利用过往的经验，在对事物做出判断的过程中抄了近道。尽管
    人们多数情况下意识不到启发法对其行为产生的影响，但它的确可以预测人们的行为。"（L1055）
  key_distinction: |
    ≠ 营销话术：书中四效应（稀缺/环境/锚定/目标渐近）各有实验出处与产品化用法
    ≠ 无代价技巧：与操纵矩阵对读，偏差利用须过"该不该"关
  why_it_matters: |
    下游 persuasion 类 skill 引用这些效应时应注明来源效应名与实验，而非当作常识技巧。
  tags: [term, cognitive-bias]
```

```yaml
- id: g10
  term: 多变的酬赏（variable reward）
  type: term
  source_chapter: 第4章（L1189–1232、L1510–1524）
  author_definition: |
    "多变的酬赏，就是指酬赏要有不可预期性。"（L77）"驱使我们采取行动的，并不是酬赏
    本身，而是渴望酬赏时产生的那份迫切需要。"（L1204）
  key_distinction: |
    ≠ 奖励/积分：可预期的奖励不产生渴望（冰箱门反例）
    ≠ 单一奖赏：三条通道（社交/猎物/自我）机制不同，可并存
    = 上瘾模型与普通反馈回路的分界线
  why_it_matters: |
    "多变"而非"多"是关键词；下游任何激励设计 skill 的第一检查项是变量的来源与存续
    （有限/无穷多变性）。
  tags: [term, core-concept]
```

```yaml
- id: g11
  term: 社交酬赏（tribal reward）
  type: term
  source_chapter: 第4章（L1243–1281）
  author_definition: |
    "社交酬赏，抑或说部落酬赏，源自我们和他人之间的互动关系。为了让自己觉得被接纳、
    被认同、受重视、受喜爱，我们的大脑会自动调试以获得酬赏。"（L1243）
  key_distinction: |
    ≠ 社交功能（评论/分享按钮）：功能只是载体，酬赏是"被部落接纳"的体验
    ≠ 确定性回报：其多变来自他人反应的不可预测（点赞、威望值、荣誉值）
  why_it_matters: |
    区分"加了社交功能"与"给了社交酬赏"：后者要求不确定的认可回路，前者可能只是
    又一个静默的消息入口。
  tags: [term, reward]
```

```yaml
- id: g12
  term: 猎物酬赏（reward of the hunt）
  type: term
  source_chapter: 第4章（L1287–1330）
  author_definition: |
    "对具体物品——比如食物和生活必备品——的需求，是人类最基本的需求之一。……取而代之
    的是其他一些东西"（资源与信息）；"猎手是为了追逐而追逐"（L1300）。
  key_distinction: |
    ≠ 内容价值本身：酬赏在追逐过程而非所得（信息流、老虎机）
    ≠ 搜集癖：机制根源是耐力捕猎时代"追逐即奖励"的进化遗产
  why_it_matters: |
    信息流类产品设计的机制内核；判断一个信息流是否"钩人"，看它是否把资源获取做成了
    不确定的追逐。
  tags: [term, reward]
```

```yaml
- id: g13
  term: 自我酬赏（reward of the self）
  type: term
  source_chapter: 第4章（L1334–1373）
  author_definition: |
    "体现了人们对于个体愉悦感的渴望。……依据他们提出的自我决定论，人们在心怀其他欲望
    之外，还渴望'终结感'。"（L1337–1339）
  key_distinction: |
    ≠ 游戏成就系统：核心是操控感、成就感、终结感（任务闭合体验）
    ≠ 外部认可：与社交酬赏的区分在于无须他人在场
  why_it_matters: |
    工具型与学习型产品最容易错配酬赏类型——给了徽章却没给"清空/完成/掌握"的终结感。
  tags: [term, reward]
```

```yaml
- id: g14
  term: 投入（investment）
  type: term
  source_chapter: 第5章（L1559–1658）
  author_definition: |
    "当用户为某个产品提供他们的个人数据和社会资本，付出他们的时间、精力和金钱时，
    投入即已发生。……投入并不意味着让用户舍得花钱，而是指用户的行为能提升后续服务
    质量。"（L212–214）
  key_distinction: |
    ≠ 付费/消费：付费是商业行为，投入是改善未来体验的行为
    ≠ 行动：行动求即时满足，投入期待长期回报；行动减摩擦，投入可加摩擦
    = 必须发生在酬赏之后、从小步开始
  why_it_matters: |
    "投入≠付费"是本书对行业认知最直接的纠偏；下游 skill 若把投入写成付费引导即失真。
  tags: [term, core-concept]
```

```yaml
- id: g15
  term: 储存价值（stored value）
  type: term
  source_chapter: 第5章（L1662–1736）
  author_definition: |
    "用户向产品投入的储存价值形式多样，可增加用户今后再次使用该产品的可能性"——内容、
    数据资料、关注者、信誉、技能五形式（L1665、L1812）。
  key_distinction: |
    ≠ 用户数据资产的泛称：特指五类让"改换产品=放弃自己"的资产
    ≠ 锁定（lock-in）的贬义：作者视角是双向收益（服务质量随投入提升），批判视角须补
      区分价值留存与被迫锁定
  why_it_matters: |
    下游所有护城河/留存类 skill 的检查清单；也提醒 B 段区分"用户真心获益的留存"与
    "恶意锁定"。
  tags: [term, moat, switching-cost]
```

```yaml
- id: g16
  term: 加载下一个触发（loading the next trigger）
  type: term
  source_chapter: 第5章（L1746–1793）
  author_definition: |
    "习惯养成类技术利用用户过去的行为为今后启动一个外部触发。"（L1749）
  key_distinction: |
    ≠ 运营推送：触发由用户自己的投入生成（发消息、定日程、滑动），非运营群发
    ≠ 定时提醒：时机对准内部触发最活跃的瞬间（Any.do 的会后焦虑）
  why_it_matters: |
    这是上瘾模型闭环的"合页"；混淆它与普通推送会漏掉"内生触发"这一设计要求。
  tags: [term, loop, core-concept]
```

```yaml
- id: g17
  term: 习惯区间（habit zone）
  type: term
  source_chapter: 第1章（L429–445）
  author_definition: |
    "要想打造习惯养成类产品，企业务必认真考虑两个因素。第一，频率……第二，可感知用途
    ……若某种行为发生的频率足够高，被感知到的用途足够多，就会进入我们的'习惯区间'。"（L429–433）
  key_distinction: |
    ≠ 爆品标准：爆品可低频高刺激；习惯区间要求频率为第一变量
    = 频率不足的行为永远成不了习惯（曲线不相交横轴）
  why_it_matters: |
    新点子/新习惯可行性过滤的第一道闸；也解释为什么低频产品要走亚马逊式"可感知用途"
    路线。
  tags: [term, diagnostic]
```

```yaml
- id: g18
  term: 维生素 vs 止痛药
  type: term
  source_chapter: 第1章（L449–474）
  author_definition: |
    "习惯养成类产品起初都是非必需品（比如维生素），可一旦发展为习惯，它们就会变成
    必需品（比如止痛药）。"（L500）
  key_distinction: |
    ≠ 投资人语境的"真/伪需求"二分：作者主张时间维度转换——先维生素后止痛药
    = 转变发生的判据："如果你因为无法实施某种行为而感到痛苦，那说明习惯业已形成"（L468）
  why_it_matters: |
    防止用"这功能可有可无"过早否掉产品，也防止用"用户 love it"误判已成习惯。
  tags: [term, product-strategy]
```

```yaml
- id: g19
  term: "痒"（itch）
  type: term
  source_chapter: 第1章（L470）；第2章（L649、L865）
  author_definition: |
    "实际上，我们所要描述的体验更接近于'痒'，它是潜伏于我们内心的一种渴求，当这种
    渴求得不到满足时，不适感就会出现。"（L470）
  key_distinction: |
    ≠ 痛点（pain point）：痒是轻微、常不被觉察的持续不适，非剧痛
    ≠ 需求：痒是情绪性的渴求状态，产品是"挠痒"的更快手段
  why_it_matters: |
    内部触发定位的搜索词：设计者该找的不是用户的"痛点"（商学院夸张用法）而是高频
    低烈度的"痒"。
  tags: [term, emotion]
```

```yaml
- id: g20
  term: 成瘾（addiction）与习惯之辨
  type: term
  source_chapter: 第1章（L476–478）；第6章（L1926–1932）
  author_definition: |
    "'成瘾'指的是长期且被动地依赖某种行为或是某个东西。依照定义，'成瘾'最终会使人
    走向自我毁灭。"（L476）
  key_distinction: |
    ≠ 习惯：习惯可以有益且无意识；成瘾是被动、渐进、以损害为终点的依赖
    = 伦理分水岭：设计习惯正当，制造成瘾"等同蓄意伤害"
  why_it_matters: |
    所有 hook 类 skill 的硬边界与 B 段素材：当使用挤占生活功能、用户主观失控时，任何
    继续优化的动作都越线。
  tags: [term, ethics, boundary]
```

```yaml
- id: g21
  term: 逆反心理（reactance）
  type: term
  source_chapter: 第4章（L1425–1463）
  author_definition: |
    "你在自主权利受到威胁时所产生的一触即发的反应。"（L1431）
  key_distinction: |
    ≠ 用户难搞/流失借口：是可被设计触发或避免的机制变量
    ≠ 单纯反感：特指选择自由被剥夺时的对抗性动机唤起
  why_it_matters: |
    下游一切"要求用户做事"的设计（onboarding、权限、打卡）都要过这道检查：给选择权
    反而更顺从。
  tags: [term, psychology, autonomy]
```

```yaml
- id: g22
  term: 多变性（有限 / 无穷）
  type: term
  source_chapter: 第4章（L1484–1492）
  author_definition: |
    "有限的多变性会使产品随着时间的推移而丧失神秘感和吸引力，而无穷的多变性是维系用户
    长期兴趣的关键。"（L1522）
  key_distinction: |
    ≠ 更新频率：是产品结构属性（可预见性），不是运营节奏
    = 无穷多变性几乎总来自"他人"（其他用户、对手、系统），个人内容消耗品天然有限
  why_it_matters: |
    判断产品生命周期的先验指标；也解释 UGC 平台对内容消耗型产品的结构性优势。
  tags: [term, retention, product-strategy]
```

```yaml
- id: g23
  term: 操纵矩阵（manipulation matrix / 操控模式）
  type: term
  source_chapter: 第6章（L1894–1985）
  author_definition: |
    用两问分四象限："我自己会使用这个产品吗""该产品会帮助用户大大提高其生活质量吗"；
    四象限为健康习惯推广者、兜售商、娱乐用户者、经销商（L1896–1968）。
  key_distinction: |
    ≠ 道德守则/合规清单：是设计者自检的决策支持工具，回答"该不该"而非"能不能"
    ≠ 二元善恶：娱乐用户者（艺术）也是合法象限，各有商业含义
  why_it_matters: |
    下游所有 hook 类 skill 的出厂检查；同时注意其主观性局限（自报+羞愧判据），需与
    外部反馈互补。
  tags: [term, ethics, core-concept]
```

```yaml
- id: g24
  term: 习惯测试（habit test）
  type: term
  source_chapter: 第8章（L2154–2200）
  author_definition: |
    "通过我的研究以及与当今最成功的习惯养成类产品生产公司的企业家们的讨论，我对这一
    过程进行了提炼，并将其命名为'习惯测试'。"（L2161）三步：确定用户、分析用户行为、
    改进产品。
  key_distinction: |
    ≠ 留存分析/埋点报表：有前置定义（忠实用户频率）、量化基准（5%）与明确产出物
      （习惯路径）
    ≠ 一次性动作：随每次功能迭代重复执行
  why_it_matters: |
    上瘾模型的验证装置；没有它，四阶段模型无法证伪也无法指导迭代。
  tags: [term, measurement]
```

```yaml
- id: g25
  term: 习惯路径（habit path）
  type: term
  source_chapter: 第8章（L2187–2198）
  author_definition: |
    "你要找到一条'习惯路径'，即你最忠实的用户共同具有的一系列相似行为。"（L2187–2188）
  key_distinction: |
    ≠ 用户旅程图：只从已成习惯的用户反推，不来自设计者想象的正途
    ≠ 相关性堆砌：要找的是与留存强相关的行为序列（Twitter"关注 30 人"）
  why_it_matters: |
    把"为什么有人留下来"变成可复制的产品改进；也是"忠诚用户画像"的替代品——看行为
    不看人口属性。
  tags: [term, measurement]
```

```yaml
- id: g26
  term: 宜家效应 / 目标渐近效应 / 文饰作用
  type: term
  source_chapter: 第3章（L1107）；第5章（L1583、L1623）
  author_definition: |
    宜家效应：付出过劳动的人会给自己的作品附加更多价值（自折纸鹤估值 5 倍，L1583）；
    目标渐近效应：距目标越近完成动机越强（洗车卡 82% 差异，L1107）；文饰作用："这一
    心理过程会令我们改变自己的态度和信念，从心理上进行调适"（L1623）。
  key_distinction: |
    ≠ 泛心理学段子：三者共同构成"投入改变态度"的机制链，且都指向可设计的行为
    （让用户动手、让进度可见、允许用户自我合理化）
  why_it_matters: |
    投入阶段 skill 的机制底层；引用时保持三者的分工（估值/动机/合理化）不混用。
  tags: [term, psychology, investment]
```

```yaml
- id: g27
  term: 病毒循环周期 / 用户终身价值
  type: term
  source_chapter: 第1章（L327–359）
  author_definition: |
    用户终身价值："一个用户在其有生之年忠实使用某个产品的过程中为其付出的投资总额"
    （L327）；病毒循环周期："老用户邀请新用户花费的时长"（L357）。
  key_distinction: |
    ≠ 增长黑客术语的泛用：书中二者的因果都挂在"依赖性/频率"上——习惯提升 LTV，频率
      压缩周期
  why_it_matters: |
    习惯的商业收益换算器；下游 skill 论证 ROI 时应回到"依赖性→LTV/定价权/周期"的
    原始链条。
  tags: [term, business]
```
