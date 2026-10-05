# candidates/cases.md — 案例提取器产出

> 提取器: case-extractor（串行降级执行，"干净视角"独立跑完：只找作者亲自使用/转述的实例）
> 全书上下文: 见 BOOK_OVERVIEW.md；出处按 fulltext.txt 实际章节与行号标注。
> 本阶段不做筛选，宁错杀，交给阶段 1.5 三重验证。案例必须绑定方法论主题（bound_to）。引用 ≤150 字。

```yaml
- id: c01
  title: 滴滴出行的四阶段套演
  type: case
  source_chapter: 中文版序言（余晨，L99–109）※非作者正文，仅作素材
  source_quote: |
    "打不到车就成了大家使用打车软件的触发。……到后期成为随机金额补贴，保证了多变酬赏
    的激励作用……累积滴滴的积分……让用户产生了路径依赖，想到出行第一件事就是打开滴滴。"
  summary: |
    中文版序言用滴滴把四阶段走了一遍：痛点（打不到车）=触发；地图定位下单=行动易发生；
    红包补贴+朋友圈分享=多变酬赏；积分、固定路线、成为司机=投入→路径依赖。
  bound_to:
    - "上瘾模型四阶段总框架"
  outcome: 4 年从无名到独角兽；亿级用户成为估值保证（序言自述）。
  tags: [case, hook-model, china]
```

```yaml
- id: c02
  title: 芭芭拉与 Pinterest（贯穿全书的虚拟案例）
  type: case
  source_chapter: 前言（L186–216）
  source_quote: |
    "她在 Pinterest 上逗留的时间会越来越长，期待发现更多的惊喜。不知不觉间，她已经滑屏
    了45分钟。……这份投入反过来又会强化她与网站之间的联系。"
  summary: |
    作者在前言用一位虚构用户完整演示四阶段：Facebook 图片（外部触发）→点击进入 Pinterest
    （行动）→视觉惊喜、滑屏 45 分钟（多变的酬赏）→收藏与关注（投入→加载下一次触发）。
    冰箱门对比：可预见结果（开灯）不产生渴望，多变结果才点燃渴望。
  bound_to:
    - "上瘾模型四阶段总框架"
    - "多变的酬赏机制"
  tags: [case, hook-model, demo]
```

```yaml
- id: c03
  title: 英与 Instagram：从朋友推荐到条件反射
  type: case
  source_chapter: 第2章（L539–545、L726–744）
  source_quote: |
    "'我没想用它来解决什么问题，只是看见好玩儿的东西就想拍下来。'……正是因为人们担心
    某个宝贵时刻会一去不复返，所以才会感觉到压力如山。"
  summary: |
    斯坦福学生英自称"没想解决什么问题"，但作者拆出完整触发链：朋友照片（人际型）→
    媒体/商店推荐（回馈型）→应用图标（自主型）→内部触发"怕美好时刻一去不复返"（FOMO）。
    用于说明外部触发四类的接力与内部触发的情绪锚定。
  bound_to:
    - "外部触发四分类"
    - "内部触发锚定"
  outcome: Instagram 用户 1.5 亿，10 亿美元被 Facebook 收购。
  tags: [case, trigger, instagram]
```

```yaml
- id: c04
  title: PayPal 的病毒式增长
  type: case
  source_chapter: 第2章（L614–618）
  source_quote: |
    "有人把钱打入你的账户，这会使你迫不及待地想要登录账户进行查询。而且，PayPal 还兼具
    实际用途，所以才会在用户中间迅速地传播。"
  summary: |
    人际型触发的正面典型：收款行为本身制造打开产品的动机，实际价值驱动自发传播。
    作者同时给出反面警示：用"黑暗模式"恶意引诱用户邀请朋友的公司会失去信任。
  bound_to:
    - "人际型触发"
    - "黑暗模式的伦理边界"
  tags: [case, viral, trigger]
```

