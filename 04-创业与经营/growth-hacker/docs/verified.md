# 《增长黑客》阶段 1.5 三重验证产出（verified.md）

> 输入：candidates/frameworks.md（34 条）+ candidates/principles.md（36 条），共 70 条。
> cases.md（23）/counter-examples.md（19）/glossary.md（28）按任务约定作素材池（A1 案例 id / 反例 id / 术语 id），不参与独立成 skill。
> 验证标准：V1 跨域 2 个独立语境 / V2 书外新问题外推 / V3 独特性。2015 年玩法参数类候选若只剩操作细节倾向淘汰；AARRR/PMF/MVP 等公共概念本身不通过 V3，但本书操作化判据可以。

## 统计

| 项目 | 数值 |
|---|---|
| 输入候选 | 70（frameworks 34 + principles 36） |
| 去重合并成独立单元 | **21**（将双池提取的同一方法论合并，保留全部出处 id） |
| 淘汰（rejected/） | **5**（f18、f31、f32、p13、p32） |
| 并入单元作降级素材 | 44（含 f15/p02/p16/p28 等：不独立成 skill，作为单元内素材与论据保留） |
| 独立成 skill 率 | 21/70 = 30%（方法密集实操书正常区间 30–70% 下沿；合并是主因，非质量差） |
| 主题聚类 | 8 个域：PMF 验证 / 获客 / 激活 / 留存 / 收入 / 传播 / AARRR 元层 / 职业道德 |

相邻单元边界互斥说明：种子筛选（准入）≠ 内容营销（渠道执行）；A/B 规范（实验方法）≠ 激活引导（魔法数字）；留存诊断（度量+归因）≠ 唤醒机制（流失召回通道）；K 值设计（病毒度量与心理）≠ 借势营销（热点时机运营）≠ 体外循环（主产品外增长体系）。

---

## 单元清单（21 个，按聚类排列）

### 域一：PMF 验证（4）

```yaml
id: U01
title: 需求真伪四问检验器
type: framework
merged_ids: [f05, p03]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章需求分析：真伪/刚性/量与肥/变现四维依次过筛（QQ邮箱附件聚合伪需求、搜狗三级火箭与VeryCD变现路径）
    - 第2章反例线：QQ邮箱附件功能上线一天即撤——真伪问的直接证伪场景
    - 第2章叮咚小区复盘：需求从真伪到设计全是硬伤即重金推广，四问缺失的代价场景
V2_predictive_power:
  passed: true
  novel_question: "AI 时代一句话就能生成一个'看起来需求很真'的产品创意，立项前怎么快速判断要不要做？"
  derived_answer: "四问过筛：①有没有可观察的客观行为证据（而非臆断）②涨价20%用户还用吗（刚性）③目标用户基数×付费能力×意愿预算够不够肥④谁付钱、变现路径是否成立。错误方向的问题拖到上线后修复，代价是立项阶段的68~200倍——四问是最便宜的质量关。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'要想清楚需求'；本书给出可执行的判据序列（四维依次过筛）+ 量化依据（68~200倍成本定律 + 40%~60%问题埋在需求阶段），是操作化而非口号。"
cluster: pmf-validation
proposed_slug: demand-four-questions
```

```yaml
id: U02
title: PMF 前置决策门（达成前禁止推广与过量优化）
type: framework
merged_ids: [f04, p01, p02]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章叮咚小区：1亿元推广加速垮塌的反面场景（O2O）
    - 第2章Instagram：从Burbn数据发现真实需求、砍功能转型达成PMF的正面场景
    - 第2章'真正的浪费是错误方向上高歌猛进'：方向先于速度的原则表述
    - 第3章开头作者再次提醒'先确认PMF再谈获取用户'——跨章复现
V2_predictive_power:
  passed: true
  novel_question: "融资到账后，团队该先扩招还是先加投放预算？"
  derived_answer: "过决策门：先出示PMF证据（留存曲线走平、自发口碑、复购），无证据则扩招与投放都在放大沉没成本——扩张速度越快，负面口碑累积越快。"
V3_exclusivity:
  passed: true
  why_not_common: "PMF 概念是公共的（Andreessen），但'达成前禁止推广/过量优化/烧钱扩张'的三禁止决策门 + '以留存曲线而非用户口头意愿作证据'的判据，是本书的操作化贡献。"
cluster: pmf-validation
proposed_slug: pmf-gate
```

