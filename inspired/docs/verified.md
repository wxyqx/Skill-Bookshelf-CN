# verified.md — 阶段 1.5 三重验证通过名单

> 合并去重：289 条候选（f46/p95/c54/x69/t25）合并为 41 个方法论单元，逐单元跑 V1 跨域 / V2 预测力 / V3 独特性。
> 通过 **18** 个（通过率 44%，符合方法论密集书 30–50% 预期）；23 个淘汰，见 `rejected/merged-units.md`。

---

## v01 — opportunity-assessment-ten-questions 机会评估十问

```yaml
id: v01
title: 机会评估十问
type: framework
merged_from: [f12, p28, p29]
V1_cross_domain:
  passed: true
  evidence:
    - 第11章：完整十问主体（产品价值/目标市场/市场规模/度量指标/竞争格局/凭什么是我们/市场时机/营销组合/必要条件/结论）
    - 第12章：产品探索以机会评估为起点（"第一周先评估产品机会"）
    - 第26章：敏捷环境下"用轻量级的机会评估方法替代冗长的市场需求文档"
    - 第40章：最佳实践第3条单独重申
V2_predictive_power:
  passed: true
  novel_question: "CEO 硬塞给你一个'必须做'的项目，怎么把话接住又不瞎干？"
  derived_answer: "十问照答一遍——即使改变不了 CEO 的决定，也明确了产品目标与度量指标，成功概率大幅提高（第11章原文给出此推演）；且第一问'要解决什么问题'能立刻暴露项目是否根本站不住。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'做个可行性分析'；作者的独特结构是：十问全部只问问题、严禁讨论解决方案（'把洗澡水和孩子一起泼掉'是作者命名的典型失败），且第一问'产品价值'最难回答——多数人答非所问只会报功能。"
→ 进入阶段 2
```

## v02 — discovery-execution-two-modes 产品探索与执行两阶段切换

```yaml
id: v02
title: 产品探索与执行两阶段切换（含流水线并行）
type: framework
merged_from: [f14, f15, p32, p33, p34, p12]
V1_cross_domain:
  passed: true
  evidence:
    - 第12章：主体——探索（定义正确的产品）与执行（正确地开发产品）是两种性质的工作，重心必须切换
    - 第22章：探索期"一天迭代好几次"的原型节奏 vs 开发期节奏
    - 第26章：敏捷环境中"产品经理和设计师的工作进度应该比开发团队领先一两个迭代周期"
    - 第28章：创业公司"先探索后扩张"的资源顺序
V2_predictive_power:
  passed: true
  novel_question: "高管总在开发中途插进新需求，怎么不伤和气地挡回去？"
  derived_answer: "因为执行阶段产品经理自己就是最大障碍（第12章原文），流水线并行给出了制度化答案：1.0 进入开发就开始定义 2.0，新需求全部纳入下一版本——挡回的理由从'我不想改'变成'我们有版本节奏'。"
V3_exclusivity:
  passed: true
  why_not_common: "常识认为'需求和设计是可排期的确定性工作'；作者断言产品探索是艺术、不可设定期限，且'所有公司其实都在做产品探索——只是用真实产品+全部开发时间做昂贵原型，让不知情的用户掏钱测试'——这是把创业失败翻译成流程语言的独特视角。"
→ 进入阶段 2
```

## v03 — product-validation-trio 价值·可用性·可行性三验证

```yaml
id: v03
title: 价值/可用性/可行性三验证
type: framework
merged_from: [f01, f26, p53, p13, p10]
V1_cross_domain:
  passed: true
  evidence:
    - 前言：十条规律第1条与第10条（三要求是产品经理的探索任务；认定后不可分割）
    - 第21章：三验证的完整操作（可行性测试/可用性测试/价值测试）
    - 第1章：交互设计师的目标定义即"可用性与价值"
    - 第5章：开发人员早期参与评估可行性（三种完善产品定义的方式之一）
    - 第12章：探索的输出定义即三要求
V2_predictive_power:
  passed: true
  novel_question: "团队说'功能全做完了，就等发布'，此时才发现没人想用，还来得及吗？"
  derived_answer: "来不及——这正是三验证要防的时刻。倒推：价值测试必须用原型在开发前完成，'只相信还不够，必须通过用户测试验证，好比不能因为开发人员相信代码没问题就允许发布'（第20章类比）。"
V3_exclusivity:
  passed: true
  why_not_common: "常识把三词当三个独立检查项；作者把它们定义为'产品经理存在的理由'——去掉任何一个，产品都不可能成功，且三者必须在写代码前用同一个原型同时验证，不是开发后的验收清单。"
→ 进入阶段 2
```

