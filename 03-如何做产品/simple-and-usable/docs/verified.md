# 三重验证产出 (阶段 1.5) — 《简约至上：交互式设计四策略》

> 输入：candidates/frameworks.md (36 条) + principles.md (61 条) 共 97 条方法论候选。
> 案例池 (43 条)、反例池 (32 条)、术语池 (16 条) 不独立成 skill：案例进 A1 段，反例进 B 段，术语进 GLOSSARY.md。
> **验证结果：97 条候选 → 20 个 skill 单元（全部通过 V1/V2/V3），2 条独立候选降级并入（f19、f14，见 rejected/），其余均以合并方式保留。**

---

## 通过验证的 20 个 skill 单元

### A. 认识与立场（第 1–2 章域）

```yaml
id: s01
title: 貌似简单排查
merged_from: [f34, p03]
V1_cross_domain:
  passed: true
  evidence:
    - 第1章: 貌似简单专节（三特征+三类假捷径）
    - 第2章: "不要指望你能教会用户多少东西，或者认为说明书可以帮助他们"——说明书假捷径在认识层的重申
V2_predictive_power:
  passed: true
  novel_question: "老板说'加个新手引导向导就简单了'，怎么回应？"
  derived_answer: "三特征命中（解决眼下问题+便宜+无争议）→ 打上貌似简单标签 → 向导剥夺控制权且越长体验越差 → 改问哪个功能该删。"
V3_exclusivity:
  passed: true
  why_not_common: "常识把向导/说明/助手当可用性补救；本书给出识别特征与机制（把失败责任推给用户、'所有人都知道有效所以失败也不追责'），并指出它们让事情更复杂。"
```

```yaml
id: s02
title: 简化的商业论证
merged_from: [f04, f05, p04]
V1_cross_domain:
  passed: true
  evidence:
    - 第1章: 公司方程式技巧（Peter Merholz）与重要性×可行性分档
    - 第1章: 汽车公司主管与"重要客户"反对案例——论证该方法的战场
V2_predictive_power:
  passed: true
  novel_question: "向 CEO 提议砍掉报表自定义功能被拒，怎么办？"
  derived_answer: "写公司方程式（续费×单价−支持成本），推演简化让支持成本降、续费升；再让各方按固定档次给重要性和可行性打分，右上角项先做——把设计判断变成商业命题。"
V3_exclusivity:
  passed: true
  why_not_common: "常识做法是'拿用户调研说话'；本书指出公司按赚钱和增长说话，给出方程式翻译+强制分档（防'什么都重要'）的组合工序。"
```

```yaml
id: s03
title: 简单基准描述
merged_from: [f06, p05, f14]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章: 描述要点的两种方式专节
    - 第2章: "在面对设计功能对照表而犹豫不决时，我就会暂时停下来，问我自己'做这个表是为了什么'"——基准的实际用法
    - 第8章: 巴黎地铁应用反例——没有基准时漏掉决定性细节
V2_predictive_power:
  passed: true
  novel_question: "团队为一个表单字段吵了两周，怎么收场？"
  derived_answer: "先写一句话基准（'用户 30 秒完成下单'）或使用情景，逐字段对照基准——吵的不是字段而是没有基准；附带乔布斯三阶段提醒：复杂感上升不是跑偏信号。"
V3_exclusivity:
  passed: true
  why_not_common: "常识直接改设计；本书要求先有成文的'简单'判断基准（一句话/使用情景两档按项目规模选），并把它作为后续一切取舍的自检句。"
```

```yaml
id: s04
title: 真实环境观察
merged_from: [f09, p06, p07, p08]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章: 走出办公室专节（经销商案例）
    - 第2章: 观察什么——办公室/家里/户外三类环境的干扰清单
    - 第2章: 橄榄球广告时段网站案例——环境决定行为的独立佐证
V2_predictive_power:
  passed: true
  novel_question: "餐饮商家总抱怨 POS 软件难用，测试室却全过，为什么？"
  derived_answer: "到店里看：午高峰单手持机、嘈杂、随时被打断——设计改为大按钮、短任务块、可在被打断的间隙生存，而非继续改功能。"
V3_exclusivity:
  passed: true
  why_not_common: "常识相信可用性测试与评审；本书断言'体验是否简约必须在纷乱环境中考察'，给出现成观察环境清单和'无法控制环境只能适应环境'的立场。"
```