```yaml
id: U03
title: MVP 验证器（双假设 + 形态选型 + 三大必备模块）
type: framework
merged_ids: [f06, f07, f08, p05, p06, p07, p33]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章 Dropbox：3分钟视频验证价值假设（等候名单5000→75000）
    - 第2章 Sendwithus：28美元假门网站用按钮点击做需求投票
    - 第2章 悠泊：微信公众号'产检'版一周上线、首日10单
    - 第2章云诺教训 + 第2章多啦口袋事故：MVP 漏掉反馈/升级/兼容模块的两种反噬（跨产品线独立证据）
    - 第8章 GitHub：'先交付再修bug'的持续交付印证
V2_predictive_power:
  passed: true
  novel_question: "想验证'宠物主是否愿意为 AI 宠物体检 App 付费'，不写一行代码怎么验？"
  derived_answer: "先锁定双假设（价值：是否满足需求；增长：是否愿买单），按成本选形态（假门网页收集点击投票 / 微信公众号承接服务 / 宣传视频测需求热度），且反馈渠道+公告+统计开关三个模块从第一天就带上，否则验证成功后无法触达验证用户。"
V3_exclusivity:
  passed: true
  why_not_common: "MVP 是公共概念，但'形态选型器（视频/手工服务/假门/公众号/暴力拼图按验证目标与成本选择）'与'上线第一天必备的反馈/公告/自动升级/统计开关清单'是本书沉淀的操作化判据；'MVP≠便宜难看残破'的澄清也纠正了最常见误用。"
cluster: pmf-validation
proposed_slug: mvp-validator
```

```yaml
id: U04
title: "行胜于言"用户调研法（付费意愿校准意见权重）
type: framework
merged_ids: [f09, p04]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章追TA'一键标为已读'：访谈全员支持、上线使用率远低预期（炫耀异性缘>防骚扰）
    - 第2章强制填资料调研：100%受访者称重要、实装吓跑新用户
    - 第2章健身房之喻：99人口头愿意、掏钱时畏缩——付费意愿才是标尺
    - 第2章 Sendwithus：用假门按钮点击（行为）而非访谈做需求投票
V2_predictive_power:
  passed: true
  novel_question: "用户访谈10个人有8个说想要深色模式，做不做？"
  derived_answer: "先查行为证据：有没有人用第三方插件/夜间模式替代？再设付费或付出门槛（愿意付费用户的意见权重高于免费评论家）；口头一致性恰恰是失真信号。"
V3_exclusivity:
  passed: true
  why_not_common: "'看行为不听口头'接近常识，但'付费意愿作为意见权重校准标尺'与'付费过程本身让用户更认真提建议'是本书给的可操作加权规则。"
cluster: pmf-validation
proposed_slug: actions-over-words
```

### 域二：获客（3）

```yaml
id: U05
title: 种子用户筛选与冷启动（含产品蝗虫甄别、排队准入设计）
type: framework
merged_ids: [f10, f11, f14, p08, p09, p12]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章筛选机制：知乎邀请制、B站100题、小米100个梦想赞助商、Facebook校园限定
    - 第3章/第8章 Tinder：先女后男、先渗透派对圈高势能节点（另一独立对象）
    - 第8章美丽说：500元/月请QQ群主带人、禁男性注册守生态
    - 第3章产品蝗虫：邀请码后台一半IP来自竞品内网、女性社区涌入男性——数据甄别场景
    - 第3章排队机制：Mailbox分批导入、Robinhood邀请插队、付费跳队筛选（Trak.io反例边界）
V2_predictive_power:
  passed: true
  novel_question: "冷启动是先冲1万注册量，还是先想办法只放100个精准用户进来？"
  derived_answer: "贵精不贵多：早期用户质量决定氛围与运营走向。先选筛选机制（邀请制/答题/付费/先攻高势能人群），并用数据日志排除蝗虫（竞品IP、观光客、乱提体验意见者）后再解读早期数据；排队/邀请码只对本身有吸引力的产品成立。"
V3_exclusivity:
  passed: true
  why_not_common: "'产品蝗虫'是作者独有术语体系；筛选机制工具箱（先女后男、答题门槛、超级粉丝测试——'没有它你愿付费维系吗'）与排队双面解读（从众强化+付费跳队验证商业价值）是可执行判据。"
cluster: acquisition
proposed_slug: seed-user-selection
```

