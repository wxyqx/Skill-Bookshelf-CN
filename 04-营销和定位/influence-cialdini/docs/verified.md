# verified.md — 三重验证通过的方法论单元

> 阶段 1.5 产出 | 候选池: 12 framework + 12 principle = 24 条
> 去重合并后: 11 个独立方法论单元
> 通过: 9 | 淘汰: 2 | 通过率: 82% (方法论密集型书籍，高于平均预期)

---

## 1. click-whirr — "卡嗒，哗"自动反应模型

- merged_from: [f01, p02(部分), g01, g02]
- supporting_cases: [c01, c02, c03]
- supporting_counter_examples: [ce10]
- supporting_glossary: [g01, g02]

```yaml
id: click-whirr
title: "卡嗒，哗"自动反应模型
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第一章: 绿松石珠宝价格翻倍 (c01) — "昂贵=优质"公式自动启动
    - 第一章: 雌火鸡与鸡貂 (c02) — 动物界的固定行为模式触发
    - 第一章: 蓝格"因为"实验 (c03) — 人类对"因为"一词的自动依从
    - 全书元框架: 六大原理 (互惠/承诺/社会认同/喜好/权威/短缺) 均以此为运作机制
V2_predictive_power:
  passed: true
  novel_question: "为什么人们在不知名餐厅更愿意点'招牌菜'而不是自己看菜单选？"
  derived_answer: "'招牌'二字是启动特征，触发了'专家选择=更好'的自动磁带。食客无需分析菜单——一个词语就绕过了对食材、口味、价格的理性比较。这与绿松石珠宝的'昂贵=优质'公式同构。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是'人有时不假思索就行动'。Cialdini 的独特贡献是:
    (1) 启动特征往往极其微不足道（一个词、一个价格标签），
        但足以绕过全部理性分析；
    (2) 信息过载使这种捷径依赖不是缺陷而是设计特征；
    (3) 识别启动特征 ≠ 识别整体——防御着力点在'按钮'而非'整体'。
```

---

## 2. contrast-principle — 认知对比原理

- merged_from: [f02]
- supporting_cases: [c07, c08]
- supporting_counter_examples: []
- supporting_glossary: []

```yaml
id: contrast-principle
title: 认知对比原理
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第一章: 原理定义和汽车经销商先看贵车再看便宜车的案例
    - 第二章: 拒绝—退让策略中大小请求的对比效应 (c07, c08)
    - 第五章: 好警察/坏警察中坏→好的对比放大 (f11引用)
    - 第七章: 短缺+竞争的对比增强
V2_predictive_power:
  passed: true
  novel_question: "房地产中介先带我看了三套破旧高价房，然后带我看一套中等房。我为什么觉得这套特别好？"
  derived_answer: "不是这套房真的好，而是前三套房是'锚定锚'，让中等房通过对比显得出色。原理明确指出：感知差异被放大。防御：不看前一套房，在纸上独立评估这套房的价格、面积、地段是否合理。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是'比较产生差异'。Cialdini 的独特贡献是:
    (1) 差异不是等比例呈现而是被'放大'——主观差异大于客观差异；
    (2) 这一放大效应可以被刻意利用——通过控制接触顺序来操纵感知；
    (3) 它是多种依从策略 (拒绝退让、好警察坏警察) 的'增强引擎'，
        理解这一点才能识别组合策略。
```

---

## 3. reciprocity-defense — 互惠原理：识别与防御

- merged_from: [f04, p01, p02, p09, g03]
- supporting_cases: [c04, c05, c06, ce01]
- supporting_counter_examples: [ce01]
- supporting_glossary: [g03]