```yaml
- id: c05
  title: 朱丽与电子邮件：5 问法示例
  type: case
  source_chapter: 第2章（L700–722）
  source_quote: |
    "5.她为什么会在意这一点？答案：因为她害怕被圈子所抛弃。现在我们有答案了！恐惧感
    是她身上最强大的内部触发。"
  summary: |
    作者虚构的推演案例（新产品"电子邮件"上线前的研究）：对中层经理朱丽连问五个为什么，
    从"收发信息"挖到"害怕被圈子抛弃"。用于示范 5 问法的完整链条与终点判据（出现情绪词）。
  bound_to:
    - "5 问法"
    - "内部触发锚定"
  tags: [case, user-research, five-whys]
```

```yaml
- id: c06
  title: 作者晨跑改黄昏跑后的"早上好"
  type: case
  source_chapter: 第1章（L279–299）
  source_quote: |
    "直到剃须刀的刀锋划过脸颊，我才意识到自己已经抹好剃须膏准备刮胡子了。虽然这是我
    每天必做的功课，但无论如何也不该在大晚上刮胡子。"
  summary: |
    作者亲历：临时把晨跑改到黄昏，身体仍按晨跑模式执行——对人打招呼说"早上好"、
    晚上刮胡子，全然未觉。作者用它定义习惯的本质（无意识执行的行为脚本）与第一章
    的起点。
  bound_to:
    - "习惯的无意识性"
  tags: [case, habit, personal]
```

```yaml
- id: c07
  title: QWERTY 键盘 vs 德沃夏克键盘
  type: case
  source_chapter: 第1章（L374–378）
  source_quote: |
    "虽然这款'德沃夏克简约型键盘'在1932年就申请到了专利，但如今市场上早已看不到它的
    踪影。……转而使用一款完全陌生的键盘，哪怕它能提高工作效率，也意味着我们将不得不
    重新学习打字。"
  summary: |
    习惯锁定效应的经典例证：效率更高的德沃夏克键盘 1932 年获专利后被 QWERTY 彻底埋葬，
    因为切换等于重新学习打字。支撑"新产品须有绝对优势"与"旧习惯是最大壁垒"两个论点。
  bound_to:
    - "撼动旧习惯需要绝对优势"
    - "储存价值/切换成本"
  tags: [case, lock-in, competition]
```

```yaml
- id: c08
  title: Google vs Bing：毫秒差异无关胜负
  type: case
  source_chapter: 第1章（L403–407）
  source_quote: |
    "在对这两个都提供匿名搜索服务的平台进行效能比较时，我们会发现它们没什么两样。……
    适应 Bing 的操作界面实际上降低了这些 Google 用户的搜索效率，会让他们觉得 Bing
    稍逊一筹，这种感觉与技术无关。"
  summary: |
    搜索效能几乎相同的两个产品，用户死守 Google：熟悉界面的任何像素差异都构成认知负担，
    "感觉 Bing 更差"与技术无关；且 Google 记录搜索轨迹做个性化，越用越准。说明习惯
    （而非性能）决定选择，以及个性化如何加固循环。
  bound_to:
    - "旧习惯的认知负担"
    - "数据投入加固循环"
  tags: [case, habit, competition]
```

```yaml
- id: c09
  title: 亚马逊"一站式购物中心"与 Progressive 保险
  type: case
  source_chapter: 第1章（L416–422）
  source_quote: |
    "通过给各大竞争对手做宣传，亚马逊网站不仅赚足了广告费，还借助别人的营销投入为自己
    在用户心目中赢得了一席之地。"
  summary: |
    低频行为养成习惯的另类路径：亚马逊为竞争对手产品做广告，消除用户价格顾虑，成为
    购物比价的"首选心智"；用户甚至进实体店用其 App 扫价。Progressive 汽车保险用同样
    比价策略把年营业额从 34 亿美元做到 150 亿美元。证明低频产品靠"可感知用途"也能
    进入习惯区间。
  bound_to:
    - "习惯区间（低频高用途象限）"
    - "基于习惯的发展战略"
  outcome: Progressive 年营业额 34 亿→150 亿美元。
  tags: [case, habit-zone, strategy]
```