```yaml
id: s05
title: 主流用户立场
merged_from: [f07, f08, p09, p10, p11]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章: 三种用户专节
    - 第2章: 为什么应该忽略专家型用户（iPod 遭嘲讽仍卖 2.4 亿台）
    - 第2章: "简单的用户体验是初学者、新手的体验，或者是压力之下的主流用户的体验"——压力推论的独立应用
V2_predictive_power:
  passed: true
  novel_question: "资深用户在论坛强烈要求自定义快捷键，做不做？"
  derived_answer: "先问这是哪类用户的声音（专家型=少数派）；用六组对照检查自己是否被带偏（立即做完 vs 先设偏好）；为主流用户说不——专家的判断有系统性偏差。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'听最活跃用户的'；本书给出三分类+标签不随年限升级+对技术的态度比使用时长更有解释力，并把'忽略专家'论证成可复述的商业案例。"
```

```yaml
id: s06
title: 掌控感与感情需求
merged_from: [f10, p12]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章: 简单意味着控制专节（"然后呢"连环追问）
    - 第2章: Things 应用案例——靠回答感情需求层脱颖而出
V2_predictive_power:
  passed: true
  novel_question: "用户抱怨记账 app 难用但又说不清哪里难用，怎么挖？"
  derived_answer: "从掌控感出发连问'然后呢'：需要掌控→怕账目失控→一次只想看本周→默认周视图+完成感——挖到感情需求层才有方案，而不是加功能。"
V3_exclusivity:
  passed: true
  why_not_common: "常识做用户访谈列功能清单；本书给的是从感情需求（掌控生活）向功能层连环下钻的固定问法，并断言简单首先是掌控感。"
```

```yaml
id: s07
title: 极端简单目标
merged_from: [f11, p15]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章: 极端的可用性专节（八组常规→极端替换）
    - 第2章: "争取你不可能达成的目标有一个重要的好处：保持正确的方向"——目标的作用机制
V2_predictive_power:
  passed: true
  novel_question: "性能目标定'响应快 20%'，团队达成后就松懈了，怎么设目标？"
  derived_answer: "升格为'瞬间响应'：达不成也不用于验收，用于让每次妥协都朝同一方向——目标是 20% 时缩短 1 秒即满足，一次次让步让产品越来越慢。"
V3_exclusivity:
  passed: true
  why_not_common: "常识要求目标 SMART 可达成；本书反其道用不可能达成的极端目标做方向舵（任何人可用/毫不费力/瞬间/不出错/混乱环境工作），并说明其在妥协时刻的防漂移作用。"
```

```yaml
id: s08
title: 用户故事法
merged_from: [f12, p13, p14]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章: 环境、角色、情节专节（皮克斯由外而内法）
    - 第2章: 好的用户故事四标准专节
    - 第2章: 描述用户行动的三规范（用户语言/不漏步骤/聚焦行为）
V2_predictive_power:
  passed: true
  novel_question: "需求文档全是功能列表，评审没人有感觉，怎么改？"
  derived_answer: "改写成故事：先环境（出差路上手机）、再角色（常被打断的销售）、后情节（30 秒记一笔）；四标准自检（简明/具体/可信/展示而非讲述）——'反复按备注核对'好过'她注重细节'。"
V3_exclusivity:
  passed: true
  why_not_common: "常识写 user story 只有'作为…我想要…'；本书给出电影式三层结构+固定回退路径（情节出问题回角色、角色出问题回环境）+展示而非讲述的执行规范。"
```

```yaml
id: s09
title: 分享认识
merged_from: [f15, p17]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章: 分享专节（Alan Colville 的 Telewest 案例，节省 300 万英镑）
    - 第2章: "跟参与项目的每一个人复述你的故事……直到你讲得自己都厌烦了"——执行的强度要求
V2_predictive_power:
  passed: true
  novel_question: "我不在场时产品决定总跑偏，怎么办？"
  derived_answer: "把认识压成三词判据（如'简单、稳定、快速'）公之于众，每次开会用它过滤提案（'这样能更简单、更稳定、更快速吗'）——让每个干系人都能独立判断。"
V3_exclusivity:
  passed: true
  why_not_common: "常识靠评审流程把关；本书的解法是把判据内化给所有人（你不在场决定也会被正确做出），并给出'讲到自己厌烦'的传播强度标准。"
```

### B. 四策略（第 3–7 章域）

