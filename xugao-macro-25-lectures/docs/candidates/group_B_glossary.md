# 术语候选（第3-4讲，全书级概念）

# ===== 第3讲 =====

- id: Bg01
  title: 生产函数（production function）
  type: term
  source_chapter: 第3讲 3.3节
  source_quote: |
    这一框架就是生产函数（production function）——个把投入要素和产出联系起来，概括了经济中
    生产活动的函数。
  summary: |
    全书供给面分析的基础工具：Y=F(K,L)，K为资本存量、L为劳动投入。作者强调每写下一个生产
    函数就等于对生产技术做出一组重要假设（规模报酬、边际报酬性质等），因此用生产函数前必须
    知道自己假设了什么。
  tags: [生产函数, 供给面]

- id: Bg02
  title: 规模报酬不变（constant returns to scale, CRS）
  type: term
  source_chapter: 第3讲 3.3.1节
  source_quote: |
    如果所有投入要素都倍增，那么总产出也应该倍增。所以应该有2Y=F(2K,2L)。
  summary: |
    生产函数的一次齐次性质：所有要素同比例放大则产出同比例放大。直观依据是"复制企业"：再建
    一个同样的企业产量应翻倍。在完全竞争下与欧拉定理结合推出要素收入完全分割产出（Y=rK+wL），
    也是增长计量按份额分解的前提。
  tags: [规模报酬, 欧拉定理]

- id: Bg03
  title: 稻田条件（Inada conditions）
  type: term
  source_chapter: 第3讲 3.3.2节
  source_quote: |
    即当资本投入量非常小时，增加一点资本带来的边际产出非常巨大。相反，当资本投入已经很多时，
    增加资本带来的边际产出微乎其微。
  summary: |
    新古典生产函数的经典假设组（因日本经济学家稻田献一得名）：无投入无产出、边际产出为正且
    递减、极小投入时边际产出趋于无穷、极大投入时趋于零。保证索洛模型稳态存在，但同时排除了
    资本回报为零或为负（产能过剩）的情形——是"假设划定分析边界"的标志性例子。
  tags: [稻田条件, 假设边界]

- id: Bg04
  title: 索洛剩余 / 全要素生产率（TFP）
  type: term
  source_chapter: 第3讲 3.4节
  source_quote: |
    尽管我们将gA看作技术进步的表征，又将其称为索洛剩余（Solow residual），或全要素生产率（TFP），
    但对它最贴切的称呼还是"对我们未知的度量"（measure of our ignorance）。
  summary: |
    增长计量中作为回归残差估计出的gA：产出增长中不能被资本和劳动解释的部分。装着技术、制度、
    文化等一切因素的黑箱。作者使用规范：称A为"索洛剩余"而尽量避免叫"技术"，因为索洛剩余中
    不只有技术，技术也不全在索洛剩余中。
  tags: [索洛剩余, TFP, 黑箱]

- id: Bg05
  title: 柯布-道格拉斯生产函数（Cobb-Douglas production function）
  type: term
  source_chapter: 第3讲 3.3.4节
  source_quote: |
    他们于1928年发表了一篇文章，提出了著名的柯布-道格拉斯生产函数（Cobb-Douglas production
    function）。Y=K^α L^β。当α+β=1时，这一生产函数呈现出规模报酬不变的特性。
  summary: |
    宏观经济学最常用的生产函数Y=AK^α L^(1-α)，由道格拉斯的份额稳定数据与柯布的数学构造于
    1928年提出。性质：要素份额恒为α与1-α；三种技术引入方式在其框架下等价；人均形式y=Ak^α。
    全书增长分析与第4讲资本密集度讨论的载体。
  tags: [柯布-道格拉斯, 生产函数]

- id: Bg06
  title: 资本份额（capital share）α
  type: term
  source_chapter: 第3讲 3.3.4节、第4讲 4.2节
  source_quote: |
    在柯布-道格拉斯生产函数（3.9）式中，α叫做资本份额（capital share）……在真实世界中，资本份额α
    决定于生产技术。那些资本密集度高的行业（如电子芯片制造），α会高一些。
  summary: |
    资本总回报占总产出的比重，数值上等于资本的产出弹性。第3讲中作为行业资本/劳动依赖度的
    度量；第4讲进一步升格为"生产技术的资本密集度"——它是技术的刻画而非仅仅是回归系数，
    并成为发展战略分析的核心参数（黄金律储蓄率也恰等于α）。
  tags: [资本份额, 资本密集度]