## v04 — minimal-product-definition 基本产品定义法

```yaml
id: v04
title: 基本产品（不可再减的定义法）
type: framework
merged_from: [f25, p51, p52, p19]
V1_cross_domain:
  passed: true
  evidence:
    - 第20章：主体——定义只满足基本要求的产品，通过用户测试后不可削减
    - 前言：规律10"去掉任何因素，都不可能达到预期的结果"
    - 第6章：过滤多余功能（"去掉这些功能，产品甚至会因为简单易用获得更多用户"）
    - 第26章：敏捷秘诀4"目标是设计出符合基本要求的产品"
V2_predictive_power:
  passed: true
  novel_question: "开发估算超期两个月，老板说砍功能赶工期，怎么办？"
  derived_answer: "如果定义的是基本产品，答案是延工期不砍功能——'你已经没有东西可削减了'；如果还能砍，说明当初定义的就不是基本产品，错误在定义阶段而非执行阶段。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'列优先级、砍低优先级功能'（MVP 式思维）；作者反其道：砍功能凑工期的结果'产品完全不是有机的整体'，'断腿的狗打不了猎'——宁延工期、不破坏基本产品完整性。"
→ 进入阶段 2
```

## v05 — hi-fi-prototype-as-spec 高保真原型替代产品文档

```yaml
id: v05
title: 高保真原型取代纸质产品说明文档
type: framework
merged_from: [f23, p49, p09]
V1_cross_domain:
  passed: true
  evidence:
    - 第18章：主体（"安息吧，纸质说明文档"）
    - 第19章：验证设计思路必须使用高保真原型，"完成其任务后应该被丢弃"
    - 第22章：原型测试是"最主要原因"
    - 第26章：用产品原型和用户故事替代厚厚的 PRD 的三个优势
    - 第28章：创业公司用原型代替说明文档招开发
V2_predictive_power:
  passed: true
  novel_question: "异地外包团队抱怨需求文档看不懂，来回邮件扯皮两个月，怎么办？"
  derived_answer: "文档是非母语+文字表达力有限时，'一定要借助高保真原型进行交流'（第18章异地沟通节）——原型让双方看同一个东西，歧义当场暴露。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'原型是设计辅助，文档才是交付物'；作者反转：原型就是交付物本体，且'使用高保真原型可以大大缩短产品上市时间'——因为纸质文档未经测试，问题全部推迟到开发期解决。附带纪律：'原型代码绝不能用在产品里，所有原型代码都是要废弃的'。"
→ 进入阶段 2
```

## v06 — prototype-testing-playbook 原型测试操作法

```yaml
id: v06
title: 原型测试操作法（物色→主持→判停）
type: framework
merged_from: [f27, f28, f29, p55, p56, p57, p58, p59, p60]
V1_cross_domain:
  passed: true
  evidence:
    - 第22章：完整操作手册（10条物色渠道/准备/环境/主持技巧/更新）
    - 第21章：价值测试与可用性测试同场进行的框架
    - 第16章：可用性测试作为市场调研工具的定位
    - 第29章："去用户住所、办公室、购物场所就地体验"
V2_predictive_power:
  passed: true
  novel_question: "测试者全程说'这里加个XX就好了'，这类口头需求要不要记下来做？"
  derived_answer: "不要——'用户如果知道自己想要什么，设计产品就不会这么麻烦了'；应该多观察操作少听抱怨，问'接下来希望发生什么'，口头加功能要求属于误导性提问训练出的吹毛求疵。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'找些用户问问意见'；作者给出可执行的独门细节：鹦鹉技巧（口述用户动作/重复其问题来代替引导）、判停标准（连续六位理解并欣赏价值即可收敛）、纠错阈值（两三个用户反映同一问题就动手）、开场纪律（五分钟还没开始测试就是话太多了）。"
→ 进入阶段 2
```

## v07 — charter-user-program 特约用户计划