```yaml
id: reciprocity-defense
title: 互惠原理的识别与防御
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第二章: 埃塞俄比亚给墨西哥捐款 (c04) — 跨文化、跨时间的互惠力量
    - 第二章: 雷根可乐实验 (c05) — 互惠压倒个人好恶
    - 第二章: 克里希纳会社募捐 (c06) — 不请自来的好处制造负债感
    - 第五章: 好警察/坏警察中互惠原理的运用 (f11引用)
    - 第二章: 拒绝—退让策略作为互惠原理的变体 (f07)
V2_predictive_power:
  passed: true
  novel_question: "一个SaaS销售先免费送我一本行业白皮书，再约产品演示。我是否有义务听他推销？"
  derived_answer: "先重新定义：白皮书是'礼物'还是'促销手段'？如果该白皮书系统性地发给所有潜在客户作为获客流程的一部分，它是促销手段→互惠义务被解除。但仍需警惕：'不请自来的好处'也能制造负债感 (p09)，即使你识破了它。防御关键是定义，不是拒绝一切。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是'受人恩惠要回报'。Cialdini 的独特贡献是:
    (1) 互惠允许不公平交换——小恩惠可触发大回报；
    (2) 不请自来的恩惠也产生义务感——负债感是被强加的；
    (3) 防御不是'一概拒绝'(p01: 会伤害真诚的人) 而是'重新定义'(f04:
        礼物→促销手段，定义后义务即解除)。
```

---

## 4. rejection-retreat — 拒绝—退让策略

- merged_from: [f07, g04]
- supporting_cases: [c07, c08]
- supporting_counter_examples: []
- supporting_glossary: [g04]

```yaml
id: rejection-retreat
title: 拒绝—退让策略 (Door-in-the-face)
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第二章: 童子军巧克力推销 (c07) — 个人日常消费场景
    - 第二章: 水门事件决策 (c08) — 重大政治决策场景
    - 第五章: 好警察/坏警察策略中互惠+对比的运用 (f11引用)
V2_predictive_power:
  passed: true
  novel_question: "软件供应商先报价100万/年，被拒后'打折'到60万/年。我该接受吗？"
  derived_answer: "第一个报价是'锚'，设计为被拒以使第二个显得合理。'打折'被感知为让步→触发互惠(对方让步→我也应让步) + 对比(60万 vs 100万显得便宜)。评估方法：忽略100万，问'60万/年的软件在市场上合理吗？'如果不知道100万，你还会觉得60万是'打折'吗？"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是'讨价还价'。Cialdini 的独特贡献是:
    (1) 拒绝退让是单方面设计的圈套，不是双方协商；
    (2) 被拒后的'退让'触发互惠原理(对方让步→我应回报)和对比原理(小请求显更小)；
    (3) 两个副产品：责任感(是我促成的)和满意度(对方终于让步了)，
        使受害者更可能履行承诺并继续合作。
```

---

## 5. commitment-consistency — 承诺和一致：识别与逃脱陷阱

- merged_from: [f05, f08, f09, p03, p04, p10, p11, g05, g06, g07]
- supporting_cases: [c09, c10, c20, ce02, ce03, ce07]
- supporting_counter_examples: [ce02, ce03, ce07]
- supporting_glossary: [g05, g06, g07]

```yaml
id: commitment-consistency
title: 承诺和一致：识别与逃脱陷阱
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第三章: 中国战俘营改造 (c09) — 入门策略+书面承诺+公开承诺的综合运用
    - 第三章: 玩具商圣诞策略 (c10) — 承诺的不可逆性
    - 第三章: 超自然冥想协会 (c20) — 机械一致作为逃避思考的避风港
    - 第三章: 莎拉和蒂姆 (ce03) — 承诺"长出自己的腿"
    - 第二章: 拒绝—退让策略中的责任感副产品 (f07关联)
V2_predictive_power:
  passed: true
  novel_question: "我答应帮朋友搬家，后来发现那天正好有个重要面试。为什么我还是觉得必须去帮忙？"
  derived_answer: "一旦口头承诺做出，一致原理开始施加内外压力。'长出自己的腿'——你开始找到新理由(朋友会失望、搬家很重要、做人要守信)。但这些理由可能在承诺前不存在。用'时间倒流测试'(p04): 如果一开始就知道有面试冲突，我会答应吗？第一闪念的'不会'就是真实判断。肠胃信号(p03)可能也会发出警告。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是'说到做到'。Cialdini 的独特贡献是:
    (1) 机械一致可以成为逃避思考的'愚昧的城堡'(ce02)——
        做出决定后播放'一致磁带'就不必再面对令人不安的现实；
    (2) 两层防御信号系统：肠胃信号(明确圈套) + 心灵信号(微妙操纵)；
    (3) 入门策略(f08)和抛低球(f09)利用承诺改变自我形象和创造新理由；
    (4) 公开(p10)和书面(p11)承诺具有不可逆的固化效果。
```

