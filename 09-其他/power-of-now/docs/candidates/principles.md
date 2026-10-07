# candidates/principles.md — 原则提取器产出

> 提取器: principle-extractor（串行降级执行，"干净视角"独立跑完）
> 出处章节按 fulltext.txt 实际章节标注；引用 ≤150 字。
> 本阶段不做筛选，交给阶段 1.5 三重验证（含与其他提取器的合并去重）。

```yaml
- id: p01
  title: 思维与情绪冲突时，思维是说谎的一方
  type: principle
  source_chapter: 第一章（另见第八章）
  source_quote: |
    "如果两者之间有明显的分歧，那么思维永远是说谎的一方，情绪则始终是真实的。……
    身体总是会给你一个真实的反映，所以请在你体内去看或是感受它。"
  summary: |
    决策与自我评估的仲裁规则：当脑中的叙事（"没事""我应该高兴""都是他的错"）
    与身体里的感受不一致时，以身体/情绪为准，用它反查思维在掩饰什么。
    观察情绪即可，不必分析。
  tags: [principle, emotion, decision]

- id: p02
  title: 练习成功的唯一度量是内在平和程度
  type: principle
  source_chapter: 第一章
  source_quote: |
    "有一个标准可以用来衡量你的练习是否成功：你内在所感觉到的平和的程度。"
  summary: |
    不以"坐了多久""顿悟了没有"衡量练习，只以平和程度为度量；且强调这种平和
    不以意识清晰度为代价——更警惕、更清醒、更临在才算数。
  tags: [principle, metric]

- id: p03
  title: 观察时绝不评判
  type: principle
  source_chapter: 第一章（另见第三、四章）
  source_quote: |
    "当你在倾听那种声音时，不要去做任何评判。不要对你所听到的声音做出判断或进行
    谴责，因为这样做意味着同样的声音又会从后门乘虚而入。"
  summary: |
    观察思维/情绪的硬规则：不判断、不分析、不贴标签，只观察。
    评判即认同的复活——"请将你的注意力集中于内在……请不要进行分析，观察就可以了"。
  tags: [principle, awareness, rule]

- id: p04
  title: 永远对当下说"是"
  type: principle
  source_chapter: 第二章
  source_quote: |
    "永远对当下说'是'。有什么比对已然存在的东西进行内在的抗拒更徒劳、更疯狂的
    吗？……向'是'臣服，对生活说'是的'，看看生活是如何为你服务而不是与你为敌的。"
  summary: |
    对已发生之事的默认态度：接受。反对当下=反对生命本身，徒劳且制造痛苦。
    是"接纳然后行动"的口号版。
  tags: [principle, acceptance]

- id: p05
  title: 接纳，然后行动
  type: principle
  source_chapter: 第二章（另见第九、十章）
  source_quote: |
    "接纳，然后采取行动。不管当下时刻的情况怎样，心甘情愿地接受它，就像它是你选择的
    一样。总是与它共事，而不是抗拒它，使它成为你的朋友和盟友而不是敌人。"
  summary: |
    顺序规则：先接纳现状（像它是你选择的一样），再采取必要行动。接纳不是终点而是
    行动的地基——"做你必须做的事情，同时，接受它的存在"；泥沼情境同理：
    接受当下现实，然后尽全力脱身。
  tags: [principle, acceptance, action]

- id: p06
  title: 不要再创造时间
  type: principle
  source_chapter: 第二章（另见第三章）
  source_quote: |
    "请你不要再创造时间，或者至少不要创造除了做必要事情之外的时间。……把你的生活
    重心完全放到当下这一刻，只在必要时简单地回顾过去和展望未来。"
  summary: |
    时间预算规则：把生活重心从过去与未来移到当下；回顾与展望只在"必要事务"范围内
    使用，用完即归位。是钟表时间/心理时间判别的总纲。
  tags: [principle, time]

- id: p07
  title: 不向痛苦之身宣战，观察就足够
  type: principle
  source_chapter: 第二章
  source_quote: |
    "就像你不能向黑暗宣战一样，你不能向痛苦之身宣战，这样做只会引发内心的冲突并
    创造更深的痛苦。所以观察它就足够了。观察它意味着接纳它成为当下时刻事实的一部分。"
  summary: |
    与负面情绪斗争=给它供能；唯一有效动作是把意识之光带进去（观察、允许、感受）。
    与黑暗抗争的隐喻贯穿全书（无意识同理）。
  tags: [principle, emotion, non-resistance]

- id: p08
  title: 不要从痛苦中汲取身份认同
  type: principle
  source_chapter: 第二章（另见第八章）
  source_quote: |
    "第一件需要记住的事是：只要你从痛苦中汲取你的身份认同，你就无法从痛苦中
    解放出来。……受害者身份是这样一个信念：过去比现在更强大，这当然是一个伪真理。"
  summary: |
    康复的头号绊脚石：把痛苦编进"我是谁"（受害者、病人、被辜负者）。只要自我感
    部分来自情绪痛苦，人就会无意识破坏治愈自己的努力；解决方案是保持觉知。
  tags: [principle, identity, healing]

- id: p09
  title: 焦虑属于未来，愧疚属于过去
  type: principle
  source_chapter: 第三章
  source_quote: |
    "焦虑、紧张、不安、压力、烦恼——所有形式的恐惧，都是因为对未来过于关注而对当下
    关注不够所引起的。愧疚、后悔、悲伤、怨恨……都是由过于关注过去而很少关注当下
    时刻引起的。"
  summary: |
    时间-情绪对照诊断表：把消极心态按时间轴定位（未来向/过去向），从而对症选工具
    （未来向→回到当下的问题清零；过去向→停止反刍、汲取教训后归档）。
  tags: [principle, diagnostic, emotion]

- id: p10
  title: 未来是过去的复制品
  type: principle
  source_chapter: 第三章
  source_quote: |
    "一般来说，未来是过去的复制品。表面的变化是有可能发生的，但是真正的变化却很少
    发生，这主要依赖于你是否能充分地保持临在，并通过汲取当下的力量来解决过去的
    事情。"
  summary: |
    对"明天会更好"的釜底抽薪：若当下的意识质量不变，未来只是旧模式的重演
    （中奖千万者照样重复制约模式）。真变化唯一的发生地是当下。
  tags: [principle, change, time]

- id: p11
  title: 改变做事的方式，而不是做什么
  type: principle
  source_chapter: 第三章
  source_quote: |
    "如果你正在做的事情无法让你感受到喜悦、自在和轻松，这并不意味着你需要改变你正在
    做的事情，你需要改变的是你做事的方式。如何做事通常比做什么事更为重要。"
  summary: |
    行动质量规则：烦躁时先别辞职/离婚/搬家，先改变"如何做"——把注意力从结果移回
    行动本身，完全接受当下事实后再看是否真需改变事情。
  tags: [principle, action, work]

- id: p12
  title: 不执着于行动结果
  type: principle
  source_chapter: 第三章（另见第九、十章）
  source_quote: |
    "请不要担心你行动的结果——仅仅关注行动本身就好了。行动的结果会自然而然地产生。
    ……《薄伽梵歌》，将对行动结果的不执着称为业力瑜伽。"
  summary: |
    行动规则：全力做事，不把自我感押在结果上；"失败或成功都不会改变你本体的内在
    状态"；"尊重每一件事，却又不在乎这一切"。
  tags: [principle, action, non-attachment]

- id: p13
  title: 情境要么应付要么接受，不要转变成问题
  type: principle
  source_chapter: 第三章（另见第四、九章）
  source_quote: |
    "一个情境出现时，我们要么是去应付它，要么就是去接受它，对它说'好的'。为什么要
    把它转变成问题呢？……思维会无意识地喜欢上问题，因为它们给你某种身份的认同。"
  summary: |
    二分规则：真实情境只允许两种处理（现在行动/接纳），禁止第三种——心理上反复琢磨
    并把它变成自我感的一部分（"钟情的戏剧性事件"）。
  tags: [principle, problem, reframing]

- id: p14
  title: 首要的是内在，其次才是外在
  type: principle
  source_chapter: 第四章
  source_quote: |
    "请像你对外界发生的事情一样地对你内心发生的事情保持兴趣。如果你内在没问题，外界
    才会正常顺利。首要的是内在，其次才是外在。"
  summary: |
    注意力分配规则：对内心状态的关注不低于对外部事件；内在秩序是外在秩序的前提。
  tags: [principle, attention]

- id: p15
  title: 先放下消极情绪，再采取行动
  type: principle
  source_chapter: 第四章
  source_quote: |
    "如果你采取任何行动——离开或者改变你的情况，首先请放下消极的情绪，如果可能的
    话，请完全地放下。由深刻观察而采取的行动比由消极心态引发的行动更为有效。"
  summary: |
    行动前置条件：任何"离开/改变"类行动前先清空消极能量，否则行动被污染、
    创造更多不幸。配套：承认恐惧、观察它、与它共存，切断恐惧与思维的联系。
  tags: [principle, action, emotion]

- id: p16
  title: 行动总比不行动好
  type: principle
  source_chapter: 第四章
  source_quote: |
    "行动总比不行动好，尤其是当你陷入不幸之中很久时。如果你所采取的行动是错误的，
    至少你会从中学到教训，在这种情况下，它就不再是个错误了。"
  summary: |
    反拖延规则：长期困在不幸中时，错误行动也比原地不动好——错误可转化为教训，
    停滞则一无所获。
  tags: [principle, action]

- id: p17
  title: 接纳之后，必须迈向"不再创造"
  type: principle
  source_chapter: 第四章
  source_quote: |
    "当你练习接纳一段时间之后，你需要再继续向下一个阶段迈进，那个不再创造这些消极
    情绪的阶段。如果你不再继续向前迈进，你的这种接纳就成了一个精神上的标记，它使你的
    小我不断地沉浸在不幸之中。"
  summary: |
    警惕"假接纳"：允许情绪存在只是第一阶段；若停留于此，接纳会变成小我的灵性徽章、
    继续浸泡在不幸里。第二阶段是识别并拆掉产生消极情绪的机制。
    "真正的接纳会立即转化这些情感。"
  tags: [principle, acceptance, trap]

- id: p18
  title: 压力=你在这里，却想去那里
  type: principle
  source_chapter: 第四章
  source_quote: |
    "压力的产生是由于你在'这里'却想到'那里'去，或你在当下却想去未来。……如果必要的
    话，你可以动作快些，工作得快些，甚至用跑的，但是不需要抗拒当下并且把自己投射到
    未来去。"
  summary: |
    压力的重新定义与反直觉处方：忙碌本身不产生压力，内在分裂才产生；允许快，
    禁止"人在此心在未来"。赶路时全力赶路并享受能量流动。
  tags: [principle, stress, work]

- id: p19
  title: 不要试图理解过去
  type: principle
  source_chapter: 第四章
  source_quote: |
    "我们没有必要去研究这些无意识的过去……如果你试图探究过去，它将会变成一个无底洞，
    永远探究不完。……更多的时间不会把你从时间中解放出来。"
  summary: |
    反回溯规则：所需的过去功课会由当下的挑战自动浮出水面；在当下观察行为/反应/情绪
    （不批判不分析）就是"以当下的力量处理过去"。理解过去可以有用但不是关键。
  tags: [principle, past, healing]

- id: p20
  title: 挑战来临时，立即回体内几秒
  type: principle
  source_chapter: 第六章（另见第四、八章）
  source_quote: |
    "当你遇到这些挑战时……你要养成习惯，将注意力集中在你身体的内在能量场上。不需要
    花费太长的时间，几秒钟就够了。但是当挑战来临的那一刻，你就必须立即采取行动。
    任何延误都会让心理——情绪条件反射出现，并将你控制。"
  summary: |
    微规则：被批评/冲突/坏消息的第一反应不是回应，而是把注意力放进身体几秒钟；
    时间窗极短，延误即被条件反射接管；之后从更深层次反应。
  tags: [principle, trigger, body]

- id: p21
  title: 转化通过身体发生，而不是远离身体
  type: principle
  source_chapter: 第六章
  source_quote: |
    "事实上，没有人曾经通过拒绝身体、折磨身体或是身体经验来达到开悟。……转化的实质
    性工作是在身体上发生的。转化是通过身体而不是远离身体来完成的。……请不要对抗你的
    身体，因为这样做就是在对抗你的本质。"
  summary: |
    灵修路线规则：禁止苦修、禁欲、压抑感官式的身体否定（作者以佛陀六年苦修后放弃
    方开悟为证）；身体是入口不是敌人。
  tags: [principle, body, boundary]

- id: p22
  title: 进入内在身体之前，先宽恕
  type: principle
  source_chapter: 第六章
  source_quote: |
    "请将注意力放在你情绪的感受上，并检查你的思维是否停留在一个怨恨的模式上，比如
    责备、自怜或者仇恨。这些会喂养你的负面情绪。……宽恕就是放下怨恨，同时放下悲痛。"
  summary: |
    冥想/内观的前置检查：若注意力转向内在时出现焦虑恶心等不适，先观察这些被压抑的
    情绪与背后的怨恨模式（可能指向他人/自己/情境/甚至未来），倾注全部注意力即接纳，
    然后才能深入。
  tags: [principle, forgiveness, meditation]

- id: p23
  title: 完全接受你的伴侣，是最伟大的催化剂
  type: principle
  source_chapter: 第八章
  source_quote: |
    "爱情最伟大的催化剂就是完全接受你伴侣的一切，而不是去批判或以任何方式改变他或
    她。……再也没有受害者和加害者，也没有原告和被告。"
  summary: |
    关系规则：停止批判（先对自己，再对伴侣）；放弃改造对方的工程——改造需求本身就是
    小我与上瘾结构。接受之后"要么分开，要么一起更深入地进入当下"。
  tags: [principle, relationship, acceptance]

- id: p24
  title: 爱情关系不是让你幸福，而是让你更有意识
  type: principle
  source_chapter: 第八章
  source_quote: |
    "爱情关系不是用来使你快乐或满足的，如果你仍想通过爱情关系来获得拯救的话，那你将
    会一次又一次地遭受挫折。但是如果你能承认爱情关系不是为了让你更幸福，而是让你更有
    意识……"
  summary: |
    关系目的论反转：把"关系该满足我"改为"关系暴露我的无意识"——每一次不和谐都是
    拯救机会（无意识被带入光中）；对伴侣的无意识行为"请为此觉得欣慰"。
  tags: [principle, relationship, reframing]

- id: p25
  title: 对当下的宽恕优先于对过去的宽恕
  type: principle
  source_chapter: 第九章（另见第六、十章）
  source_quote: |
    "对当下的宽恕甚至比对过去的宽恕更为重要。如果你宽恕每一刻，允许它的存在——你就
    不会去积累需要在未来宽恕的怨恨了。"
  summary: |
    宽恕的时间轴前移：不等伤害累积后算总账，而是事中即时允许——宽恕每一刻，
    就清空了"未来需要宽恕的库存"。宽恕=放下怨恨与悲痛，"不去抗拒生命"。
  tags: [principle, forgiveness]

- id: p26
  title: 高质量的"不"：臣服不是不行动
  type: principle
  source_chapter: 第十章
  source_quote: |
    "臣服不是说你允许那些无意识的人利用你。绝对不是。你完全可以坚定地对那个人说
    '不'……让它成为一个非反应的'不'，高质量的'不'，一个不带任何消极情绪的'不'。"
  summary: |
    反误读规则：臣服/不抗拒≠任人摆布、≠"我不在乎"（那是戴面具的抗拒）；可以对人与
    情境坚定说不或离开，只要这个"不"出自清晰洞见而非反应，不带消极情绪；
    不抗拒≠不行动（无为=内心不抗拒+高度警惕）。
  tags: [principle, boundary, surrender]
```
