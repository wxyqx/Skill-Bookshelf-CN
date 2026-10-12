# verified.md — 三重验证通过的方法论单元

> 阶段 1.5 产出
> 候选池: 19 frameworks + 18 principles = 37 条
> 去重合并后: 13 个独立方法论单元
> 通过: 10 | 淘汰: 3 | 通过率: 77%

---

## 1. interdependence-assessment — 相互依赖关系评估框架

- merged_from: [f01, f02, p07, p12]
- supporting_cases: [c05投入模型, c12较小利益原则]
- supporting_counter_examples: [ce10对替代选择的关注, ce22不现实婚姻期望]
- supporting_glossary: [g07相互依赖理论, g08比较水平CL, g09替代比较水平CLalt]

```yaml
id: interdependence-assessment
title: 相互依赖关系评估框架
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第6章: 作为核心理论提出社会交换公式（结果=奖赏-代价，满意度=结果-CL，依赖度=结果-CLalt）
    - 第11章: 用投资模型（投入+满意度+替代选择质量）解释对冲突的反应方式
    - 第12章: 较小利益原则解释权力不平衡——对关系利益较少者拥有更多权力
    - 第13章: 用替代比较水平解释离婚决策——只有当替代选择更好时人们才会离开
V2_predictive_power:
  passed: true
  novel_question: "我对现在的关系不满意但又舍不得分手，这是为什么？"
  derived_answer: "根据相互依赖理论，满意度和依赖度是两个独立维度。你可能处于'不幸福但稳定'象限：结果低于你的期望（CL）所以不满意，但结果仍好于你的替代选择（CLalt）所以不会离开。替代选择可能是单身、其他追求者、或任何替代关系的选项。CLalt越低越离不开，不管满意不满意。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是"不开心就分手"。独特贡献在于:
    (1) 满意度和稳定性是两个独立维度——你可以不开心但离不开，
        也可以开心但有更好选择；
    (2) 决定你留不留下的不是你有多幸福，而是你有没有更好的选择；
    (3) 比较水平（期望）会随经历而上升——曾经让你惊喜的，
        习惯后就变成理所当然，满意度自然下降。
```

---

## 2. negativity-bias-ratio — 坏比好更有力量与 5:1 比例

- merged_from: [p01, p02]
- supporting_cases: [c13戈特曼四类夫妻]
- supporting_counter_examples: [ce05末日四骑士]
- supporting_glossary: [g12坏比好更有力量]

```yaml
id: negativity-bias-ratio
title: 坏比好更有力量与 5:1 黄金比例
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第6章: 作为一般原则提出——负面事件比同等正面事件影响更大
    - 第11章: 戈特曼发现正面/负面交流比率低于5:1的夫妻56%在四年后离婚
    - 第4章: 归因偏差中体现——坏行为的归因比好行为的归因影响更大
    - 第10章: 一次背叛造成的伤害需要多次善意才能修复
V2_predictive_power:
  passed: true
  novel_question: "我和伴侣平时挺好的，但一吵架就特别伤人，这样的关系有问题吗？"
  derived_answer: "关键看比率。如果平时有大量积极互动（欣赏、支持、幽默、亲昵），偶尔的激烈争吵不一定是问题。但如果正面互动少于负面互动的5倍，关系就有风险。一次深度伤害可能需要5次以上的积极事件才能抵消。问自己：我们之间好的时刻是坏的时刻的5倍以上吗？如果不是，问题不在于吵架本身，而在于积极互动太少。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是"打是亲骂是爱"或"只要有爱就能克服一切"。
    独特贡献在于:
    (1) 给出了具体的5:1量化比例——不是"尽量多做好事"
        而是精确到"至少5倍正面才能抵消负面"；
    (2) 负面的不对称性不是因为人小气，而是演化而来的心理机制
        （损失比收益对生存更重要）；
    (3) 仅仅"没有冲突"是不够的——还需要大量积极互动来缓冲。
```

---