```yaml
id: v07
title: 特约用户计划（charter user program）
type: framework
merged_from: [f20, p40, p41, x30, x31]
V1_cross_domain:
  passed: true
  evidence:
    - 第15章：完整方法（6人/大众10-15人、十项注意）
    - 第22章：物色测试者的第一渠道就是特约用户
    - 第38章：企业级产品第4条"挑选大约六位优秀的目标用户"
    - 第29章：观察实际用户而非尝鲜者（反面呼应）
V2_predictive_power:
  passed: true
  novel_question: "发帖招试用用户，居然没人报名，说明什么？"
  derived_answer: "第15章注意3直接给出：'很可能是因为产品要解决的问题不像产品经理想象的那么重要，将来也很难销售出去'——招募困难本身就是产品价值的免费验证，应重新考虑产品计划。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'找种子用户/内测群，人多越好'；作者的硬约束相反：绝不超过10人（否则无法深入）、不收费（否则伙伴变客户）、且必须区分特约用户与尝鲜者——后者能容忍缺陷，按其需求做出的产品'很可能只适合他们自己'。"
→ 进入阶段 2
```

## v08 — product-principles-priority 产品原则与优先级共识

```yaml
id: v08
title: 产品原则与目标优先级共识
type: framework
merged_from: [f16, f17, p35, p36, p37, p38]
V1_cross_domain:
  passed: true
  evidence:
    - 第13章：主体（产品原则定义+两类错误）
    - 第32章：拒绝特例产品的依据就是产品原则
    - 第17章：人物角色与产品原则同为团队共识工具
    - 第30章：大公司施展的前提是决策依据清晰
V2_predictive_power:
  passed: true
  novel_question: "产品会上两派吵了三小时僵持不下，请 CEO 拍板行不行？"
  derived_answer: "不行——'出现这种局面说明沟通方式有问题'，请高管定夺会激化矛盾；正确诊断是'多数团队对事实并无争议，而是对目标和目标优先级理解不同'，先按重要性排出目标顺序写在白板上，方案之争自然化解。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'价值观共识''对齐'这类空话；作者的独特处：原则必须排序（'最重要的究竟是易用性还是可靠性'）、区分产品原则与设计原则（'清晰导航'不是产品原则）、以及把会议冲突归因为优先级未对齐而非利益冲突。"
→ 进入阶段 2
```

## v09 — persona-driven-focus 人物角色聚焦

```yaml
id: v09
title: 人物角色聚焦（筛选功能+单一关键人物）
type: framework
merged_from: [f22, p46, p47, p48, x36, x37, x38]
V1_cross_domain:
  passed: true
  evidence:
    - 第17章：主体（五大用途+三项注意）
    - 第37章：大众网络服务第2条"按典型特征抽象用户类型"
    - 第22章：原型测试者的筛选要覆盖人物角色之外
    - 第11章：机会评估第二问"为谁解决这个问题"
V2_predictive_power:
  passed: true
  novel_question: "销售说'大客户山姆要这个功能'，客服说'老太太玛丽用不了'，听谁的？"
  derived_answer: "先问人物角色清单：产品这版的关键人物是谁——'就该添加对玛丽重要的功能；如果某项功能只是针对山姆的，就该被淘汰'；决定谁不是目标用户与决定谁是目标用户同样重要。"
V3_exclusivity:
  passed: true
  why_not_common: "设计界把人物角色当设计工具；作者的独特用法是产品管理决策工具：'每个发布周期竭尽全力让产品经理集中精力关注一类关键人物角色'、'宣称产品老少皆宜是自欺欺人'、人物角色必须来自面对面交流而非想象。"
→ 进入阶段 2
```

## v10 — emotion-based-demand 情感需求分析（恐惧·贪婪·欲望）

```yaml
id: v10
title: 情感需求分析（恐惧/贪婪/欲望）
type: framework
merged_from: [f40, p83, p84, p85, x57]
V1_cross_domain:
  passed: true
  evidence:
    - 第34章：主体（企业级买恐惧贪婪、大众买孤独/爱/自豪）
    - 第31章：苹果第三层"用户体验为情感服务"（四百美元的 iPhone 情感溢价）
    - 第35章：情感接纳曲线以情感需求驱动为底层逻辑
    - 第36章：视觉设计满足情感需求
V2_predictive_power:
  passed: true
  novel_question: "两个笔记应用功能一样，为什么一个收费贵三倍还有人买？"
  derived_answer: "从情感需求分析：它卖的可能不是记录功能（恐惧：怕丢资料）而是自豪感/身份认同；'只有从情感的角度重新观察市场上的产品和服务，你才能体会用户的真实感受'——并进一步推出真正的竞争对手可能是线下生活方式而非同类应用。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'讲功能、讲性价比'；作者断言'消费者购买产品大多源于情感需求'，且给出可操作的三分类（企业级=恐惧+贪婪；大众=孤独/爱/自豪），不同用户 subtype（eBay 的阔绰买家/折扣买家/竞价刺激买家）情感需求不同。"
→ 进入阶段 2
```