```yaml
id: U06
title: "从最笨的事情做起"冷启动打法（人工补课式增长）
type: framework
merged_ids: [f12, p10]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章 Airbnb：租相机挨家挨户帮房东拍照，周营收200→400美元，后制度化
    - 第3章聚美优品：创始人注册女性马甲写BB霜软文，几十万销售额
    - 第3章 Strikingly：创始人加2000个用户逐个聊天
    - 第3章有道云协作：内部50人高强度试用再分层扩大内测
V2_predictive_power:
  passed: true
  novel_question: "拿不到任何应用商店推荐位、也没有投放预算，第一批客户还能从哪里来？"
  derived_answer: "人工补课选型：按获客卡点选择最笨动作——内容缺失就人肉生产（马甲软文/上门拍照），信任缺失就一对一陪聊，供给缺失就手工服务。判据：渠道红利不可得时，人工补课是唯一可控杠杆，且顺带建立对用户的真实理解（磨刀不误砍柴工），规模化后应制度化而非一直人扛。"
V3_exclusivity:
  passed: true
  why_not_common: "与 Paul Graham 'Do things that don't scale' 同源，但本书给出中国语境的适用判据（何时人工、补哪一环、何时功成身退）与多个本土实证，属于操作化而非格言。"
cluster: acquisition
proposed_slug: do-things-that-dont-scale
```

```yaml
id: U07
title: 内容营销引擎（三作用 + 持续输出）
type: framework
merged_ids: [f13, p11, f15]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章 KISSmetrics：内容贡献82%流量的流量场景
    - 第3章 OkCupid OkTrends：内容博客成为新用户首要来源（另一独立对象）
    - 第3章知乎：整理站内优质回答做持续输出引擎（平台型对象）
    - 第3章聚美马甲软文：内容直接劝诱转化的转化场景（第8章复盘亦引）
V2_predictive_power:
  passed: true
  novel_question: "老板要求做出一篇'10万+爆款'，团队该怎么办？"
  derived_answer: "拒绝一次性爆款思维：内容营销三作用（引流/培养潜在用户/劝诱转化）需要7次重复提醒才转化，应搭建持续输出引擎——明确受众、固定选题机制、标题多版本测试、鼓励互动晋级传播者、选对发布渠道；单篇爆款是引擎的副产品。"
V3_exclusivity:
  passed: true
  why_not_common: "'打造内容引擎而非赌爆款'与'三作用定位'是本书的方法框架；区别于泛泛的'内容很重要'。"
cluster: acquisition
proposed_slug: content-marketing-engine
```

### 域三：激活（4）

```yaml
id: U08
title: A/B 测试操作规范（铁律 + 失败率预期 + 微优化边界）
type: framework
merged_ids: [f16, p14, p15, p16, p17]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章铁律三原则：双方案并行、单变量、预设判优标准
    - 第4章微软/谷歌失败率：仅1/3有效、12000+次仅10%带来业务变化——预期管理场景
    - 第4章百姓网'投递简历'：架构扭曲导致测试结论失真的移动端场景
    - 第4章 OkDork/Twitter：着陆页删干扰、聚焦行动召唤的实战场景
V2_predictive_power:
  passed: true
  novel_question: "设计团队为按钮颜色吵了一周，谁拍板？"
  derived_answer: "三个条件满足就交给A/B：双方案并行、只变一个变量、预先定好判优标准；数据面前审美和职级都失效。但先过体量判据：未到'0.x%波动=百万美元损失'的规模，精力应投向跃进式改变而非41种蓝。"
V3_exclusivity:
  passed: true
  why_not_common: "单变量原则是实验法常识，但'多数测试注定失败'的失败率预期管理 + 微优化陷阱警示 + '测试架构本身扭曲用户选择空间'的失真判据（结论与用户反馈冲突时先怀疑测量方法）是本书的组合性贡献。"
cluster: activation
proposed_slug: ab-testing-protocol
```

```yaml
id: U09
title: 激活优化（魔法数字探查 + Aha 前置 + 降门槛绕路）
type: framework
merged_ids: [f17, f19, p24]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章 LinkedIn：A/B 测出邀请魔法数字"4"（少于4被忽略、多于4生焦虑）
    - 第4章 Twitter：新用户关注5-10人留存更高→注册末尾强制推荐关注
    - 第5章 Quora/Pinterest：把活跃用户标准动作引导给新用户、预订阅推荐账号'有事可做'
    - 第4章降门槛：Skype游戏声道伪造立体声、QQ音乐图片法锁屏歌词、WiFi万能钥匙截屏+OCR绕封闭API（技术受限的独立场景群）
V2_predictive_power:
  passed: true
  novel_question: "注册转化尚可但新用户次日几乎全走光，先优化哪一步？"
  derived_answer: "从留存数据反推与留存强相关的关键行为（社交产品=关注N人/完善资料），把它做成注册流程的默认引导（魔法数字）；若关键行为被技术/平台卡住，用'要结果不要路径'的绕路方案先降门槛——两条腿缺一不可。"
V3_exclusivity:
  passed: true
  why_not_common: "'魔法数字'是本书引进并操作化的术语体系：找留存相关行为→做成默认引导→A/B校准参数的三步流程，与'绕路实现'的工程化降级思路，都是可执行判据而非'要抓好新手引导'的空话。"
cluster: activation
proposed_slug: activation-aha-magic-number
```