```yaml
- id: c10
  title: Evernote 微笑曲线
  type: case
  source_chapter: 第1章（L342–346）
  source_quote: |
    "在免费使用产品的头一个月过去后，仅有 0.5% 的用户转变为付费用户。然而，这个比例会
    渐渐上升。到了第 33 个月，已经有 11% 的用户开始付费。在第 42 个月，这个比例显著
    增长到了 26%。"
  summary: |
    CEO 利宾公布的使用曲线：初期使用量下滑，形成依赖后大幅攀升，呈"笑脸"形；付费
    转化率随使用时间从 0.5% 升至 26%。用于论证依赖性提升用户终身价值与付费意愿——
    习惯本身就是商业模式。
  bound_to:
    - "用户终身价值"
    - "习惯与商业收益"
  tags: [case, monetization, data]
```

```yaml
- id: c11
  title: 巴菲特提价论与免费游戏行规
  type: case
  source_chapter: 第1章（L336–340）
  source_quote: |
    "要衡量一个企业是否强大，就要看看它在提价问题上经历过多少痛苦。……免费视频游戏
    行业的行规是，游戏开发商延迟向玩家收取费用，直到玩家玩上瘾。"
  summary: |
    价格灵活性的两个例证：巴菲特/芒格因"习惯降低价格敏感度"投资 See's Candies 与
    可口可乐；免费游戏延迟收费、先让玩家上瘾再卖虚拟道具。Candy Crush Saga 5 亿下载、
    日均净利 100 万美元。论证"依赖性=定价权"。
  bound_to:
    - "价格灵活性"
    - "多变的酬赏（付费前先钩住）"
  tags: [case, pricing, freemium]
```

```yaml
- id: c12
  title: Facebook 后来居上与病毒循环周期
  type: case
  source_chapter: 第1章（L355–359）
  source_quote: |
    "20天内，若以两天为一循环周期，用户量可能会达到20470；但是如果将这个周期减半，变成
    一天一循环，那用户数量将超过2000万！"
  summary: |
    Facebook 晚于 MySpace/Friendster 进入社交网络，却凭"使用频率越高、病毒式增长越快"
    的良性循环胜出。斯科克的算术：邀请周期从 2 天缩到 1 天，20 天用户量差三个数量级。
    论证高频使用压缩病毒循环周期、加速增长。
  bound_to:
    - "病毒循环周期"
    - "习惯加快增长"
  tags: [case, growth, viral]
```

```yaml
- id: c13
  title: Mint 的单一行动召唤邮件
  type: case
  source_chapter: 第2章（L577–585）
  source_quote: |
    "该网站原本可以在邮件上多添加一些触发，比如提醒你查询银行账户、浏览信用卡消费清单，
    或是办理金融业务。但是它没有。"
  source_quote_note: 原文为图3说明与正文转述，引文为编译
  summary: |
    外部触发设计范本：账户警告邮件把所有可能任务整合为一个橙色大按钮"登录 Mint"。
    用于说明"选择项越多权衡越久，单一明确指令更易形成无意识行为"。
  bound_to:
    - "一次只给一个明确的下一步指令"
  tags: [case, cta, email]
```

```yaml
- id: c14
  title: 内容发布简化史：博客→Twitter→Pinterest/Instagram
  type: case
  source_chapter: 第3章（L892–902）
  source_quote: |
    "评论家并不看好 Twitter 每条推文不得超过 140 个字符的规定……他们恰恰忽略了一点，
    这样的限制实际上使更多的人具备了在网络上书写的能力。"
  summary: |
    网络内容供给的每次爆发都源于发布门槛的骤降：注册域名装 CMS→博客平台一键注册→
    140 字符微博→随手拍摄分享。威廉姆斯注解："选取人性中的某种欲望……利用现代科技来
    逐步满足这种欲望。"支撑"简化驱动行为频率"与"能力六要素"的宏观证据。
  bound_to:
    - "简化三步法"
    - "能力六要素"
  tags: [case, simplification, history]
```

