# candidates/principles.md — 原则提取器产出（阶段 1）

> 来源：《战略与路径》十二章。引文经与 src/ 原文定点核对。宁多勿漏，待阶段 1.5 三重验证。

```yaml
- id: p01
  title: 先立后破，保留安全冗余
  type: principle
  source_chapter: 第三章
  source_quote: |
    "'先立后破、爬行钉住加保留安全冗余'的原则推动清洁替代"。
  summary: |
    做任何不可逆的大转型（换技术栈、换供应商、换能源结构）时：新系统没立稳之前不拆旧系统，转型全程保留安全冗余。
    判断标准：旧系统的退出节奏由新系统的建成进度决定，而不是由目标日期决定。
  tags: [transition, risk-control, energy]

- id: p02
  title: 顽固问题从制度土壤求解
  type: principle
  source_chapter: 第七章
  source_quote: |
    "凡是广泛存在的问题、长期存在的问题一定要从制度、基础土壤的角度去分析、去求解、去采取措施"。
  summary: |
    凡是广泛存在、长期存在的问题，不要在症状层修补（补贴、运动、道德呼吁），必须上溯到制度与基础土壤层面求解。
    使用规则：先验证问题是否"广泛+长期"，两个条件同时满足才适用。
  tags: [root-cause, governance]

- id: p03
  title: 三次分配次序原则
  type: principle
  source_chapter: 第七章
  source_quote: |
    "一次分配讲效率兼顾公平、二次分配讲公平兼顾效率、三次分配讲自愿讲道德，也要讲有效激励的制度安排"。
  summary: |
    调节分配问题的次序：一次分配（工资、要素报酬）是基础，二次分配（税收、转移支付）是关键，三次分配（捐赠）只是配套辅助。
    应用规则：解决贫富差距优先改一次分配结构（源头），不把希望主要寄托在再分配与慈善上。
  tags: [distribution, common-prosperity]

- id: p04
  title: 法拍房比例判断房价风险
  type: principle
  source_chapter: 第六章
  source_quote: |
    法拍房 2017 年 5000 套→2020 年 127 万套；占比超交易量 5% 即影响定价、超 20-30% 房价必跌。
  summary: |
    判断一个城市房价下行风险的可操作指标：法拍房占二手房交易量的比例。<5% 安全，5-20% 定价承压，>20-30% 价格必螺旋下跌。
    使用规则：配合交易量萎缩（连续两年降 30%+）一起判断，法拍是打破"有价无市"僵局的关键变量。
  tags: [real-estate, indicator, risk]

- id: p05
  title: 楼面地价不超过房价三分之一
  type: principle
  source_chapter: 第六章
  source_quote: |
    "楼面地价不要超过当期房价的1/3"。
  summary: |
    政府控制地价与房价联动的基本标尺：楼面地价 ≤ 当期房价的 1/3。超过则地价推高房价、挤压开发商利润与质量空间。
    可迁移用法：分析任何"上游原料成本占比"对下游价格健康度的约束（原料/成品 ≤ 1/3 为健康区）。
  tags: [real-estate, land, pricing]

- id: p06
  title: 住宅用地占比与人均用地标尺
  type: principle
  source_chapter: 第六章
  source_quote: |
    城市人均 100 平米土地、住宅用地占比 25%、公租房覆盖 20% 人口人均 20 平米、公租房与商品房 1∶3 搭配。
  summary: |
    城市土地供应的一组量化标尺：人均建设用地 100 平米、其中住宅用地占 25%、公租房覆盖 20% 人口。深圳高房价的根源即可用此诊断（2000 万人需 2000 平方公里，实际仅 1000 平方公里）。
    用于判断一个城市房价的根本成因是需求还是供地。
  tags: [real-estate, land-supply]

- id: p07
  title: 制造业占比红线
  type: principle
  source_chapter: 第五章
  source_quote: |
    红线：2035 年前制造业占 GDP 比重不低于 25%、2050 年前不低于 20%；制造业占比下降的国际经验是"缓慢渐进、迈入高收入后才开始"。
  summary: |
    经济体在未跨入高收入行列前，制造业占比过早过快下滑是产业空心化前兆。守住占比红线，同时观察四个配套特征（下降是否渐进、科研是否领先、生产性服务业是否同步）。
    适用于产业政策评估与经济结构健康度诊断。
  tags: [manufacturing, industrial-policy]

- id: p08
  title: 企业杠杆率警戒线
  type: principle
  source_chapter: 第六章
  source_quote: |
    房企负债率 90 年代末 50.3%→2020 年 80.13%；新模式要求"负债率降低至国家要求的'三道红线'以下，甚至降低到50%以内"。
  summary: |
    高杠杆行业（房地产、金融）的资产负债率警戒线参考：50% 为健康上限，80%+ 为危机区。行业整体杠杆触顶是拐点信号之一。
    使用规则：结合行业属性校准（重资产行业上限可略高），重点看增速而非绝对值。
  tags: [leverage, risk, real-estate]

- id: p09
  title: 房企"不交楼不月供"
  type: principle
  source_chapter: 第六章
  source_quote: |
    五个转变之一：预售制改"不交楼不月供"。
  summary: |
    预售制度的改革方向：购房者月供与交楼绑定，风险由购房者转向银行与开发商。本质是把"烂尾风险"分配给最能控制它的一方。
    可迁移用法：任何交易设计中，风险应分配给最有能力控制它的一方。
  tags: [real-estate, risk-allocation]

- id: p10
  title: 绝不追求任何技术 100% 自给
  type: principle
  source_chapter: 第九章
  source_quote: |
    反"小而全"：绝不追求任何技术 100% 自给；日用消费品"形成一定的自主保障能力即可，并不一定要追求大包大揽、完全国产"。
  summary: |
    自主可控的边界：只对"卡脖子"关键环节追求自主，非关键环节保持开放分工。全面自给反而降低效率、丧失朋友圈。
    判断标准：被断供后是否"一剑封喉"——能封喉的才值得自主化投入。
  tags: [technology, self-reliance, trade]

- id: p11
  title: 平台不得大数据杀熟；脱敏数据归平台
  type: principle
  source_chapter: 第四章
  source_quote: |
    原始个人数据所有权归消费者、平台只有使用权且不得大数据杀熟；脱敏后数据平台可拥有所有权并出售，原始数据人无收益主张权（因举证验证成本极高无法操作）。
  summary: |
    数据权利分配的两条规则：原始数据归个人（平台只有使用权、禁止杀熟）；脱敏加工后归平台（个人不再主张收益）。
    适用于数据产品设计、隐私条款、数据交易合规的权责划界。
  tags: [data-economy, platform, privacy]

- id: p12
  title: 公共服务平台出事重罚
  type: principle
  source_chapter: 第四章
  source_quote: |
    公共服务类平台出事重罚（赔偿至少加 10 倍）；网约车出事常规赔偿 180 万元 vs 优步赔数千万美元——支撑重罚逻辑。
  summary: |
    承担公共职能的平台（出行、支付、社交基础设施）出事须惩罚性赔偿（≥10 倍），因为其外部性远超普通商业主体。
    可迁移用法：对"系统性重要"主体（大平台、系统重要性银行）的问责标准应高于普通主体。
  tags: [platform, regulation, liability]

- id: p13
  title: 战略上藐视、战术上重视
  type: principle
  source_chapter: 第十二章
  source_quote: |
    "战略上藐视（纸老虎）、战术上重视（真老虎）"；32 字原则——丢掉幻想准备斗争、保持定力增强信心、守住底线灵活应对、抓住关键克服短板。
  summary: |
    对抗长期竞争压力的心态与操作分离：战略层面不被对手声势吓倒（多数威胁因成本约束不会全面发生），战术层面逐项认真准备（备份、反制、底线预案）。
    配套原则："先为不可胜而后可胜"——先保证自己不败，再求胜。
  tags: [strategy, competition, mindset]

- id: p14
  title: 判断政策转向看相对成本而非财政动机
  type: principle
  source_chapter: 第三章（问答）
  source_quote: |
    判断新能源政策转向的方法：看度电成本与火电的相对关系，而非财政动机；中国光伏度电成本已低于火电。
  summary: |
    预测一项政策/技术能否持续推广，看它相对于在位方案的成本曲线交叉点，而不是政府补贴口风。补贴是结果（交叉点过后取消），不是原因。
    适用于新能源、新技术、新商业模式可持续性判断。
  tags: [forecasting, energy, cost-curve]

- id: p15
  title: 货币自由兑换两个前置条件
  type: principle
  source_chapter: 第十章（问答）
  source_quote: |
    货币自由兑换两边界条件：人均 GDP 进入高收入圈、货币清算占比与 GDP 占比相当。
  summary: |
    把模糊的"何时开放资本账户"转化为两个可检验的门槛：经济体量达标 + 货币国际使用份额与经济份额匹配。门槛未到就开放是自毁（广场协议、休克疗法为镜）。
    可迁移用法：重大金融开放决策先列可检验前置条件清单。
  tags: [finance, currency, sequencing]

- id: p16
  title: 征税面从窄、税负从轻
  type: principle
  source_chapter: 第七章
  source_quote: |
    遗产税出台原则"征税面从窄、税负从轻"；遗产税须统筹国际竞争，不能只看国内调节功能（法国 70% 遗产税致富豪外迁）。
  summary: |
    新税种（及各类新管制）出台的节奏原则：起步时覆盖面窄、税负轻，先立制度再逐步扩大，且必须考虑要素外逃的国际竞争约束。
    可迁移用法：任何增加成本的制度落地都应"窄起步、轻负担、留退出通道"。
  tags: [tax, institutional-design]

- id: p17
  title: 大中城市 1:3 梯次与超大城市 1500 万上限
  type: principle
  source_chapter: 第一章
  source_quote: |
    每亿人约 1 个超大城市、全国 14 个左右；超大城市人口天花板 1500 万；城市群内大中小城市按 1∶3 梯次递减。
  summary: |
    城市群规划的量化标尺：超大城市人口上限约 1500 万、城市群内城市规模按 1:3 逐级递减、都市圈城市化率 70%+。
    用于判断一个城市的人口政策空间与楼市长期容量。
  tags: [urbanization, city-planning]

- id: p18
  title: 低风险≠低危害（风险分级要分维度）
  type: principle
  source_chapter: 第十二章
  source_quote: |
    高/中/低风险指"全面发生的可能性"而非危害度——低风险项一旦发生危害反而最大（"金融核弹"）。
  summary: |
    做风险分级时必须区分两个维度：发生可能性（概率）与危害度（损失）。低概率项可能危害最大，须分别管理：高概率项靠预防、低概率高危害项靠威慑与备胎。
    适用于一切风险管理清单的设计。
  tags: [risk-management, framework-hygiene]

- id: p19
  title: 反垄断盯住 80-90% 份额
  type: principle
  source_chapter: 第四章
  source_quote: |
    平台经济十大原则之一：反垄断（防 80%—90% 份额）；平台与金融业务隔离。
  summary: |
    平台治理的数量化红线：单一平台市场份额达 80-90% 即触发反垄断关注；金融业务必须与平台业务隔离（防火墙）。
    可迁移用法：判断一个生态是否需要分拆/隔离时，用份额阈值+业务混业两个触发器。
  tags: [antitrust, platform, regulation]

- id: p20
  title: 资本项下管制是盾牌
  type: principle
  source_chapter: 第十二章
  source_quote: |
    三个护身符：资本项下管制；外资在华巨量资产（3.6 万亿美元工商投资+2.2 万亿金融资产）；外贸体量结构。"资本项下不可自由兑换是体制优势/盾牌"。
  summary: |
    开放次序原则：资本账户自由化是最后一步而非第一步；资本项下管制在博弈中是防御盾牌（对方金融核弹打不进来，己方也不被动挨打）。
    适用于新兴市场金融开放次序、个人资产配置的国别风险视角。
  tags: [finance, capital-control, geopolitics]
```