```yaml
id: U10
title: 补贴模式升级路径（返利→限期券→现金→红包）
type: framework
merged_ids: [f20, p18]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章滴滴快的现金大战：补贴一停订单急剧下降的悬崖场景（程维自述）
    - 第4章滴滴打车红包：必须分享才能使用、最大红包往往流向新客（升级场景）
    - 第4章限期优惠券：针对预估流失周期做挽回的独立场景
    - 第6章微信红包溯源：9天4000万封的关系链机制参照
V2_predictive_power:
  passed: true
  novel_question: "预算只够支撑一轮补贴，发现金券还是做分享红包？"
  derived_answer: "按演进序列判断：现金只影响单次决策、买不来留存；让补贴必须经关系链流动（红包），一次预算同时完成拉新+留存+传播；并预演'停止补贴后的留存曲线'再决定形式。"
V3_exclusivity:
  passed: true
  why_not_common: "'现金→红包'的本质区别（关系链二次传播能力）与'抢到最大红包的永远是从没用过滴滴的人'的补贴流向判据，是本书对补贴方法论的独特提炼。"
cluster: activation
proposed_slug: subsidy-ladder
```

```yaml
id: U11
title: 游戏化 PBL 设计与"锦上添花"边界
type: framework
merged_ids: [f21, p19]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章 Foursquare：徽章/地主早期疯狂增长、核心搜索被挤掉后停滞（反例场景）
    - 第4章星巴克星享卡/Duolingo徽章：成熟产品的放大器场景
    - 第4章滴滴'滴米'：用游戏化调度B端接单意愿（供给侧场景，与C端独立）
    - 第4章 Waze：点数识别并提拔社区领袖（社区治理场景）
V2_predictive_power:
  passed: true
  novel_question: "产品增长乏力，要不要上排行榜和徽章体系救一下？"
  derived_answer: "先回答'产品对用户的核心价值是什么'：游戏化只能锦上添花不能雪中送炭——产品价值成立时PBL是放大器，不成立时排行榜只会加速暴露空洞（Foursquare把徽章置于搜索之上即反例）。四特征（目标/规则/反馈/自愿参与）齐备再上线。"
V3_exclusivity:
  passed: true
  why_not_common: "游戏化概念公共，但'只能锦上添花、不能雪中送炭'的红线判据与 PBL+地主身份的落地组合是本书给出的边界判据。"
cluster: activation
proposed_slug: gamification-boundary
```

### 域四：留存（3）

```yaml
id: U12
title: 留存诊断流程（真增长定义 + 三口径 + 品类基准 + 流失五分类 + 有损服务）
type: framework
merged_ids: [f22, f23, p20, p21, p22, p23]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章真增长=新增−流失：游泳池模式自欺的总命题
    - 第5章 40-20-10 规则与品类基准：游戏/电商/社媒各自达标线（对照场景）
    - 第5章流失五分类归因：Color（性能）、新浪微博（骚扰）、你画我猜（热度减退）三类独立样本
    - 第5章有损服务：QQ农场静态列表、微信放弃消息强一致、小米模糊库存、刀塔传奇低清资源包（降级取舍的独立场景群）
V2_predictive_power:
  passed: true
  novel_question: "DAU 还在涨但收入不涨，该从哪里查起？"
  derived_answer: "先看真增长：新增−流失的差值是否为正、留存曲线是否走平。三口径（次日/7日/30日）对照品类基准定位差距，按五分类归因（性能/骚扰/热度/替代品/其他）对症下药；若是性能硬伤，用有损服务两原则（保核心、少牺牲）先止血，而非继续拉新给漏水的池子灌水。"
V3_exclusivity:
  passed: true
  why_not_common: "任务指定的可过判据：40-20-10 法则与品类基准对照、流失五分类、'有损服务'术语及两原则，均是本书沉淀的操作化诊断体系；'真增长=新增−流失'的定义也修正了'看累计用户'的常见误读。"
cluster: retention
proposed_slug: retention-diagnosis
```