## 3. relationship-mindset — 关系信念：宿命型 vs 成长型

- merged_from: [f10, p03]
- supporting_cases: [c10宿命信念vs成长信念研究]
- supporting_counter_examples: [ce09命运信念陷阱, ce06读心术]
- supporting_glossary: []

```yaml
id: relationship-mindset
title: 关系信念：宿命型 vs 成长型
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第4章: 明确提出两种关系信念体系及其对关系认知的影响
    - 第11章: 宿命信念者遇到冲突更倾向于逃避或结束关系，成长信念者积极解决
    - 第14章: 成长信念与关系维持努力正相关，宿命信念与离婚风险正相关
    - 第8章: 宿命信念者对"完美爱情"的期待使他们对伴侣更挑剔
V2_predictive_power:
  passed: true
  novel_question: "为什么我朋友每次恋爱一开始都觉得遇到了真爱，但几个月后就失望分手？"
  derived_answer: "她可能持有宿命信念：认为真爱是天注定的，找到对的人就应该完美。关系刚开始时一切都新鲜美好，符合'天造地设'的期望。但随着时间推移，不可避免地出现摩擦和不完美，这与'真爱就不会有问题'的信念冲突。宿命信念者不会认为关系需要经营，而是认为'找错人了'，于是结束关系去寻找下一个'对的人'，进入下一轮循环。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是"相信真爱"vs"不相信爱情"的简单二分。
    独特贡献在于:
    (1) 信念不是关于爱情是否存在，而是关于关系能否改变和成长——
        这是Dweck成长型思维在关系领域的具体应用；
    (2) 宿命信念包含一整套相互关联的错误信念（读心术、伴侣不会改变、
        每次性爱都应完美、男女截然不同等），不是单一观念；
    (3) 信念是可改变的——识别出自己的宿命思维是改变的第一步。
```

---

## 4. love-triangle-passion-decline — 爱情三角理论与激情消退

- merged_from: [f06, f07, p09]
- supporting_cases: [c11吊桥实验, c14斯滕伯格爱情三角]
- supporting_counter_examples: [ce22不现实婚姻期望]
- supporting_glossary: [g13爱情三角理论, g14浪漫之爱, g15相伴之爱]

```yaml
id: love-triangle-passion-decline
title: 爱情三角理论与激情消退规律
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第8章: 斯滕伯格三角理论（亲密+激情+承诺）作为爱情分类核心框架
    - 第8章: 双因素理论（生理唤醒+浪漫归因）解释吊桥效应等现象
    - 第6章: 浪漫激情随时间下降，因为比较水平上升和新奇感消失
    - 第13章: 激情消退是离婚的相关因素之一
V2_predictive_power:
  passed: true
  novel_question: "我结婚三年了，感觉激情少了很多，是不是不爱了？"
  derived_answer: "根据爱情三角理论，爱情有三个成分：亲密（热情、理解、分享）、激情（性唤醒、欲望）、承诺（决心、维护）。浪漫之爱（亲密+激情）的激情成分会自然减弱——不是因为不爱了，而是因为新奇感消失、比较水平上升、生理唤醒难以长期维持。更关键的是：亲密和承诺是否还在并持续增长？如果是，这是从浪漫之爱向相伴之爱的正常过渡，不是不爱了。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是"爱情会变亲情"或"婚姻是爱情的坟墓"。
    独特贡献在于:
    (1) 不是简单的"爱情→亲情"，而是三个成分各自变化——
        激情下降但亲密和承诺可以增长，是不同类型的爱而非"没爱了"；
    (2) 激情消退有具体机制（比较水平上升、新奇感下降、生理适应），
        不是抽象的"时间长了就这样"；
    (3) 双因素理论解释了为什么刺激情境（吊桥、恐怖片）能增强浪漫感——
        这给出了主动创造激情的方法。
```

---

## 5. self-expansion-boredom — 自我延伸模型与关系厌倦

- merged_from: [f05, p12(部分)]
- supporting_cases: [c07自我延伸模型研究]
- supporting_counter_examples: [ce20关系倦怠]
- supporting_glossary: []