```yaml
- id: c15
  title: Twitter 主页三次演变
  type: case
  source_chapter: 第3章（L1015–1040）
  source_quote: |
    "2009 年的 Twitter 主页以激发用户动机为目标。然而到了 2012 年，Twitter 的战略重心
    转向了推动用户行为。"
  summary: |
    主页从 2009 年杂乱文本（解释价值主张）→"分享和发现正在发生的一切"→简洁界面+
    140 字符自我介绍+"登录/注册"两个行为召唤→移动端下载引导。作者用它论证"先解决
    能力问题"与"与其推销不如让用户真刀真枪试一次"。
  bound_to:
    - "先解决能力问题，而非动机"
    - "行动阶段减摩擦"
  tags: [case, design-evolution, twitter]
```

```yaml
- id: c16
  title: 简化设计四例（注册器/分享按钮/锁屏相机/无限滚动）
  type: case
  source_chapter: 第3章（L934–998）
  source_quote: |
    "苹果公司意识到……有必要简化拍照步骤。因此，它将相机程序设置为在锁定屏幕上可直接
    打开，无须输入解锁密码。"
  summary: |
    能力六要素的应用案例组：Facebook 注册器删去注册中间步骤（同时附异议：隐私敏感者
    反而焦虑）；Twitter 嵌入式分享按钮把转链接缩为一步（25% 推文含链接）；iPhone 锁屏
    直开相机抢时间要素；Pinterest 无限滚动取消翻页等待。Google 干净主页（L962–970）
    省时间与脑力。共同点：找最短板做减法。
  bound_to:
    - "能力六要素与补最短板"
  tags: [case, simplification, ux]
```

```yaml
- id: c17
  title: 饼干罐稀缺实验与亚马逊"仅剩 14 台"
  type: case
  source_chapter: 第3章（L1062–1076）
  source_quote: |
    "虽然饼干没有差别，玻璃罐也一模一样，但被试者显然更珍惜几乎空着的那一罐里的饼干。
    ……面对突然增多的饼干，人们做出的价值判断比一开始就被分到十块饼干时的价值判断
    还要低。"
  summary: |
    稀缺效应实验：两罐相同饼干，2 块装被估值更高；突然增多的饼干估值反而更低。作者
    联系亚马逊"仅剩 14 台/最后三本"的库存显示，说明稀缺信号被产品化。也提示该手法
    的操纵边界（与 p09、p14 对读）。
  bound_to:
    - "稀缺效应"
    - "启发法的产品化应用"
  tags: [case, scarcity, experiment]
```

```yaml
- id: c18
  title: 地铁站里的小提琴家与 90 美元的啤酒
  type: case
  source_chapter: 第3章（L1083–1089）
  source_quote: |
    "当演出地点改在了地铁站，他的音乐不啻对牛弹琴。……啤酒的价格越高，他们喝得越开心。
    ……几乎没有一个被试者发现，他们自始至终喝到的，都是同一种啤酒。"
  summary: |
    环境效应两个实验：世界级小提琴家约书亚·贝尔在地铁站免费演奏无人驻足（票价上千的
    音乐厅座无虚席）；fMRI 下被试者喝标价 90 美元的同一款啤酒报告更愉悦、愉悦脑区波动
    更强。说明价值判断随情境与预期漂移，产品语境本身是变量。
  bound_to:
    - "环境效应"
    - "启发法的产品化应用"
  tags: [case, context-effect, experiment]
```

```yaml
- id: c19
  title: 洗车卡实验与 LinkedIn 资料进度条
  type: case
  source_chapter: 第3章（L1105–1109）
  source_quote: |
    "第二组顾客——卡上已经免费打过两次孔的顾客，完成这八次消费的人数比第一组高出了
    82%。这一研究证明了目标渐近效应的存在。"
  summary: |
    目标渐近/赠券效应：同样需消费 8 次，"10 次卡已打 2 孔"组的完成率高 82%。LinkedIn
    用个人资料完成条（而非数字比例）让用户直观看见自己接近目标。产品化用法：预填进度、
    可视化接近感。是投入阶段"小步开始"的心理学基础之一。
  bound_to:
    - "目标渐近效应"
    - "投入分解成小块任务"
  tags: [case, goal-gradient, experiment]
```