```yaml
id: U13
title: 唤醒机制三通道选型（EDM/推送/网页唤起）
type: framework
merged_ids: [f24]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章 EDM 四策略：奖励（GoDaddy/Pocket）、进展（Evernote）、个性化推荐（知乎每周精选/淘宝）、社交提示（Facebook被圈照片点击转化75%+）——邮件通道内四个独立机制场景
    - 第5章消息推送：日启动率可提540%但23%用户曾因推送卸载（风险边界场景）
    - 第5章网页唤起 App：Url Scheme/Chrome Intent 四级方案（技术通道场景）
V2_predictive_power:
  passed: true
  novel_question: "一批三个月未打开的流失用户，用什么方式唤回最合适？"
  derived_answer: "按触达深度分层选通道：可邮件/可推送/仅网页的不同层级用不同唤起方式；内容上选四策略之一（奖励/进展/个性化/社交提示）而非群发广告；且先自问'产品本身值得回来吗'——唤醒是补救手段，不是留存不足的替代品。"
V3_exclusivity:
  passed: true
  why_not_common: "'唤醒是补救而非替代'的定位原则 + 三通道×四策略的选型矩阵是本书的操作化框架；与'多发推送召回'的粗暴直觉相反。"
cluster: retention
proposed_slug: winback-mechanisms
```

```yaml
id: U14
title: 增长指标体系搭建器（North Star 共识 + 分析纪律 + 双套指标字典）
type: framework
merged_ids: [f02, f03, f34, p30, p31]
V1_cross_domain:
  passed: true
  evidence:
    - 第1章 Facebook 月活 vs 注册量：核心指标锚定品类价值的共识场景
    - 第1章 WhatsApp消息发送量/陌陌'登录并提交地理位置一次'：活跃定义因产品而异的独立对象
    - 第1章婴儿车-奶粉销量互证 + LinkedIn察觉雷曼访客骤增：数据交叉验证与异动预警的独立场景
    - 附录A 网站13项+移动13项：逐项口径陷阱与作弊识别（PV可刷iframe、总用户数有水分）
V2_predictive_power:
  passed: true
  novel_question: "各部门各报各的数，周会为'哪个指标更重要'吵不完怎么办？"
  derived_answer: "自上而下确立一个核心指标（锚定品类核心价值，通常一个就够），让团队在领导者不在场时仍能自行判断取舍；配套先有假设再取数据的分析纪律、跨指标互证习惯，并用附录A字典排除虚荣指标（可零成本刷出来的数字一律存疑）。"
V3_exclusivity:
  passed: true
  why_not_common: "North Star 概念公共，但'定义必须锚定品类核心价值+终结部门争执'的选型判据、'先有假设再取数据+数据间相互印证'的分析纪律、以及 26 项带口径陷阱注解的指标字典，是本书可复用的操作层。"
cluster: retention
proposed_slug: growth-metrics-system
```

### 域五：收入（2）

```yaml
id: U15
title: 免费-收费模式决策器（四支柱 + 砍免费版静默试验）
type: framework
merged_ids: [f25, p25]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章免费四支柱与前提：边际成本趋零+海量市场，'少数付费者补贴多数免费者'（Evernote付费率0.5%的参照）
    - 第6章 Bidsketch：免费用户撑不起付费率→静默删免费选项一周→转化率升8倍
    - 第6章 CrazyEgg：取消免费当月营收翻番（独立对象）
    - 第8章 GitHub：免费公开仓库+收费私有仓库的模式场景
V2_predictive_power:
  passed: true
  novel_question: "免费用户占了99%，成本快撑不住了，应该直接宣布收费吗？"
  derived_answer: "先过前提判据（边际成本趋零+海量市场+二八法则成立才玩得起免费）；不满足时不要直接砍——先静默从页面删除免费选项做一周A/B，验证付费用户数不变、转化率跳升后再公开切换；免费是手段不是目的。"
V3_exclusivity:
  passed: true
  why_not_common: "'静默砍免费版试验法'的操作顺序（悄悄删→验证→公开转付费）是本书给出的反直觉可复制流程，远比'考虑一下收费'具体。"
cluster: revenue
proposed_slug: freemium-decision
```

```yaml
id: U16
title: "变惩为奖"三原则（不责备、给补偿、给便利）
type: framework
merged_ids: [f26, p26]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章 QQ 会员'点灯事件'：1元淘宝代点灯波及300万人→转化15%非会员（越轨场景一）
    - 第6章 CleanMyMac：检测到盗版序列号→弹出49元中国区专属优惠页（越轨场景二，独立对象）
V2_predictive_power:
  passed: true
  novel_question: "发现大批用户在用盗版序列号/钻价格漏洞，该发律师函还是装看不见？"
  derived_answer: "堵不如疏，按三原则走：①绝不责备用户（选择受渠道与信息不对称影响，谴责只会粉转黑）②给予合理补偿（抵消'到手即失'的损失感）③提供转化便利（清晰引导、最简步骤、优惠价格）——把越轨者识别为'准付费用户'而非敌人。"
V3_exclusivity:
  passed: true
  why_not_common: "对越轨用户的常规直觉是封杀/追责，'变惩为奖'的三原则清单是反直觉且带实证（15%转化）的操作化框架。"
cluster: revenue
proposed_slug: turn-penalty-into-reward
```