```yaml
id: s10
title: 四策略总纲
merged_from: [f03, p01, p18]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章: DVD 遥控器思想实验归纳四类
    - 第4–7章: 四策略各占一章逐一展开（同一框架的四个应用场）
    - 第6章: "删除不必要的、组织要提供的、隐藏非核心的"——三策略合用口诀
V2_predictive_power:
  passed: true
  novel_question: "导航栏 12 项太乱，从哪下手？"
  derived_answer: "按序过四策略：先删（假想目标用户不需要的）→ 删剩的组织（按用户标准分组）→ 非核心隐藏（高级项收起）→ 都不行转移（交给搜索）——新技术方案本质仍是这四类。"
V3_exclusivity:
  passed: true
  why_not_common: "'少即是多'是口号；本书给出穷尽式四分类（任何简化方案都落进一类）+固定尝试顺序+可叠加性，来自大量真实方案的归纳。"
```

```yaml
id: s11
title: 删除策略
merged_from: [f16, f17, f18, f19, p19, p20, p21, p22, p23, p24, p25, p33, p22/f22 掌控感边界]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章: 砍掉残缺功能/沉没成本翻转专节
    - 第4章: "但我们的用户想要"逆向工程专节
    - 第4章: 删减过多专节（无按钮电梯）——删除边界的独立语境
V2_predictive_power:
  passed: true
  novel_question: "旧报表模块'当年花了三个月开发，删了可惜'，怎么判？"
  derived_answer: "举证责任反转：开发成本是沉没成本收不回来，唯一标准是它现在能发挥几分作用、保留额外导致多少成本（用户负担+维护）——答不出就删；同时对每个'要加X'的要求逆向工程出真问题。"
V3_exclusivity:
  passed: true
  why_not_common: "常识按'功能有没有人用'投票保留；本书翻转举证责任（为什么要留着它）、给'假如用户想'的替代问法（目标用户经常遇到吗）、64% 功能从未使用的实证，以及'删到不能再减'的控制感边界。"
```

```yaml
id: s12
title: 减速带清理
merged_from: [f21, p26, p27, p28, p29, p30, p31, p32]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章: 负担专节（减速带隐喻）
    - 第4章: 删除干扰因素专节（Zhu 研究：链接本身降低理解力）
    - 第4章: 删减文字/精简句子专节（克鲁格减半法、兰哈姆五规则）
V2_predictive_power:
  passed: true
  novel_question: "首页改版后用户说'说不上来就是累'，怎么查？"
  derived_answer: "逐个元素问'这是减速带吗'：删装饰线条、补充链接移文末、错误消息改成消除错误来源（对账单列表化）、文字删一半再删一半、选项收敛+聪明默认值——每个小负担对每次使用都收费。"
V3_exclusivity:
  passed: true
  why_not_common: "常识只审功能；本书把'看起来无害的小东西'重新定价为认知负担（减速带），并给出四类冗余藏身之所、视觉减法清单、防错优先于错误消息等具体工序。"
```

```yaml
id: s13
title: 组织策略
merged_from: [f36, f24, p34, p35, p36, p37, p38, p39, p43]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章: 是非分明专节（分类标准判定）
    - 第5章: 期望路径专节（公园土路）
    - 第5章: 围绕用户行为组织专节（注册步骤推迟简化）
V2_predictive_power:
  passed: true
  novel_question: "商品分类改了三版用户还是找不到东西，怎么定标准？"
  derived_answer: "问多位用户他们的分法，取众口一致且重复交叉最少的；不按字母表（不知道叫什么就完蛋）、不按格式（看文字时想看图）；围绕行为排序（查找→加购→付款），注册能推迟就推迟。"
V3_exclusivity:
  passed: true
  why_not_common: "常识按逻辑或内容属性分类；本书给标准的三重判定（用户是非分明+多数一致+重叠最少）+'期望路径'检验（感觉不错而非规划逻辑）+别按字母表/格式的反直觉规则。"
```

```yaml
id: s14
title: 视觉组织
merged_from: [f23, p40, p41, p42]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章: 分层专节（伦敦地铁图感知分层）
    - 第5章: 网格与大小位置专节（重要性 1/2→大小 1/4）
    - 第5章: 色标系统专节（学习成本与适用条件）
V2_predictive_power:
  passed: true
  novel_question: "表单 17 个字段挤在一起显得复杂，怎么收拾？"
  derived_answer: "不可见网格对齐（不改一字即可变简单）、重要性减半则大小减到 1/4、用颜色分 2-3 层让每次只感知一层、层间差别最大化（眯眼测试）、色标只给天天重复使用的用户。"
V3_exclusivity:
  passed: true
  why_not_common: "常识把视觉当美化；本书把颜色/大小/网格当信息架构工具（感知分层零学习成本 vs 色标要学习记忆），并给出可执行的自检动作。"
```