```yaml
id: self-expansion-boredom
title: 自我延伸模型与关系厌倦
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第6章: 自我延伸模型作为关系动机理论提出
    - 第8章: 用来解释为什么新关系令人兴奋（快速自我延伸）而长期关系容易沉闷（延伸速度减慢）
    - 第14章: 关系维持策略中，共同参与新奇活动是预防厌倦的有效方法
V2_predictive_power:
  passed: true
  novel_question: "为什么我和伴侣在一起越久越觉得无聊，但一分开又想念？"
  derived_answer: "根据自我延伸模型，新关系令人兴奋是因为伴侣带来新知识、新体验、新角色——快速的自我延伸。在一起久了之后，彼此变得熟悉，自我延伸的速度减慢，关系变得沉闷。分开后想念是因为你想念的不是刺激感，而是亲密和陪伴（相伴之爱的成分仍然很强）。解决方法不是换人（换人只是重复同样的曲线），而是共同创造新的体验来重启自我延伸。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是"时间长了就腻了"。
    独特贡献在于:
    (1) 厌倦不是因为"不爱了"或"找错人了"，而是因为自我延伸速度减慢——
        这是正常的心理过程，不是关系失败的信号；
    (2) 解决方法不是换人（换人只是把曲线重新走一遍），
        而是主动创造新奇体验、学习新技能、进入新角色；
    (3) 这是有实证支持的理论（Aron等人的研究），不是鸡汤。
```

---

## 6. conflict-management-toolbox — 冲突管理工具箱

- merged_from: [f14, f16, f17, p04, p05, p06, p14]
- supporting_cases: [c13戈特曼四类夫妻, c15说话者听话者技术]
- supporting_counter_examples: [ce05末日四骑士, ce16要求退避模式]
- supporting_glossary: [g17辩证张力]

```yaml
id: conflict-management-toolbox
title: 冲突管理工具箱
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第11章: 冲突的性质、辩证张力、升级过程、解决方法
    - 第5章: 沟通技术（说话者-听话者技术）是冲突管理的核心工具
    - 第14章: 关系修复中的冲突管理部分
    - 第12章: 权力不平衡如何影响冲突模式（要求/退避）
V2_predictive_power:
  passed: true
  novel_question: "我和伴侣一吵架就冷战，谁也不理谁，这样好吗？"
  derived_answer: "冷战属于要求/退避模式中的退避一方——一方想讨论（要求者），另一方逃避（退避者）。这是一个自我强化的恶性循环：退避导致要求者更坚持，增加的压力使退避者更抵触。戈特曼的研究显示，逃避型夫妻也能维持稳定婚姻，但前提是双方都习惯回避且没有未解决的重大问题。如果只有一方回避另一方想讨论，这就是问题。建议用说话者-听话者技术结构化沟通，或约定'稍后再谈'但必须履行。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是"吵架伤感情，不吵就是好"或"夫妻床头吵架床尾和"。
    独特贡献在于:
    (1) 冲突不可避免（辩证张力永远存在），关键是怎么处理；
    (2) 不是"越少吵架越好"——多变型夫妻（频繁激烈但有智慧）
        也能维持稳定婚姻，关键是5:1的正负比率；
    (3) 提供了具体可操作的工具（说话者-听话者技术、戈特曼三不要、
        顺应原则），不是"好好沟通"的空话。
```

---

## 7. relationship-maintenance — 关系维持策略库

- merged_from: [f18, f19, p11, p18]
- supporting_cases: [c24关系维持策略, c25米开朗基罗现象, c28Lauer45年婚姻研究]
- supporting_counter_examples: [ce26维持失败模式, ce27自我控制耗竭]
- supporting_glossary: []