### 域六：传播（3）

```yaml
id: U17
title: 病毒循环 K 值设计器（双指标 + 八种心理触发器）
type: framework
merged_ids: [f27, f28, p27]
V1_cross_domain:
  passed: true
  evidence:
    - 第7章 K 因子公式与双指标：K=感染率×转化率、病毒循环周期（度量框架）
    - 第1章 Hotmail：邮件签名内置传播因子，18个月1200万用户（覆盖面场景）
    - 第4章 LinkedIn 双重病毒循环：新用户带新用户+注册动作唤回老用户（循环结构场景）
    - 第7章八种心理：喜爱/逐利/互惠/求助/炫耀/稀缺/怕错过/懒惰各有独立产品案例
V2_predictive_power:
  passed: true
  novel_question: "邀请功能上线后 K=0.3，怎么知道该改哪里？"
  derived_answer: "拆双指标诊断：感染率低→扩充邀请渠道（通讯录之外的微博/邮件/二维码）；转化率低→优化着陆页与注册步骤、缩短操作路径；周期太长→一键分享+制造紧迫感。再为分享动作匹配至少一种心理触发器（互惠/炫耀/逐利…）并注意节制炫耀频次。"
V3_exclusivity:
  passed: true
  why_not_common: "K 因子公式是行业公共知识，但'双指标拆解定位瓶颈+循环周期速度观+八种心理逐一匹配触发器'的诊断与设计流程是本书的操作化贡献（任务指定 K 值设计可过 V3）。"
cluster: viral
proposed_slug: viral-k-factor
```

```yaml
id: U18
title: 体外病毒循环与病毒活动策划（三大考验 + 六要点 + 付出感设计）
type: framework
merged_ids: [f29, f30, p28, p29]
V1_cross_domain:
  passed: true
  evidence:
    - 第7章追TA整蛊H5：一个月700万参与、65万粉丝，同时暴露1%下载转化与平台封杀（圈人-筛选场景）
    - 第7章云诺'世界末日'点击领空间：微调控件付出感设计，日新增+400%（活动策划场景）
    - 第7章百度云1/1000价格 Bug 营销：话题简明可转述+修复拖延造窗口（话题场景，独立对象）
    - 第8章美丽说微博小测试：先分享才能看结果的单款10-30万授权（另一产品线）
V2_predictive_power:
  passed: true
  novel_question: "主产品本身没有传播性，想做个小活动引流，如何评估值不值得做？"
  derived_answer: "先过三大考验自检：创意能否一句话转述且不易被山寨？生命周期只有三五天到两周、有无换皮续命方案？引来的人群与主产品是否契合（垂直产品借大众爆款导流基本失败）？执行时按六要点（一句话创意/简单参与/成就时刻怂恿分享/留槽点/放开漏洞造二次传播/预备二三次传播方案），并让用户略微付出代价——付出感比直接白给更显价值。"
V3_exclusivity:
  passed: true
  why_not_common: "'体外循环三大考验''活动六要点''让用户略微付出代价反而更珍惜'（付出感>白给）都是本书的实操提炼，且自带平台风险与道德边界的清醒认知（追TA被微信干预、Bug营销涉价格欺诈）。"
cluster: viral
proposed_slug: external-viral-loop
```

```yaml
id: U19
title: 借势营销与"营销前置"思维
type: framework
merged_ids: [f33]
V1_cross_domain:
  passed: true
  evidence:
    - 第7章去啊vs去哪儿文案大战：小网站顺势露脸的热点爆发期场景
    - 第7章 SegmentFault 光棍节程序员闯关秀：注册量翻18倍的节点策划场景
    - 第7章猎豹'春运抢票版'：实为预装插件的老产品——营销前置（研发阶段植入卖点）的独立场景
V2_predictive_power:
  passed: true
  novel_question: "热点来了，追还是不追？追的话怎么不算白忙？"
  derived_answer: "按时机艺术判断：热点爆发期将推广融入用户语境（借势），话题须简明可转述、且与自身产品价值有真实连接；更高级是营销前置——在产品研发阶段就为可预测的节点（节日/周期性刚需）预埋卖点与节奏，而非临时跟风。"
V3_exclusivity:
  passed: true
  why_not_common: "'借势=时机的艺术'与'营销前置'（为营销而设计产品版本）是本书对热点营销的两层提炼；与 K 值设计（产品内机制）分属不同方法层。"
cluster: viral
proposed_slug: moment-marketing
```

### 域七：AARRR 元层（1）