```yaml
id: s15
title: 隐藏策略
merged_from: [f25, f26, f27, p44, p45, p46, p47, p48, p49, p50]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章: 隐藏部分专节（三类可隐藏功能）
    - 第6章: 渐进展示与阶段展示专节
    - 第6章: 适时出现专节（《纽约时报》选词词典）
V2_predictive_power:
  passed: true
  novel_question: "设置页 40 个选项吓退新用户，怎么收拾？"
  derived_answer: "三类可隐藏判断（细节/选项偏好/地区信息）→ 渐进展示（默认只露核心，精确控制进扩展区）→ 不做自定义也不做自动定制 → 提示用应邀探索且放在用户关注点上（位置>大小）→ 适时出现。"
V3_exclusivity:
  passed: true
  why_not_common: "常识把隐藏当'收进更多菜单'；本书给完整工序：什么该藏（三类）+怎么藏（彻底隐藏+适时出现）+怎么提示（关注点模型、别贴'高级'标签）+为什么不做自定义/自动定制（衣柜被搬走）。"
```

```yaml
id: s16
title: 转移策略
merged_from: [f28, f29, p52, p53, p56, p57]
V1_cross_domain:
  passed: true
  evidence:
    - 第7章: 用户最擅长做什么专节（人机分工表）
    - 第7章: 转移专节（RunKeeper 平台分工）
    - 第7章: 信任用户专节（原型测试建立信任）
V2_predictive_power:
  passed: true
  novel_question: "注册表单要求电话必须 11 位不带符号，用户老填错，怎么改？"
  derived_answer: "结构化是机器的活：让用户按自然格式输入，机器识别；再过人机分工表（人擅长判断与少量输入，机器擅长记忆检索与格式化）——把格式校验的复杂性还给计算机。"
V3_exclusivity:
  passed: true
  why_not_common: "常识把自动化当银弹；本书给双向分工表（人/机器各擅长的清单）+平台长短板对照+转移前提（必须先相信用户能行，用原型测试建立信任），失败案例（智能旅行规划抢人的判断权）同样入册。"
```

```yaml
id: s17
title: 开放式体验
merged_from: [f30, f31, p54, p55]
V1_cross_domain:
  passed: true
  evidence:
    - 第7章: 菜刀与钢琴专节（开放界面模型）
    - 第7章: 创造开放式体验专节（合并相似功能为多用途工具）
V2_predictive_power:
  passed: true
  novel_question: "要不要做'智能推荐模板'功能？"
  derived_answer: "先检查它是不是'仅适合中级用户的便捷特性'（两头不讨好）；替代路线是开放式工具：合并相似功能成一个可命名的通用工具，把模糊性留给用户——用户自己定义成功。"
V3_exclusivity:
  passed: true
  why_not_common: "常识追求'聪明的产品替用户做对'；本书论证简单界面的最高境界是专家和主流用户各设目标（菜刀/钢琴），并给出'削减中级便捷特性'这个可操作的检查项。"
```

### C. 收尾与哲学（第 8 章域 + 第 1 章哲学）

```yaml
id: s18
title: 复杂性放置
merged_from: [f01, f02, p58, p59]
V1_cross_domain:
  passed: true
  evidence:
    - 第8章: 顽固的复杂性专节（Tesler 法则+四问）
    - 第8章: 银行对账单案例——简化用户侧的复杂性转移到代码与服务器
    - 第7章: 人机分工——同一法则在第 7 章的应用场（跨章呼应）
V2_predictive_power:
  passed: true
  novel_question: "四策略用尽，这个功能还是复杂，到此为止了吗？"
  derived_answer: "换问句：不是'怎么更简单'而是'复杂性放到哪里'——四问逐一过（自动化还是用户控制/专用按钮还是通用/一次完成还是分段/有意识还是无意识），把残留复杂性放到代价最小且用户感受不到的位置。"
V3_exclusivity:
  passed: true
  why_not_common: "常识追求消灭复杂性；本书立守恒律（复杂性像打地鼠，按下这边那边冒头），把设计终局问题改写为分配问题——这是统摄四策略的更高层原则。"
```