```yaml
- id: c20
  title: Stack Overflow 的威望值与勋章
  type: case
  source_chapter: 第4章（L1261–1271）
  source_quote: |
    "为什么会有众多用户不惜将宝贵时间投入这样一份没有酬劳的工作中呢？……当威望值达到
    一定标准时，这些作者就能获得代表特殊地位和特许权利的勋章。"
  summary: |
    社交酬赏范本：用户每天无偿写 5000 条高技术含量回复，动力是投票累积的威望值与勋章
    （不可预测的认可）。说明社交认同足以支撑重劳动，且"不确定因素将寻常任务变成诱人
    的游戏"。
  bound_to:
    - "社交酬赏"
    - "社交认同大于经济激励"
  tags: [case, social-reward, community]
```

```yaml
- id: c21
  title: 英雄联盟的荣誉值机制
  type: case
  source_chapter: 第4章（L1273–1281）
  source_quote: |
    "玩家可以给他们认为光明正大的游戏行为奖励荣誉值。……玩家可以根据荣誉值判断出哪些
    人是'捣蛋鬼'，从而与其他玩家一起联手把这些害群之马踢出局。"
  summary: |
    用社交酬赏治理社区：面对匿名捣蛋鬼败坏游戏名声，开发商依班杜拉社会学习理论设计
    玩家互授的"荣誉值"，让合作行为获得不确定的集体认可，社区自净。示范酬赏机制可以
    是行为治理工具而不只是增长工具。
  bound_to:
    - "社交酬赏"
    - "社会学习理论"
  tags: [case, social-reward, governance]
```

```yaml
- id: c22
  title: 桑人耐力捕猎与信息流狩猎
  type: case
  source_chapter: 第4章（L1290–1330）
  source_quote: |
    "在捕猎的过程中，猎手是为了追逐而追逐。这种心理机制有助于解释现代人需索无度的状态。
    ……为了满足这份好奇，大家会继续滑动翻页，一睹神秘图片的全貌。"
  summary: |
    猎物酬赏的机制拼图：桑人猎手 8 小时追垮 500 磅羚羊——为追逐而追逐；老虎机日吞 10
    亿美元；Twitter 时间序信息流让人不停滑动"找相关推文"；Pinterest 把图片截成两半
    当诱饵。共同机制：把资源获取变成不确定的追逐过程。
  bound_to:
    - "猎物酬赏"
  tags: [case, prey-reward, mechanism]
```

```yaml
- id: c23
  title: 自我酬赏三例：魔兽世界/Mailbox/Codecademy
  type: case
  source_chapter: 第4章（L1343–1373）
  source_quote: |
    "人们只有体验到终结感，才会觉得愉悦和满足。……Codecademy 针对不同学习阶段提供的
    这种即时反馈正是对自我的一种酬赏。"
  summary: |
    自我酬赏的三个形态：魔兽世界升级/攻地（成就感与掌控感）；Mailbox 追求"未读邮件为零"
    （终结感，Dropbox 1 亿美元收购）；Codecademy 交互式即时纠错把学编程的苦役变挑战
    （胜任感+不确定的关卡）。支撑"自我酬赏=操控感/成就感/终结感"的分类。
  bound_to:
    - "自我酬赏"
  tags: [case, ego-reward, learning]
```