## v11 — irrational-user-signals 非理性消费者与新生测试

```yaml
id: v11
title: 研究非理性消费者，警惕技术爱好者（含新生测试）
type: framework
merged_from: [f41, f42, f43, p86, p87, p88, x58]
V1_cross_domain:
  passed: true
  evidence:
    - 第35章：主体（邦弗特访谈：情感接纳曲线五分类）
    - 第15章：尝鲜者警告（按其需求做出的产品只适合他们）
    - 第29章："应该选择实际用户作为观察对象，不要选择产品尝鲜者，更不能选择公司同事"
    - 第37章：口碑营销与核心用户（超理性消费者）的张力
V2_predictive_power:
  passed: true
  novel_question: "社区里最热情、天天提建议的极客用户，他的需求清单该不该优先做？"
  derived_answer: "不该优先——技术爱好者'购买产品仅仅因为采用了新技术，对技术本身痴迷，最容易误导产品经理'；应转而研究非理性消费者：情感需求被放大、为解决问题付出超常成本的愤怒用户，'大众的消费动机与非理性消费者类似'。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'深度用户/核心粉丝的意见最宝贵'；作者反转：技术爱好者最没有参考价值，非理性消费者才值得研究——大众不会因痴迷电池技术买普锐斯，但会像狂热环保主义者那样为情感买单。附带独门工具'新生测试'：用中学第一天的新生视角重新审视日常烦恼。"
→ 进入阶段 2
```

## v12 — special-product-defense 特例产品防御

```yaml
id: v12
title: 特例产品防御（说不的框架）
type: framework
merged_from: [f38, p80, x54, x40]
V1_cross_domain:
  passed: true
  evidence:
    - 第32章：主体（企业软件大客户+网络广告合同两个场景）
    - 第11章：诱饵之一"只要大客户提出要求，项目就直接上马"
    - 第38章：企业级第3条重申"一旦妥协，你就变成了定制软件商"
    - 第7章：特例产品=NPS 劣质收益
V2_predictive_power:
  passed: true
  novel_question: "广告主愿意签七位数合同，条件是首页改成他们的布局，接不接？"
  derived_answer: "不接——特例产品'混淆了客户需求和产品需求，必然使公司偏离正轨'；且网络广告'以牺牲长远的信誉为代价换取短期的访问流量'。替代路径：与客户梳理需求本质找通用解、通过系统集成商满足定制、或设计共赢合作方式。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'客户是上帝，大单要接'；作者给出制度性诊断：三条理由说明产品需求不能用户说了算（不知道要什么/不知道什么可行/用户间需求难统一），产品公司的本质区别就是满足大众需求——接特例等于改行做定制软件商，被合同绑死。"
→ 进入阶段 2
```

## v13 — metric-driven-improvement 指标驱动改进现有产品

```yaml
id: v13
title: 指标驱动改进（不做功能加工厂）
type: framework
merged_from: [f30, p61, x46]
V1_cross_domain:
  passed: true
  evidence:
    - 第23章：主体（保险网站投保流程 7%→15% 示例）
    - 第11章：注册成功率 9%→18% 收益翻倍的同类论证
    - 第25章：发布后用可量化指标评估表现
    - 第37章：大众网络服务的扩展性与客服成本指标
V2_predictive_power:
  passed: true
  novel_question: "季度规划时用户提了二十条功能请求，怎么定优先级？"
  derived_answer: "先量化漏斗：'能提高指标的功能才是你关注的重点'——把二十条请求映射到注册转化/留存等关键指标上，没有指标映射的请求降权；改进产品'不是简单地满足个别用户的要求，也不能对用户调查的结果照单全收'。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'收集需求→排期实现'（功能加工厂）；作者诊断'大多数产品团队实际上只是功能加工厂，添加新功能反而让产品更糟'，改进的杠杆藏在转化率数字里——9%注册成功率翻倍即可让收益翻倍，这类机会被'公司过于自负'掩盖。"
→ 进入阶段 2
```