```yaml
id: s19
title: 细节支撑简单
merged_from: [f33, p60]
V1_cross_domain:
  passed: true
  evidence:
    - 第8章: 细节专节（巴黎地铁应用漏掉"方向"）
    - 第8章: "花上半天时间……也许就能把成千上万次愤怒的用户投诉消弥于无形"——瑕疵定价公式
V2_predictive_power:
  passed: true
  novel_question: "有人反对修一个'只省用户 3 秒'的小问题，怎么回应？"
  derived_answer: "用'瑕疵×用户数×频率'定价：百万用户每天用，3 秒累积成几年；高频路径上的微小缺口优先修——简单是整体印象，由最薄弱的细节决定。"
V3_exclusivity:
  passed: true
  why_not_common: "常识按'改动收益'排序，小瑕疵永远排不上；本书给出反直觉的规模乘法（微小瑕疵×百万用户=灾难），并以地铁应用在站台崩塌的亲历案例佐证。"
```

```yaml
id: s20
title: 简单的边界
merged_from: [f35, f32, p02, p61]
V1_cross_domain:
  passed: true
  evidence:
    - 第1章: 特征专节（夏克椅 vs 潘顿椅，简单≠极简主义）
    - 第8章: 简单发生在用户的头脑中专节（旅行社手册 vs 网站）
    - 第4章: 认知负担模型——"塞满"一侧的机制说明（跨章呼应）
V2_predictive_power:
  passed: true
  novel_question: "设计被砍到'性冷淡'，用户却说冷冰冰，哪错了？"
  derived_answer: "砍掉的是特征不是复杂性：特征源自方法/产品/任务（夏克椅耐磨 vs 潘顿椅可堆叠），应保留；同时对照另一边界——删干扰思绪的元素但不塞满每个像素，为用户的生活留白。"
V3_exclusivity:
  passed: true
  why_not_common: "常识把简单等同极简或留白风格；本书给出双边界模型：下防'删光个性'（特征应保留），上防'塞满到用户能力上限'（留白让用户填入自己的生活）。"
```

---

## 合并与降级说明（审计用）

| 原候选 | 去向 | 说明 |
|---|---|---|
| f34, p03 | s01 | 同一识别器（三特征+三类假捷径+各自破绽） |
| f04, f05, p04 | s02 | 方程式+分档排序是同一商业论证流程的两步 |
| f06, p05, f14 | s03 | 基准描述两法；f14（问题三阶段）作为 B 段"复杂感上升≠跑偏"的边界并入，不独立（V1 弱：仅一处专节+概述句，见 rejected/f14.md） |
| f09, p06, p07, p08 | s04 | 观察法+环境清单+两条格言 |
| f07, f08, p09, p10, p11 | s05 | 三分类、六组对照、忽略专家、压力推论同属"为谁设计" |
| f10, p12 | s06 | "然后呢"追问与掌控感原则互为表里 |
| f11, p15 | s07 | 同一目标替换清单 |
| f12, p13, p14 | s08 | 三层结构+四标准+行动描述规范同为故事工序 |
| f15, p17 | s09 | 判据内化方法与执行强度要求 |
| f03, p01, p18 | s10 | 四策略本体+加功能不可持续（动机）+多方案规则 |
| f16, f17, f18, f19, p19–p25, f22/p33 | s11 | 功能层删除全套；f19 见 rejected/f19.md；掌控感边界进 B 段 |
| f21, p26–p32 | s12 | 感知细节删除（负担/选择/干扰/错误/视觉/文字） |
| f36, f24, p34, p35, p36, p37, p38, p39, p43 | s13 | 信息架构层组织全套 |
| f23, p40, p41, p42 | s14 | 视觉层组织（分层/色标/网格） |
| f25, f26, f27, p44–p50 | s15 | 隐藏全套（什么该藏/怎么藏/怎么提示/为何不做自定义） |
| f28, f29, p52, p53, p56, p57 | s16 | 人机分工+平台分工+表单结构化+信任 |
| f30, f31, p54, p55 | s17 | 开放界面+多合一工具 |
| f01, f02, p58, p59 | s18 | 法则+四问 |
| f33, p60 | s19 | 同一细节命题 |
| f35, f32, p02, p61 | s20 | 双边界（≠极简 / 留白） |

**数量健康度**：通过率 97→20（21%），考虑到本书是策略手册而非论证密集型著作（大量候选为同一策略的操作细则），落在合理区间偏下；第 2 章 7 个（认识域最厚）、四策略各 1–2 个、第 8 章 3 个，结构分布与原书骨架一致。