```yaml
- id: c24
  title: Mahalo vs Quora：奖金打不过投票
  type: case
  source_chapter: 第4章（L1386–1398）
  source_quote: |
    "Quora 没有给提交答案者奖励过一分钱。……人们对于社交酬赏以及同伴认同的渴望要远远
    大于对经济利益的期待。"
  summary: |
    同赛道的对照实验：Mahalo 用虚拟货币悬赏提问，月访问冲到 1410 万后迅速冷却；Quora
    零奖金，靠投票建立稳定社交反馈，反超并长存。结论：误判核心动机（以为钱是杠杆）
    是激励设计的头号错误；社交认同才是内容社区的硬通货。
  bound_to:
    - "社交认同大于经济激励"
    - "酬赏必须与动机吻合"
  outcome: Mahalo 冷却衰落，Quora 成为问答社区主导者。
  tags: [case, incentive, counter-evidence]
```

```yaml
- id: c25
  title: MyFitnessPal vs Fitocracy：作者亲历的逆反
  type: case
  source_chapter: 第4章（L1435–1455）
  source_quote: |
    "这种在手机上对自己饮食违纪行为供认不讳的做法就变成了强加于我的负担。……在这样
    的事实面前，我要么臣服，要么放弃，最终我选择了放弃。"
  summary: |
    作者亲历对照：MyFitnessPal 要求逐餐记录卡路里，漏记一天即前功尽弃感，作者因逆反
    心理弃用；Fitocracy 用社区评论、"奖品"与问答互动让记录变成社交参与，作者主动回访。
    论证保障自主权、让用户在既有行为与改良模式间选择的规则。
  bound_to:
    - "保障用户自主权（逆反心理）"
    - "让用户在既有方式与更便捷方式间选择"
  tags: [case, reactance, personal, health-app]
```

```yaml
- id: c26
  title: 折纸实验与"小心驾驶"立牌实验
  type: case
  source_chapter: 第5章（L1579–1604）
  source_quote: |
    "自己动手折纸的人对自己作品的价值评估是第二组价值评估的5倍。……在同意贴小标识之后，
    房主们更容易接受在自家草坪上立一块有碍观瞻的大标识牌。"
  summary: |
    投入改变态度的两个实验：阿雷利折纸实验（自折纸鹤估值 5 倍，宜家效应）；立牌实验
    （先请贴 3 英寸小标识，两周后 76% 同意立大牌子；直接请求仅 17%）。共同说明点滴
    投入改变估值与后续行为，是投入阶段设计的实验基础。
  bound_to:
    - "投入改变态度的三心理机制"
    - "投入要分解成小块任务"
  tags: [case, investment, experiment]
```

```yaml
- id: c27
  title: 储存价值五例：iTunes/LinkedIn/Mint/Twitter vs App.net/eBay/Photoshop
  type: case
  source_chapter: 第5章（L1672–1736）
  source_quote: |
    "科技行业许多观察家认为该产品实际上比 Twitter 更好。但是，与其他企图复制服务的尝试
    一样，App.net 并没获得成功。"
  summary: |
    五类储存价值各配实例：iTunes 曲库（内容）；LinkedIn"哪怕一点点信息"与 Mint 账户
    聚合（数据资料）；Twitter 关注网络 vs App.net（关注者——"创建公司所需的技术一天
    之内就能建成"，但关注网络无法复制）；eBay/Yelp/Airbnb 评分（信誉）；Photoshop
    熟练度（技能，无法迁移到竞品）。
  bound_to:
    - "储存价值五形式"
    - "点滴信息投入也有强黏性"
  tags: [case, stored-value, moat]
```

```yaml
- id: c28
  title: Any.do 的会后通知
  type: case
  source_chapter: 第5章（L1753–1763）
  source_quote: |
    "在 Any.do 搭建的情景中，在用户最有可能体验到内部触发——担心会议结束后会忘记执行
    某一后续任务而引发的焦虑感——的时候，应用程序会给用户发送一个外部触发。"
  summary: |
    加载下一个触发的教科书例：新用户被引导连接日历（投入），应用在会议结束时推送
    "记录后续任务"——外部触发恰好落在内部触发（怕忘事的焦虑）最活跃的时刻。示范
    "用户投入生成未来触发+时机对准情绪"的双重要求。
  bound_to:
    - "加载下一个触发"
    - "提出要求时对接内部触发"
  tags: [case, trigger, timing]
```