- id: Bg07
  title: 增长计量 / 增长核算（growth accounting）
  type: term
  source_chapter: 第3讲 3.4节
  source_quote: |
    利用生产函数，我们可以将经济增长分解为来自资本、劳动力以及技术的贡献……这就是增长计量
    （growth accounting）。
  summary: |
    把GDP增速分解为资本贡献α·gK、劳动贡献(1-α)·gL与技术贡献gA的核算方法：gY=αgK+(1-α)gL+gA。
    可观测变量回归估α，gA作残差。是本讲分析中国增长源泉与减速原因的主工具，也是"数量检验
    流行叙事"（人口红利说）的手段。
  tags: [增长核算, 分解]

- id: Bg08
  title: 稳态（steady state）
  type: term
  source_chapter: 第3讲 3.5.2节
  source_quote: |
    人均资本存量不变的状态被称为稳态（steady state）。这一状态下的人均资本存量水平被称为稳态
    人均资本存量，用k*来表示。
  summary: |
    索洛模型中人均资本不再变化的状态，满足sAf(k*)=(n+δ)k*。稻田条件保证无论起点高低都收敛到
    稳态；稳态人均产出、消费都是k*的单调函数，故长期福利水平问题可以化为稳态资本存量问题。
    大道定理保证经济很快收敛到稳态附近，使"长期"讨论有现实意义。
  tags: [稳态, 索洛模型]

- id: Bg09
  title: 储蓄的黄金律（golden rule）
  type: term
  source_chapter: 第3讲 3.5.3节
  source_quote: |
    给定技术水平，有一个最大化稳态人均消费量的储蓄率，被称为储蓄的黄金律（golden rule）水平
    ……可以解出，s_Golden=α。
  summary: |
    最大化稳态人均消费的储蓄率水平，柯布-道格拉斯下等于资本份额α。它是"以福利而非产出为目标"
    时评价储蓄率高低（中国储蓄过剩问题）的模型基准：高于黄金律意味着过度投资、消费被挤压。
  tags: [黄金律, 储蓄率, 福利]

- id: Bg10
  title: 外生变量与内生变量（exogenous / endogenous variables）
  type: term
  source_chapter: 第3讲 3.5.1节
  source_quote: |
    所谓外生变量（exogenous variables），是那些取值由建模者设定的变量。而内生变量（endogenous
    variables）则是取值在模型内部被决定的变量。
  summary: |
    建模的基本二分：外生变量在求解前给定（只是假设），内生变量由模型解出（体现要发掘的经济
    机制）。索洛模型中n、g、s、δ外生，K内生积累。评价模型的关键是审查外生假设是否贴合现实。
  tags: [内生, 外生, 建模]

# ===== 第4讲 =====

- id: Bg11
  title: 生产技术的资本密集度（capital intensity）
  type: term
  source_chapter: 第4讲 4.2节
  source_quote: |
    在本书中，为了清晰起见，我们把柯布-道格拉斯生产函数中的资本份额α称为生产技术的资本密集度
    （capital intensity）。这是对生产方式的一个刻画。
  summary: |
    全书规范用法：α=生产技术的资本密集度，刻画生产方式对资本的依赖（芯片高、服装低）；A称为
    索洛剩余而非"技术"。与要素需求结合：α越大，厂商在给定相对价格下选择越高的资本/劳动比。
    资源禀赋决定可用的资本密集度区间，是发展战略分析的核心概念。
  tags: [资本密集度, 技术选择]

- id: Bg12
  title: 资源禀赋结构（endowment structure）
  type: term
  source_chapter: 第4讲 4.3.2节、4.4.1节
  source_quote: |
    我们要问的是：给定一个经济当前所拥有的资本和劳动力的资源禀赋结构（endowment structure），
    这个经济应该采用什么样资本密集度的生产技术？
  summary: |
    经济当时拥有的资本与劳动力的相对数量（以人均资本存量k/l为代表）。禀赋结构决定合意的资本
    密集度区间，且随资本积累动态变化；发展战略是否与禀赋匹配决定经济绩效——是连接增长模型
    与发展经济学的枢纽概念。
  tags: [资源禀赋, 人均资本]