```yaml
id: U20
title: AARRR 漏斗诊断定位法（元层框架）
type: framework
merged_ids: [f01]
V1_cross_domain:
  passed: true
  evidence:
    - 第1章定义：五环节拆解增长目标、减少每环损耗（总纲场景）
    - 第3-7章结构印证：每章对应一环、各环方法互不混用（章节级独立佐证）
    - 第8章五案例复盘：问题→手段→数据→启示均先定位漏斗环节再选方法（应用场景）
V2_predictive_power:
  passed: true
  novel_question: "增长全面停滞，预算和人力都有限，先从哪个环节下手？"
  derived_answer: "先做漏斗定位：用指标链（访问→注册→激活→留存→付费→分享）找出转化率最低的环节，只对该环节设计实验（获客卡住看渠道选型、激活卡住看魔法数字、留存卡住回PMF诊断），避免在非瓶颈环节浪费实验预算。"
V3_exclusivity:
  passed: true
  why_not_common: "AARRR 是 McClure 的公共框架，本身不通过 V3；通过的是本书的操作化用法——'定位卡点环节→对该环节单独设计实验'的诊断流程 + 与'真增长=新增−流失'的修正组合（防止把获取排第一误读为优先级）。"
cluster: aarrr-meta
proposed_slug: aarrr-funnel-diagnosis
```

### 域八：职业道德（1）

```yaml
id: U21
title: 增长职业道德红线三闸（换位思考 / 最小授权最大知情 / 契约精神）
type: framework
merged_ids: [p34, p35, p36]
V1_cross_domain:
  passed: true
  evidence:
    - 后记红线一：换位思考、己所不欲勿施于人（常识自问闸）
    - 后记红线二：最小程度的授权、最大程度的知情（权限闸；Path/SkillPages 通讯录滥用为独立反例）
    - 后记红线三：法无禁止即可为的空间是暂时的、谨守契约精神（长期闸；疯狂来往艳照门为预演）
    - 正文与后记的张力本身（Airbnb垃圾邮件/Bug营销 vs '不要把新手误带到沟里'）是作者自我校准的独立佐证
V2_predictive_power:
  passed: true
  novel_question: "新功能想默认上传用户通讯录来提升匹配精度，能做吗？"
  derived_answer: "过三道闸：①换位常识——站在用户立场，他们知道吗、会接受吗；②权限闸——逐项问'是否必要？用户是否已知？后果是否知情？'，最小授权、最大知情；③长期闸——今天法无禁止，明天监管收紧怎么办（疯狂来往即预演）。任何一闸不过即砍。"
V3_exclusivity:
  passed: true
  why_not_common: "在 GDPR/个保法之前的 2015 年，把道德约束操作化为'三道闸'并置于全书方法论之上，是作者的前瞻性贡献；'看似用智商压制了用户，却在道德上输得一败涂地'是差异化表述。今天虽成合规常识，作为增长手法的守门判据仍有独立价值。"
cluster: ethics
proposed_slug: growth-ethics-redlines
```

---

## 聚类总表