```yaml
- id: c29
  title: Tinder 与 Snapchat：每次使用都埋下回访
  type: case
  source_chapter: 第5章（L1765–1779）
  source_quote: |
    "Snapchat 的自动销毁功能可以鼓励用户及时回应，用户每发送一条照片信息就会加载下一个
    触发，这种方式将用户牢牢地吸引进来。"
  summary: |
    投入-召回闭环两例：Tinder 每次滑动累积匹配概率，匹配即推送通知（350 万对/天）；
    Snapchat 每条阅后即焚消息隐含"要求回应"，双击即回（日均 40 张/人）。说明高频产品
    可让"投入→触发"压缩到单次会话内完成。
  bound_to:
    - "加载下一个触发"
  tags: [case, loop, mobile]
```

```yaml
- id: c30
  title: 《圣经》应用程序（YouVersion）全案
  type: case
  source_chapter: 第7章（L2000–2121）
  source_quote: |
    "我们害怕用户会卸载程序，可事实正好相反，人们将手机上的那条消息拍下来，开始在
    Instagram、Twitter 和 Facebook 上互相分享。他们感觉上帝来到了他们身边。"
  summary: |
    四阶段纵向综合案例：桌面网站失败→移动版成功（可访问性=触发密度）；圣诞推送实验
    （预期遭投诉反被分享）；读经计划切分小片段+每日节奏（行动）；次日经句神秘感+
    "今日任务完成"钩形符号+链条不断（酬赏与人为推进效应）；高亮/书签/评论使应用成为
    "卷了边的书"（投入）；周日教堂人际传播与"谦虚地吹牛"（社交触发）。作者全程以自己
    启动"上瘾"读经计划的第一人称体验佐证。
  bound_to:
    - "上瘾模型四阶段总框架"
    - "频率优先"
    - "投入的链条效应（人为推进效应）"
  outcome: 1 亿台设备下载，应用商店《圣经》类目居首，估值或达 2 亿美元。
  tags: [case, hook-model, comprehensive]
```

```yaml
- id: c31
  title: Twitter"关注 30 人"临界点
  type: case
  source_chapter: 第8章（L2189–2198）
  source_quote: |
    "Twitter 发现，只要新用户关注的其他用户人数达到 30，即可达到一个临界点，极大地增加
    他们今后继续使用网站的可能性。"
  summary: |
    习惯路径的标杆样本：早期 Twitter 分析发现新用户关注满 30 人后留存概率大增，于是
    改进注册流程引导新用户立刻关注他人。示范"确定习惯用户→找路径→改产品"的完整闭环。
  bound_to:
    - "习惯路径与 5% 基准"
    - "习惯测试三步"
  tags: [case, habit-path, data]
```

```yaml
- id: c32
  title: Buffer 的诞生：解决自己的问题
  type: case
  source_chapter: 第8章（L2213–2219）
  source_quote: |
    "我很快意识到，将要发布的推文提前编入时间表，其效率要远远高得多。……这一过程相当
    烦琐，于是我产生了一个想法。"
  summary: |
    "照镜子"机会策略的实例：创始人加斯科因想多分享好内容，手动按时间表发推烦不胜烦，
    于是做定时发推工具，用户超 110 万。作者引用格雷厄姆"不要问'我应该解决什么问题'，
    要问'我希望其他人为我解决什么问题'"作为方法论包装。
  bound_to:
    - "机会四策源地（照镜子）"
  tags: [case, opportunity, founder]
```