---

## 6. social-proof — 社会认同：多元无知与虚假证据

- merged_from: [f10, p05, p12, g08, g09, g10]
- supporting_cases: [c12, c13, c14, ce04, ce05, ce06]
- supporting_counter_examples: [ce04, ce05, ce06]
- supporting_glossary: [g08, g09, g10]

```yaml
id: social-proof
title: 社会认同：多元无知与虚假证据
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第四章: 吉诺维西谋杀案 (c12) — 多元无知在紧急事件中的致命后果
    - 第四章: 琼斯城集体自杀 (c13) — 社会认同在极端场景下的力量
    - 第四章: 维特效应 (c14) — 相似性条件与模仿性自杀
    - 第四章: 虚假社会证据 (ce05) — 配音笑声、假采访
    - 第四章: 韩国航空KAL007 (ce06) — 自动导航的危险
V2_predictive_power:
  passed: true
  novel_question: "一个App Store应用显示'10万人下载，4.8星'，我应该信任它吗？"
  derived_answer: "社会认同原理使人自动认为'这么多人用=一定好'。但需检查(p12): (1) 证据是否独立——评论是否可以伪造？(2) 相似性——下载者的需求和我一样吗？(3) 不确定性条件——如果我不确定需要这个应用，社会证据的效力更强。虚假社会证据(ce05)的信号：所有评价完全一致(真实群体总有分歧)。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是'从众'。Cialdini 的独特贡献是:
    (1) 多元无知(g09)——不是冷漠而是误判，每个人都在找社会证据但都提供错误证据；
    (2) 相似性是社会认同的关键调节变量——与自己相似的人的行为影响最大；
    (3) 不确定性最大化社会认同——不确定时最依赖他人行为；
    (4) 维特效应(g10)——社会认同可影响生死决策；
    (5) 紧急求助策略(p05)——指定一人消除不确定性和责任分散。
```

---

## 7. liking — 喜好：分离人与交易

- merged_from: [f06, p06, g11, g12]
- supporting_cases: [c15, c16, c17]
- supporting_counter_examples: []
- supporting_glossary: [g11, g12]

```yaml
id: liking
title: 喜好原理：分离人与交易
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第五章: 拼板教室 (c15) — 合作创造好感
    - 第五章: 乔·杰拉德卡片 (c16) — 称赞的自动效果
    - 第五章: 信用卡徽章实验 (c17) — 关联原理的无意识运作
    - 第五章: 光环效应 (g11) — 外表吸引力的自动扩散
    - 第五章: 关联原理 (g12) — 与正面/负面事物的形象管理
V2_predictive_power:
  passed: true
  novel_question: "一个猎头和我聊了半小时，夸我项目做得好，提到自己也是Java出身。然后推荐一个岗位。我该考虑这个岗位吗？"
  derived_answer: "分离法(f06): 问自己'如果不是这个人推荐，我会对这个岗位感兴趣吗？'称赞(c16: 即使不真实也有效)和相似性(同是Java出身)都是喜好触发器。光环效应(g11)可能使你认为对方专业、可信。关键：好感的来源(称赞、相似性)与岗位本身的质量无关。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是'我们更愿意对喜欢的人说yes'。Cialdini 的独特贡献是:
    (1) 喜好可以由多种因素自动触发(外表、相似性、称赞、关联、接触与合作)，
        且当事人通常否认自己受影响；
    (2) 即使知道对方有求于己、称赞不真实，喜好仍然有效——这是'卡嗒哗'机制；
    (3) 防御不是'不受影响'(不可能) 而是'认知切割'——
        主动将提出请求的人与请求本身分离评估。
```

---

## 8. authority — 权威：两问验证法