- id: Bg13
  title: 多样化锥（diversification cone）
  type: term
  source_chapter: 第4讲 4.3.2节
  source_quote: |
    只有人均资本存量处在下面这个区间中时，两类技术才会被同时采用……所以这个锥叫做多样化锥
    （diversification cone）。在多样化锥中……经济获得了比单独采用任何一种技术时都更高的产出。
  summary: |
    源自国际贸易理论的概念：在k-L坐标系中，两技术同时被采用的人均资本存量区间构成的锥形区域。
    锥内混合两种技术可获得比单独用任一技术更高的产出；锥外只有一种技术被采用。用于定位经济
    在发展阶梯上的位置。
  tags: [多样化锥, 技术选择]

- id: Bg14
  title: 比较优势发展战略（comparative advantage development strategy）
  type: term
  source_chapter: 第4讲 4.4.1节
  source_quote: |
    对一个国家的发展最有利的战略是，根据不同阶段经济的资源禀赋状况，选择各阶段对自己最有利的
    生产技术来组织生产——这便是林毅夫提出的比较优势发展战略。
  summary: |
    林毅夫提出的战略：随禀赋积累动态选择各阶段最有利（符合比较优势）的生产技术，从劳动密集型
    逐级上移到资本密集型。理论上等价于让市场自由选择（福利经济学第一定理），实践对应改革开放
    后中国的"小步快走"路径，是新结构经济学的滥觞。
  tags: [比较优势, 林毅夫, 发展战略]

- id: Bg15
  title: 赶超战略（leapforward strategy）
  type: term
  source_chapter: 第4讲 4.3.1节、4.4.2节
  source_quote: |
    也正是出于这种思路，中国在改革开放前曾力推赶超战略（leapforward strategy），试图通过大力
    建设重工业来"赶美超英"。
  summary: |
    落后国家无视自身禀赋、强行复制发达国家资本密集型产业结构的战略。后果：企业缺乏自生能力
    →压低利率工资与必需品价格→计划配置+国企化+人民公社→宏观失衡与激励缺失。改革开放前绩效
    差的主因，也是"制度内生于战略与禀赋矛盾"的典型样本。
  tags: [赶超战略, 重工业优先]

- id: Bg16
  title: 自生能力（viability）
  type: term
  source_chapter: 第4讲 4.4.2节
  source_quote: |
    按照林毅夫的定义，这样的企业缺乏自生能力（viability）。
  summary: |
    林毅夫定义：企业若无法在自由竞争的市场中以正常利润存活，即缺乏自生能力。违背比较优势建
    立的重工业企业在当时禀赋下资本密集型行业无法负担市场利率与工资，必然缺乏自生能力，需要
    持续的政策扭曲来维持——是判断产业政策可持续性的诊断概念。
  tags: [自生能力, 林毅夫, 企业存活]

- id: Bg17
  title: 新结构经济学（new structural economics）
  type: term
  source_chapter: 第4讲 4.1节、进一步阅读指南
  source_quote: |
    这正是林毅夫所倡导的新结构经济学（new structural economics）的思路。在这一讲中，我们会把
    分析的重心放在新结构经济学的滥觞——林毅夫提出的比较优势发展战略上。
  summary: |
    林毅夫在世行首席经济学家任上提出的理论体系，是本讲分析思路的学术来源：在主流框架中重新
    引入结构与禀赋维度，以"禀赋结构→合意产业结构→发展战略→绩效"为分析主线。本讲即用生产
    函数+技术选择模型为其提供微观基础。
  tags: [新结构经济学, 林毅夫, 结构]

- id: Bg18
  title: 有效需求（effective demand）
  type: term
  source_chapter: 第3讲 3.2节
  source_quote: |
    以"萨斯陷阱"闻名于世的马尔萨斯（Malthus，1766—1834）则提出了有效需求（effective demand）
    的概念，认为需求有可能小于供给，从而对供给构成约束。
  summary: |
    马尔萨斯提出的概念：有购买力支撑、能实际影响供给的需求。关键在于需求必须由收入分配决定
    的购买力支撑，而非无限欲望——由此需求可能小于供给并构成约束，与萨伊定律对立。是全书
    后续需求面分析（消费不足、过剩储蓄）的思想源头。
  tags: [有效需求, 马尔萨斯, 需求面]