```yaml
- id: c33
  title: 手机响了为什么没接（B=MAT 诊断例）
  type: case
  source_chapter: 第3章（L815–821）
  source_quote: |
    "可能是因为手机放在包里，你一时间没找到。……也许你以为对方是电话推销员，不想接听。
    ……就算你有强烈的动机，并且能轻易接通电话，但还是没接上，因为你压根儿就没听见。"
  source_quote_note: 三种解释合并摘引
  summary: |
    福格的示意案例：同一个"未接来电"有三种归因——够不着（能力受阻）、不想接（动机不足）、
    静音（触发缺失）。作者借它示范 B=MAT 作为诊断工具的用法：行为缺失时逐项排查，
    而不是笼统归因于"用户不感兴趣"。
  bound_to:
    - "B=MAT 福格行为模型"
  tags: [case, diagnostic, fom]
```

```yaml
- id: c34
  title: 动机三分类的广告例（希望/性卖点/社交/恐惧）
  type: case
  source_chapter: 第3章（L841–859）
  source_quote: |
    "像恐惧这一类的负面情绪也可以充当动机，而且效果甚佳。"
  source_quote_note: 四则广告案例合并摘引
  summary: |
    广告业是动机的直白实验室：奥巴马 2008 竞选海报打"希望"（趋希望避恐惧）；内衣/域名/
    汉堡广告用性卖点（趋快乐）；百威用好友助威画面（趋认同）；头盔广告用事故伤疤
    （避恐惧）。作者同时警示：对一部分人有效的动机对另一部分人可能适得其反。
  bound_to:
    - "动机三分类"
  tags: [case, motivation, advertising]
```

```yaml
- id: c35
  title: 操纵矩阵的正反例：哈里曼的努鲁国际 vs Cow Clicker
  type: case
  source_chapter: 第6章（L1914–1922、L1958–1963）
  source_quote: |
    "只有将自己变成那些农民中的一员，哈里曼才能设计出解决方案，满足那些农民的需求。"
    /"当该游戏走红，一些人不可救药地迷恋上该游戏之后，博格斯特关闭了游戏，引发了一场
    他所谓的'奶牛危机'。"
  summary: |
    操纵矩阵两端的对照组：前海军军官哈里曼为设计扶贫方案与肯尼亚农民同住（健康习惯
    推广者——先成为用户）；博格斯特开发的讽刺游戏 Cow Clicker 除了点击奶牛听"哞"声
    一无所有，却真有人沉迷（经销商/剥削利用的反面教材，作者用它佐证"本世纪的烟草"之讥）。
  bound_to:
    - "操纵矩阵（操控模式四象限）"
  tags: [case, ethics, contrast]
```

```yaml
- id: c36
  title: 移动应用的"一次使用"之殇与 Any.do 的应对
  type: case
  source_chapter: 第5章（L1755–1757）
  source_quote: |
    "2010年，移动应用程序的下载比例是 26％，但这些下载的应用程序仅被使用过一次。"
  source_quote_note: 原文为"下载比例是26%，但这些下载的应用程序仅被使用过一次"
  summary: |
    背景数据案例：约 26% 的应用下载后只被打开一次，使用频率随应用总数增多而下降。
    Any.do 的对策是在第一次使用时就教用户完成投入（连接日历）。用于说明移动端留存
    之难与"尽早开始投入"的必要性。
  bound_to:
    - "投入要分解成小块任务"
    - "加载下一个触发"
  tags: [case, retention, mobile]
```

```yaml
- id: c37
  title: 新生行为史料的四次打脸
  type: case
  source_chapter: 第8章（L2232–2246）
  source_quote: |
    "'美国人需要电话，但我们不需要，我们有足够的信差。'……'飞机是很有趣的玩具，但
    毫无军事价值'。"
  source_quote_note: 多则史料合并摘引
  summary: |
    判断新生行为之难的史料组：布朗尼相机被当 1 美元儿童玩具；邮政总工程师断言美国
    不需要电话；福煦元帅称飞机无军事价值；1957 年编辑断言数据处理是一时风尚；1995 年
    斯托尔《互联网？我呸！》。Facebook 从哈佛花名册到十亿用户。支撑"新生行为"机会
    扫描：早期用户的边缘行为可能就是主流习惯的雏形。
  bound_to:
    - "机会四策源地（新生行为）"
  tags: [case, history, opportunity]
```