- merged_from: [p07, ce08]
- supporting_cases: [c11, ce08]
- supporting_counter_examples: [ce08]
- supporting_glossary: []

```yaml
id: authority
title: 权威原理：两问验证法
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第六章: 密尔格兰服从实验 (c11) — 65%普通人服从到最高电压
    - 第六章: 护士耳药水事件 (ce08) — 95%护士准备执行有问题的医嘱
    - 第六章: 多个权威符号实验(头衔、衣着、身份标志)的跨场景证据
V2_predictive_power:
  passed: true
  novel_question: "一个LinkedIn资料显示'前Google首席工程师'的人推荐了一个付费课程。我应该因为他的背景就信任这个课程吗？"
  derived_answer: "两问法(p07): (1) 他是真正的专家吗？前Google首席工程师的专长可能是大规模系统架构，与课程内容(假设是数据分析)可能不匹配——检查权威的实质而非象征。(2) 他会对我诚实吗？如果他有课程分成或 affiliate 链接，利益关系使其可信度打折。两个问题将盲目服从转化为有选择的参考。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是'不要盲从权威'。Cialdini 的独特贡献是:
    (1) 权威的影响不需要真正的专家——头衔、衣着、身份标志等'象征'就足以触发服从；
    (2) 即使是训练有素的专业人士(护士)也会盲目服从权威象征；
    (3) 两问法将模糊的'要批判性思维'转化为两个具体可操作的问题：
        这个权威是真正的专家吗？他会说真话吗？
```

---

## 9. scarcity — 短缺：两步情绪防御法

- merged_from: [f12, p08, g13, ce09]
- supporting_cases: [c18, c19, ce09]
- supporting_counter_examples: [ce09]
- supporting_glossary: [g13]

```yaml
id: scarcity
title: 短缺原理：两步情绪防御法
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第七章: 理查德卖车策略 (c18) — 短缺+竞争的组合
    - 第七章: 巧克力小甜饼实验 (c19) — 短缺增强欲望但不增强体验
    - 第七章: 短缺情绪压制认知 (ce09) — 知识不足以防御
    - 第七章: 心理抗拒 (g13) — 自由受限产生恢复动机
V2_predictive_power:
  passed: true
  novel_question: "一个限时秒杀活动显示'仅剩3件，倒计时2分钟'。我心跳加速想买。我该怎么办？"
  derived_answer: "第一步(f12/p08): 心跳加速和紧迫感本身就是停止信号——'一个明智的依从决定中没有恐慌和狂热的位置'。暂停。第二步: 问'我为什么想要它？'如果为了使用(吃、穿、用)，短缺不改变功能——'短缺的小甜饼吃起来并不会味道更好'(c19)。如果为了拥有(稀缺感、社交资本)，短缺可作价格参考但不改变东西本身。心理抗拒(g13)可能使你更想要——但这是'恢复自由'的冲动而非对东西本身的需求。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是'物以稀为贵'。Cialdini 的独特贡献是:
    (1) 短缺引起的是情绪冲动而非认知判断，而知识(认知)不足以对抗情绪(ce09)——
        因此防御的第一步不是'理性分析'而是'用情绪冲动本身作为停止信号'；
    (2) 占有 vs 使用的区分——短缺影响拥有欲但不改变使用价值；
    (3) 心理抗拒(自由受限→恢复动机)是短缺效应的底层机制，而非东西本身的价值。
```

---

## 淘汰单元摘要

| id | title | 淘汰项 | 原因 |
|---|---|---|---|
| f03 | 柔道策略（利用自然之力） | V2, V3 | 只能推导出"用巧劲不用蛮力"的常识结论；"利用杠杆而非力量"非反直觉见解 |
| f11 | 好警察/坏警察策略 | V1 | 仅在第五章出现一次，无第二个独立语境佐证；是多原理组合的案例而非独立方法论 |

---

## → 进入阶段 2

以下 9 个单元将通过 RIA++ 构造为独立 SKILL.md:

1. click-whirr
2. contrast-principle
3. reciprocity-defense
4. rejection-retreat
5. commitment-consistency
6. social-proof
7. liking
8. authority
9. scarcity