| cluster | slug | 包含候选 id | 覆盖内容 | A1 案例 id | 反例 id | 术语 id |
|---|---|---|---|---|---|---|
| pmf-validation | demand-four-questions | f05, p03 | 需求真伪/刚性/量与肥/变现四问 + 68~200倍成本定律 | c06 | x01, x02 | t03 |
| pmf-validation | pmf-gate | f04, p01, p02 | PMF 前置决策门、三禁止、错误方向浪费 | c03 | x01, x14 | t03 |
| pmf-validation | mvp-validator | f06, f07, f08, p05, p06, p07, p33 | 双假设、形态选型、三大必备模块、尽早交付 | c05, c06, c07, c21 | x04, x05 | t04 |
| pmf-validation | actions-over-words | f09, p04 | 行为>口头、付费意愿校准意见权重 | c06 | x03 | — |
| acquisition | seed-user-selection | f10, f11, f14, p08, p09, p12 | 种子筛选、蝗虫甄别、先女后男、排队准入 | c20, c22 | x06, x07 | t05, t06, t07 |
| acquisition | do-things-that-dont-scale | f12, p10 | 人工补课选型、最笨的事情 | c08, c18, c19 | — | t06 |
| acquisition | content-marketing-engine | f13, p11, f15 | 三作用、持续引擎、六要领、八段式文案 | c08 | — | — |
| activation | ab-testing-protocol | f16, p14, p15, p16, p17 | 铁律三原则、失败率预期、微优化边界、架构失真 | c02, c10, c12 | x09, x10 | t08 |
| activation | activation-aha-magic-number | f17, f19, p24 | 魔法数字、Aha 前置、降门槛绕路 | c02, c10 | — | t09 |
| activation | subsidy-ladder | f20, p18 | 返利→限期券→现金→红包演进 | c11 | x11 | t12 |
| activation | gamification-boundary | f21, p19 | PBL 组合、四特征、锦上添花红线 | c14, c17 | x08 | t11 |
| retention | retention-diagnosis | f22, f23, p20, p21, p22, p23 | 真增长定义、三口径、40-20-10、五分类、有损服务 | — | x12, x13, x14 | t15, t16, t26 |
| retention | winback-mechanisms | f24 | 三通道选型、EDM 四策略、补救非替代 | c02, c10 | x13 | t17, t18 |
| retention | growth-metrics-system | f02, f03, f34, p30, p31 | North Star、分析纪律、26 项指标字典、虚荣指标 | — | x19 | t14, t26, t27, t28 |
| revenue | freemium-decision | f25, p25 | 免费四支柱、五模式、砍免费版静默试验 | c12, c21 | x15 | t19, t27 |
| revenue | turn-penalty-into-reward | f26, p26 | 不责备/给补偿/给便利 | — | — | — |
| viral | viral-k-factor | f27, f28, p27 | K=感染率×转化率、循环周期、八种心理 | c01, c10 | x17 | t13, t21, t25 |
| viral | external-viral-loop | f29, f30, p28, p29 | 三大考验、活动六要点、付出感设计、Bug 营销 | c15, c16, c17, c22 | x17 | t22, t24 |
| viral | moment-marketing | f33 | 时机的艺术、营销前置、话题可转述 | — | — | t23 |
| aarrr-meta | aarrr-funnel-diagnosis | f01 | 五环定位→对环节设计实验 | c19, c22 | — | t02 |
| ethics | growth-ethics-redlines | p34, p35, p36 | 换位思考、最小授权最大知情、契约精神 | — | x18 | — |

## 降级素材注（未独立成 skill 但保留为单元素材）

- **f15 宣传报道文案八段式模板** → 并入 U07 content-marketing-engine 作执行层素材（模板+滑梯理论），不独立。
- **p02 真正的浪费是错误方向上高歌猛进** → 并入 U02 pmf-gate 作格言级论据。
- **p16 别让用户思考（着陆页三步）** → 并入 U08 ab-testing-protocol 作应用案例素材（OkDork 3%→8%、Twitter +250%）。
- **p28 让用户略微付出代价** → 并入 U18 external-viral-loop（与云诺案例强绑定，构成"付出感设计"要点）。
- **rejected 的 f18/f31/f32/p13/p32** 各自素材去向见 rejected/*.md。
- cases.md 23 条、counter-examples.md 19 条、glossary.md 28 条全部按上表挂接为 A1 案例 / 反例 / 术语素材；未挂接的 c04（与 x01 重复绑定 PMF）、c09（出海选市场，无框架候选承接，留作阶段 2 素材）、c13/c14（社交购物，挂 revenue 域作背景）等不丢失。

## 全集群通用时效警示（2015 年快照）

本书具体打法建立在 2014–2015 年平台生态之上，以下参数层**全部按当期重查，skill 只保留判断逻辑层**：

1. **开放平台红利**：微博/QQ 空间/人人开放平台的流量矿藏已枯竭，平台规则随时收紧（Zynga/五分钟之鉴 x16）——"借力大平台"逻辑保留，"薅平台羊毛"参数失效。
2. **补贴大战**：O2O 现金补贴被监管与资本周期终结——红包的关系链设计逻辑保留，撒钱参数不可复制。
3. **SEO/ASO 权重**：PR 值已成历史名词，ASO 关键词堆砌与评分引导（p13）被官方封禁/替代——"吃透分发规则"思想保留，规则本身须当期重查。
4. **微信规则**：诱导分享、H5 测试页、朋友圈小游戏的封杀持续加码（追TA之鉴）——体外循环必须先评估当期平台政策。
5. **邮件生态**：EDM 四策略在欧美有效、国内打开率极低——通道选型按目标市场替换（国内换短信/私域/推送）。
6. **重定向广告**：第三方 cookie 已被 ATT/GDPR/个保法终结（t20）——"再营销"逻辑保留，技术实现当期重查。
7. **统计口径**：书中无显著性检验/样本量讨论，40-20-10 与社媒 80% 等基准系圈内口传——作参考锚点而非硬标准。
8. **行为操纵手法**（诱饵效应、羞辱式引导、制造紧迫感）须锚定 U21 道德三闸与当代 dark pattern 批判整体降权引用。
9. **幸存者偏差**：案例全是赢家；外卖库（手法全可复制、成本近零仍被碾压出局）提示增长黑客是放大器而非护城河——引用任何案例数据时须带此前提。