```yaml
id: relationship-maintenance
title: 关系维持策略库
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第14章: 专门一章讲关系维持和修复
    - 第6章: 相互依赖视角下的维持机制（顺应、牺牲、自我控制）
    - 第8章: 相伴之爱与长期关系维持
    - 第4章: 认知维持机制（积极错觉、认知相互依赖）
V2_predictive_power:
  passed: true
  novel_question: "结婚久了是不是自然就平淡了？有什么办法能保持幸福？"
  derived_answer: "满意度自然下降是正常的（比较水平上升、新奇感消失），但幸福不是被动维持的。研究发现最有效的维持策略是：(1)积极性（保持礼貌愉快，不是'反正老夫老妻了就不用讲究了'）；(2)保证（表达爱意和承诺，不是'都结婚了还用说吗'）；(3)分担任务（公平承担家务，不是'谁有空谁做'）。这些行为一旦停止，满意度就会下降——维持是持续过程，不是一劳永逸。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是"婚姻需要经营"但不知道具体怎么经营。
    独特贡献在于:
    (1) 有实证研究支持的具体策略清单和优先级（积极性>保证>分担任务）；
    (2) 认知机制（积极错觉、认知相互依赖、感知优越感）
        和行为机制同样重要；
    (3) 米开朗基罗现象——好的关系帮助你成为理想的自己，
        这是超越"维持现状"的成长型维持。
```

---

## 8. attachment-pattern-awareness — 依恋类型自我觉察

- merged_from: [glossary g02]
- supporting_cases: [c01依恋类型四分类]
- supporting_counter_examples: [ce01不安全依恋恶性循环]
- supporting_glossary: [g02依恋类型]

```yaml
id: attachment-pattern-awareness
title: 依恋类型自我觉察
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第1章: 依恋类型作为个体差异的核心维度
    - 第4章: 依恋类型影响社会认知——焦虑型更容易感知到拒绝
    - 第10章: 依恋类型影响嫉妒和压力反应
    - 第14章: 安全依恋型更容易维持健康关系，不安全依恋型需要更多努力
V2_predictive_power:
  passed: true
  novel_question: "为什么我一谈恋爱就变得特别黏人，对方稍微冷淡就焦虑得不行？"
  derived_answer: "你可能是焦虑-矛盾型依恋。这种依恋模式源于早期照料经历： caregivers的回应不一致，导致你对被遗弃高度敏感。进入亲密关系后，任何微小的距离信号都会触发强烈的焦虑反应。这不是'太爱了'，而是依恋系统的过度激活。关键觉察：焦虑时问自己——'我焦虑的是对方真的变了，还是我的依恋系统被触发了？'安全型依恋不是天生的，可以通过觉察和练习获得。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是"有的人就是缺乏安全感"或"恋爱脑"。
    独特贡献在于:
    (1) 依恋类型不是性格缺陷，而是早期依恋经历形成的关系认知模式——
        有明确的分类（安全/焦虑/回避）和行为预测力；
    (2) 不同依恋类型在关系中的典型行为模式不同——
        焦虑型怕被抛弃所以黏人，回避型怕被伤害所以保持距离；
    (3) 依恋类型不是固定的——安全的关系体验可以改变依恋模式，
        自我觉察是改变的第一步。
```

---

## 9. social-penetration-intimacy — 社会渗透与亲密建立

- merged_from: [f12, f13]
- supporting_cases: [c09社会渗透理论, c08曝光效应]
- supporting_counter_examples: [ce17羞怯自我实现循环]
- supporting_glossary: [g06匹配假设]