## v14 — smooth-deployment 平滑部署

```yaml
id: v14
title: 平滑部署（版本更新的用户耐心管理）
type: framework
merged_from: [f31, p62, p63, x47]
V1_cross_domain:
  passed: true
  evidence:
    - 第24章：主体（用户反感七个原因+三种部署方式）
    - 第37章：大众网络服务第9条"部署前仔细测试，逐步过渡，步幅不可过大"
    - 第26章：敏捷秘诀8"除非达到产品经理的要求，否则不要轻易发布新版本"
    - 第38章：企业级第9条升级之痛
V2_predictive_power:
  passed: true
  novel_question: "改版上线被用户骂上热搜，紧急回滚还是坚持教育用户？"
  derived_answer: "都不是最优——事前就该并行部署：新旧版本同时运行、旧版本保留一段时间并公示最后期限、区域性逐步部署；'优秀的产品赢得的好感是宝贵的信任，不要轻易试探用户的耐心'。已发生则回滚并按增量部署重走。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'新版本=进步，用户会适应'；作者列出七条用户反感原因并断言'不是所有用户都喜欢新版本'——互联网时代坏口碑迅速传播，糟糕版本给竞争对手可乘之机。"
→ 进入阶段 2
```

## v15 — rapid-response-window 发布后快速响应阶段

```yaml
id: v15
title: 发布后快速响应阶段
type: framework
merged_from: [f32, p64, p65, x48]
V1_cross_domain:
  passed: true
  evidence:
    - 第25章：主体（发布后几天至一周全员待命）
    - 第23章：互联网服务"几乎实时的数据反馈"改进
    - 第37章：大众服务持续可用的客服压力背景
    - 第32章（反面）：特例产品挤占的正是响应资源
V2_predictive_power:
  passed: true
  novel_question: "产品刚发布，团队想立刻解散去开下一个项目，同意吗？"
  derived_answer: "不同意——'此时正是收集反馈、改进产品的最佳时机'，急于撤军是大忌；关键不是会不会出问题，而是能多快解决。企业级做法更极端：派人上门安装，'不安装好产品就别想离开'。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'发布=项目结束，庆功转入下一个'；作者定义了一个正式流程阶段：几天至一周内每天简短会议+分级响应，投资极小、回报'绝非其他项目阶段可比'。"
→ 进入阶段 2
```

## v16 — new-old-thing 新瓶装老酒

```yaml
id: v16
title: 新瓶装老酒（老需求+新技术）
type: framework
merged_from: [f39, p81, p82, p75, p85, x55]
V1_cross_domain:
  passed: true
  evidence:
    - 第33章：主体（谷歌搜索"饱和"市场翻盘、iPod 百种 MP3 中胜出）
    - 第34章："只要市场上还有蹩脚的产品，就有机会"
    - 第29章："创新不是发现新问题，而是用新方法解决已有的问题"
    - 第16章（反面印证）：市场调研定义不出新品，成功来自需求与可行方案的契合
V2_predictive_power:
  passed: true
  novel_question: "所在赛道已有巨头，创业还有戏吗？"
  derived_answer: "有——成功产品往往不是新鲜事物；两件法宝：对现有产品的缺陷洞若观火（可用性测试连竞品一起测）+ 跟踪新技术让'之前无法实现的方案变得可能'，'只要做到一次，你的产品将所向披靡'。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'找蓝海、避开红海'；作者直说这是媒体炒作出来的错误观念，'新瓶装老酒'——瓶（体验/技术/便利/价格）才是变量，酒（需求）早就在那里。"
→ 进入阶段 2
```

## v17 — user-research-limits 市场调研的边界