```yaml
id: social-penetration-intimacy
title: 社会渗透与亲密建立
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第5章: 社会渗透理论和人际亲密过程模型
    - 第3章: 临近和熟悉是吸引力的基础（曝光效应）
    - 第7章: 友谊发展中的自我表露规律
    - 第8章: 亲密感是爱情的核心成分之一
V2_predictive_power:
  passed: true
  novel_question: "为什么我和喜欢的人聊了很久还是感觉不亲近？"
  derived_answer: "根据社会渗透理论，亲密感来自自我表露的广度（话题多样性）和深度（个人意义）。如果只聊表面话题（广度够但深度不够），或者只聊一个领域（深度够但广度不够），都不会产生真正的亲密。人际亲密过程模型还指出，光有表露不够，还需要对方的应答性（兴趣、同情、尊重）以及你感知到对方的应答。检查：你有自我表露吗？对方有回应吗？你感知到对方的回应了吗？"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是"聊得多了就熟了"。
    独特贡献在于:
    (1) 亲密不是时间长短问题，而是自我表露的广度和深度问题——
        认识十年可能还不如一次深度交谈亲密；
    (2) 表露需要相互性——匹配彼此的开放程度，
        一次说太多太快是危险的（会让人不舒服）；
    (3) 应答性比表露本身更重要——说再多对方没反应也不会产生亲密。
```

---

## 10. cognitive-bias-defense — 关系认知偏差防御

- merged_from: [f08, f09, f11, p15, p17]
- supporting_cases: [c06汉娜实验, c11自我实现预言]
- supporting_counter_examples: [ce03首因效应偏差, ce04行动者观察者效应, ce14错误归因]
- supporting_glossary: [g05首因效应, g07证实偏差]

```yaml
id: cognitive-bias-defense
title: 关系认知偏差防御
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第4章: 首因效应、证实偏差、归因偏差、自我实现预言
    - 第5章: 人际隔阂——以为伴侣理解自己但实际没有
    - 第10章: 嫉妒中的认知偏差（过度解读、灾难化）
    - 第11章: 冲突中的归因偏差（维持苦恼vs改善关系的归因模式）
V2_predictive_power:
  passed: true
  novel_question: "为什么我总觉得伴侣不够爱我，但朋友都说他对我挺好的？"
  derived_answer: "可能有几种认知偏差在起作用。首因效应设定了最初的期望（如果刚开始他特别热情，后来的正常对待就会显得冷淡）。证实偏差让你更容易注意到支持'他不够爱我'的证据，忽略反面证据。如果你倾向于不安全依恋，对拒绝的高度敏感会放大这些偏差。关键检验：如果朋友看到的和你感受到的不一样，不是朋友'不懂'，而可能是你的认知滤镜在起作用。试着列出具体的'不够爱'的证据和反证据，用数据而非感觉判断。"
V3_exclusivity:
  passed: true
  why_not_common: |
    常识是"当局者迷，旁观者清"。
    独特贡献在于:
    (1) 不是泛泛地说"你可能想多了"，而是给出具体的偏差机制
        （首因效应、证实偏差、归因偏差、自我实现预言）；
    (2) 每种偏差在关系中的具体表现不同——
        首因效应影响第一印象，证实偏差影响后续判断，
        归因偏差影响对行为的解释，自我实现预言影响实际行为；
    (3) 偏差不是因为人笨——而是大脑的认知捷径，
        在关系中因为利害关系大而被放大。
```

---

## 淘汰单元摘要

| id | title | 淘汰项 | 原因 |
|---|---|---|---|
| Rusbult四象限模型 | Rusbult 不满反应四象限 | V3 | "退出/发声/忠诚/忽视"分类是学术分类，不够独特和反直觉，可并入冲突管理工具箱 |
| Gottman冲突风格分类 | Gottman 夫妻冲突风格分类 | V1 | 主要出现在第11章一处，缺少第二个独立语境；作为冲突工具箱的一部分而非独立skill |
| 归属需要是人类基本动机 | 归属需要 | V2, V3 | "人需要关系"是常识，可预测力弱（不能推出具体行动）；作为背景概念而非独立方法论 |

---

## → 进入阶段 2

以下 10 个单元将通过 RIA++ 构造为独立 SKILL.md:

1. interdependence-assessment
2. negativity-bias-ratio
3. relationship-mindset
4. love-triangle-passion-decline
5. self-expansion-boredom
6. conflict-management-toolbox
7. relationship-maintenance
8. attachment-pattern-awareness
9. social-penetration-intimacy
10. cognitive-bias-defense