```yaml
id: v17
title: 市场调研的作用与边界（含"用户不知道自己要什么"）
type: framework
merged_from: [f21, p42, p43, p44, p45, x33, x34, x35]
V1_cross_domain:
  passed: true
  evidence:
    - 第16章：主体（调研工具能回答的6问 vs 不能回答的根本问题）
    - 第15章：用户研讨会式的间接交流不可替代面谈
    - 第33章：成功的两个认识之一是"深入理解用户需求"（调研只是手段之一）
    - 第11章：机会评估与调研的分工（价值判断 vs 事实收集）
V2_predictive_power:
  passed: true
  novel_question: "调研报告说'92%用户希望增加导出功能'，这算不算验证了需求？"
  derived_answer: "不算——'调查结果为获得解决方案提供了一条途径，但不是解决方案本身'，'哪怕所有用户都回答喜欢X特性，我们还是可以通过提供Y特性更实际地解决他们的需求'；调研能回答'谁在用、怎么用、卡在哪'，不能回答'该打造什么产品'。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'用户说的就是需求'或反向'用户是傻子别听'；作者给出精确边界：'我从来没听说过仅仅通过市场调研就成功定义出来的产品'，同时调研对完善现有产品极其有效——双面论断+用户研讨会三弊端（用户不知道什么可行/没见到产品不知道要什么/群体互动失真）。"
→ 进入阶段 2
```

## v18 — tech-headroom-20percent 20% 技术余量

```yaml
id: v18
title: 20% 技术余量（预防重写代码危机）
type: framework
merged_from: [f04, f05, p11, p15, x06, x09]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章：主体（20%自主时间/余量 headroom/eBay 1999 崩溃+三次重写）
    - 第37章：大众网络服务第3条"分配20%的资源专门为系统扩展做好准备"
    - 第29章（对照）：20%创新法则证明"预留自主时间"是作者反复使用的组织杠杆
V2_predictive_power:
  passed: true
  novel_question: "开发团队抱怨'必须停下来重写代码'，答应还是不答应？"
  derived_answer: "先看余量：平时给足20%就不会走到这一步；已发生则三步走——按团队估计上浮的可行计划、分块递增重写（哪怕九个月拖成两年也要让用户看到改进，占用25%-50%资源）、谨慎选择仅剩的用户可见特性。拒绝递增式重写=用户流向对手。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'技术债以后再说，先做功能'；作者用 eBay 濒临崩溃、Friendster 覆灭的案例断言'这类问题通常由产品管理失误引发——产品经理一直迫使开发团队满负荷工作'，余量不是工程福利而是产品生存保险。"
→ 进入阶段 2
```

---

## 通过名单汇总

| # | skill-slug | 中文 | 一句话 |
|---|---|---|---|
| 1 | opportunity-assessment-ten-questions | 机会评估十问 | 只问问题不谈方案的十问过滤法 |
| 2 | discovery-execution-two-modes | 探索与执行两阶段 | 定义产品是艺术，执行是工程，重心必须切换 |
| 3 | product-validation-trio | 三验证 | 价值/可用性/可行性在写代码前用原型同时验证 |
| 4 | minimal-product-definition | 基本产品 | 通过测试后不可削减，超支只延工期 |
| 5 | hi-fi-prototype-as-spec | 高保真原型即文档 | 原型取代 PRD，可测试才合格 |
| 6 | prototype-testing-playbook | 原型测试操作法 | 物色→主持（鹦鹉技巧）→判停（连续六位） |
| 7 | charter-user-program | 特约用户计划 | ≤10个开发伙伴，招不到=需求不成立 |
| 8 | product-principles-priority | 产品原则与优先级共识 | 分歧的本质是优先级未对齐 |
| 9 | persona-driven-focus | 人物角色聚焦 | 决定谁不是用户同样重要，每版聚焦一类人 |
| 10 | emotion-based-demand | 情感需求分析 | 企业买恐惧贪婪，大众买孤独自豪 |
| 11 | irrational-user-signals | 非理性消费者信号 | 警惕技术爱好者，研究愤怒的用户（新生测试） |
| 12 | special-product-defense | 特例产品防御 | 接特例=改行做定制软件商 |
| 13 | metric-driven-improvement | 指标驱动改进 | 别当功能加工厂，9%→18%收益翻倍 |
| 14 | smooth-deployment | 平滑部署 | 别试探用户的耐心 |
| 15 | rapid-response-window | 快速响应阶段 | 发布后一周是黄金窗口，关键是多快解决 |
| 16 | new-old-thing | 新瓶装老酒 | 老需求+新技术=所向披靡 |
| 17 | user-research-limits | 市场调研的边界 | 调研能完善产品，定义不出产品 |
| 18 | tech-headroom-20percent | 20%技术余量 | 预留自主时间，防重写代码危机 |
