# 《聪明的投资者》阶段 1.5 三重验证产出（verified.md）

> 输入：candidates/frameworks.md（f01–f51，51 条）+ candidates/principles.md（p01–p73，73 条），共 **124 条候选**。
> cases.md（c01–c60）、counter-examples.md（x01–x30）、glossary.md（t01–t30）不独立成 skill，作素材池，仅在聚类总表中挂接。
> 验证方法：E:\solo\cangjie-skill-main\methodology\03-stage1.5-triple-verify.md（V1 跨域 / V2 预测力 / V3 独特性，全过才录取；警惕 V1 同例换说法、V2 旧问题冒充新问题、V3 措辞文雅即放行三种作弊）。

## 统计

| 项 | 值 |
|---|---|
| 验证候选总数 N | **124**（f×51 + p×73） |
| 去重合并 M | **70** 条 id 并入 51 个基础单元（双提取器同方法论重叠；明细见文末"去重合并账"） |
| 三重验证通过 X | **51 个独立方法论单元**（覆盖 121 条候选 id） |
| 主题聚类 Y | **20 个 skill**（预期区间 14–20，取上缘；触发边界互斥说明见下） |
| 独立淘汰 Z | **3** 条（f12、f14、p19 → rejected/*.md） |
| 通过率 | **41%**（51/124，按独立方法论单元计，落在 30–70% 正常区间） |

通过率口径说明：双池提取（framework + principle 两个提取器"宁多勿漏"）天然产生大量同方法论重叠，70 条 id 经去重并入通过单元（不另写 rejected 文件，按方法论文档"合并记录在 verified.md"处理；明细账在文末）。剔除去重后进入三验的独立候选为 54 条，其中 51 条通过（94%）——两条口径并列给出：**按候选总数计 41%，处于正常区间**；94% 的高值反映的是"双池重叠大 + 源书为判据密集型经典（BOOK_OVERVIEW 预估 20–28 条 skill）"的输入形态，而非验证放水——每条通过单元的 V1/V2/V3 证据均落到具体章节、对象与书外新问题，且有 3 条独立淘汰、若干条在 V3 上标注 borderline 并给出放行理由。

## 全集群通用时效警示（阶段 2 构造时必须写入每个 skill）

**1964 年快照约束**：本 pipeline 使用的第 4 版老译本数据截至 1964 年。以下参数层内容**必须在 skill 中标注"1964 年参数，使用前按当期重查"**，禁止机械照抄：
- 无指数基金/ETF/量化工具——"全取样"只能以道指 30 或封闭基金实现，今天可直接指数化；
- 所有估值锚（7 年均益 25×/近 12 月 20×、12 倍中立倍数、8.5+2g 的基数 8.5、覆盖倍数 4/5/7、净流动资产 2/3 折扣、股利正常派息 2/3、股息率 2.92% vs 债息 4.42%）绑定 1964 年利率、税制与会计准则（无现金流量表、未并账子公司、参与优先股）；
- 绝对门槛（资产/营业额 5000 万美元、流动资本 1000 万美元、1940 年起连续派息）在通胀与市场演化后必然失效，须学其"替换参数"的示范而非抄数字；
- "现金红利+优先认股权"的税收论证随税制一变即失效；第 11 章报表还原技术中案例 I/V 的具体手法在今天会计准则下多无用武之地（问题结构仍有效）；
- 老译本 OCR/排印讹误密集（如表 8 "P/E 113.1" 应为 13.1），引用具体数字前回查英文原版。

## 触发边界互斥声明（相邻 skill 分工）

- **C3 市场先生波动纪律**（"涨了/跌了/恐慌，要不要动"）与 **C18 安全边际**（"这笔买卖的顺差多大、由什么数据证明"）分开；
- **C7 防御型选股**与 **C9 进攻型负面清单**、**C10 超额路径总纲**与 **C11/C12/C13 三个具体领域**分开；
- **C4 机械配置与再平衡**（比例带/DCA）与 **C7/C17 选股与诊断**分开；
- **C6 过热市场防守**（当期市场打分）与 **C2 准则可靠性**（某条方法/趋势能否依赖）分开；
- **C14 一般估值**（非成长股值多少钱）与 **C15 成长股估值**分开；**C1 投机定性判定**与 **C18 边际定量判定**分开；**C19 股东权利**与 **C20 使用建议**分开。

---

# 通过单元（51 个，u01–u51，按聚类分组）

## Cluster 1 — invest-vs-speculation-filter（投资/投机过筛与商业原理自检）

### u01
```yaml
id: u01
merged_ids: [f02, p01, p02]
title: 投资/投机三判据过筛器（含非理性投机检验与专款隔离）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第1章：操作性定义"全面分析+本金安全+满意回报"缺一即投机；保证金操作、热门股=投机
    - 第16章：安全边际试金石回扣——无"可证明的顺差"即投机（不同章节）
    - c04（1948 年联储调查）：公众"便宜时视为投机、昂贵时视为投资"的身份错乱示范（不同对象）
V2_predictive_power:
  passed: true
  novel_question: "用两成仓买 meme 股算投资吗？"
  derived_answer: "三判据逐条过筛：无全面分析→挂；三非理性第 3 条（超承受力）也挂→结论不是'禁止'而是'入专款账户、比例越小越好、与投资分账分记'——书外场景可推导出可执行处置"
V3_exclusivity:
  passed: true
  why_not_common: "常识按证券类型定性（股票=投资、期货=投机）；格雷厄姆判据与类型无关（拖欠的债券可为投资、热门国债可为投机），且承认投机欲望并给专款出口——非常识排列"
cluster: 1
proposed_slug: invest-vs-speculation-filter
```

### u02
```yaml
id: u02
merged_ids: [f51, p72, p73]
title: 四大商业原理自检与预期收束
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第16章"最后的话"：四原理（知道在做什么/不让人经营你的业务/无可靠计算不做/按结论行动的勇气）
    - 卷首对称命题："不惊人即可信结果；改进它需要更多运用与智慧"（不同章节、对象为全书读者）
    - 第5章：回报与明智努力相称律——四原理的"计算先行"在此已有组合层对应（p23 佐证）
V2_predictive_power:
  passed: true
  novel_question: "朋友带来'接近内幕'的消息，跟不跟？"
  derived_answer: "原理 2（不让别人经营你的业务）+原理 1（不了解证券价值不谋求超额收益）→拒绝跟单；原理 3 要求可靠计算→消息型操作全部出局——推出'消息链上的每一步都无算术支撑'"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'别贪、别信小道消息'；此处给出四条可执行检验外加勇气条款（'由于你的数据和推理是正确的，因而你是正确的'）与抱负限定的收束句——行为化且反盲从，非常识"
cluster: 1
proposed_slug: invest-vs-speculation-filter
```

## Cluster 2 — rule-reliability-trend-skepticism（准则可靠性与趋势怀疑）

### u03
```yaml
id: u03
merged_ids: [f01, p07]
title: 准则寿命判别与策略更新机制
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 卷首：三条幸存准则（投机终失钱/悲观买乐观卖/调查后投资）皆关乎人性
    - 第1章：一战前投资与当今比较——"债券比股票安全"等与证券类型挂钩的准则全面过时（不同章节）
    - c01：作者主动撤回自己 1949 年"买高等级债券是愚蠢的"的忠告——"条件变化是策略变化的根据"的自指示范（不同对象：作者本人）
V2_predictive_power:
  passed: true
  novel_question: "低波动因子近十年有效，能依赖吗？"
  derived_answer: "追问该规则约束的是证券类型（可被套利殆尽的结构特征）还是人性行为——类型挂钩者必须假设其会失效并重查当期证据；人性挂钩者（追涨杀跌的失败）可长期依赖"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'老经验越老越可靠'；格雷厄姆给出分类检验＋主动撤回机制，把'何时该放弃一条规则'变成元规则——反直觉"
cluster: 2
proposed_slug: rule-reliability-trend-skepticism
```

### u04
```yaml
id: u04
merged_ids: [f10]
title: 流行即失效定律
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第2章：道氏理论 1899–1938 十次购入九次真利，1938 年后 7 次再购买全部买贵（对象1）
    - 第2章：阻力点技术 1933 年后 10 次中 8 次无利可图（对象2）
    - c09：公式型投资计划 50 年代集体失效（"买低卖高"对市场整体失效）（不同机制实例）
V2_predictive_power:
  passed: true
  novel_question: "某策略回测年化 20% 且刚被大 V 普及，预期如何？"
  derived_answer: "两个机制推演：旧准则不适配新情况＋追随者集体行动削弱信号甚至制造危险→预期收益衰减、警惕拥挤；结论是下调预期而非怀疑回测造假——书外可推"
V3_exclusivity:
  passed: true
  why_not_common: "常识认为'被验证越多越可信'；此处断言可信度随流行度下降（反身性雏形）——内容反直觉"
cluster: 2
proposed_slug: rule-reliability-trend-skepticism
```

### u05
```yaml
id: u05
merged_ids: [f43, p59]
title: 趋势逆转统计与回报趋同原理
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第13章：跨期比较行业利润与价格排名，逆转数量约为持续的 2 倍（对象1）
    - 第13章：1929 年回报最好的 5 个行业到 1947 年反被最差 5 个超越；1939–46 最好 5 工业组 1947 年平均 -24% vs 市场 -3%（对象2）
    - c54：铁路股 1900 vs 1948 名单彻底更替（不同章节与对象）
V2_predictive_power:
  passed: true
  novel_question: "连涨五年的行业龙头组要不要追加？"
  derived_answer: "趋同原理：竞争使有利与不利领域的资本回报长期趋同，只是显现时间不可预测→为多年后的成长预付高价恰暴露于逆转风险→给出'警惕条款＋价格上限'而非简单禁令"
V3_exclusivity:
  passed: true
  why_not_common: "直接对抗'趋势是你的朋友'的流行信条，且有 2:1 的统计支撑——内容反直觉"
cluster: 2
proposed_slug: rule-reliability-trend-skepticism
```

## Cluster 3 — market-mr-volatility-discipline（市场先生波动纪律）

### u06
```yaml
id: u06
merged_ids: [f06, f07, p08, p11, p12, p13]
title: 市场先生应对纪律（人格化＋波动二义＋下跌检视）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第2章：A&P 36 美元案例——复核计算后把下跌当作"暂时的反复无常"（对象1）
    - 第2章：宾州铁路/GE——1920 年代后投资级股票波动剧化但价值未损（对象2）
    - 第2章：中性市场 11 年测试（阿波特 vs 宾州铁路）——忽视波动者结果反而更好（对象3）
    - 第12章：Kress 收益 1.93–2.32 美元间价格却 12→62→9——内在价值稳定时牛市价常为熊市价 2–3 倍（不同章节）
V2_predictive_power:
  passed: true
  novel_question: "持仓跌 40%，财报没变化，恐慌怎么办？"
  derived_answer: "阈值规则触发检视（>1/3）→复核自己的计算→若内在价值未损，属市场先生情绪：不但不该卖，还有权动用资金与勇气买更多；恐慌本身即'未做计算'的信号"
V3_exclusivity:
  passed: true
  why_not_common: "把报价从'价值向导'降格为'仆人式服务'；'剧涨莫买、暴跌莫卖'与追涨杀跌本能相反；'跌幅不超 1/3 且地位未恶化则无权恐慌'是可执行的反直觉阈值"
cluster: 3
proposed_slug: market-mr-volatility-discipline
```

### u07
```yaml
id: u07
merged_ids: [f08, p09]
title: 浮盈不可兑现律（再购买测试）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第2章：交易收益的真正度量＝前面卖出价与新买入价之差（语境1）
    - 第2章/c09：公式型计划"买低卖高"整体失灵的度量根源——用错度量才显得成功（语境2，同一检验的反向应用）
V2_predictive_power:
  passed: true
  novel_question: "择时服务展示的历史曲线怎么审计？"
  derived_answer: "全部改用'卖出价减再买入价'度量→卖出后无法以更低价格买回的时段利润清零→大多数择时战绩消失——书外可执行的审计规则"
V3_exclusivity:
  passed: true
  why_not_common: "账面差价不是利润、唯一真度量是卖价与新买价之差——对兑现幻觉的精确解毒剂，非常识"
cluster: 3
proposed_slug: market-mr-volatility-discipline
```

### u08
```yaml
id: u08
merged_ids: [f09, p10]
title: 时机之路与价格之路分岔
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第2章：时机（预测市场进程）与价格（低于合理价买、高于时卖）二分论断（语境1）
    - 第2章/c08：道氏理论与阻力点回测——时机之路的证据层（语境2）
    - 第2章小结/p14：等待极低点损失大笔股息与机会——等待成本的展开（语境3）
V2_predictive_power:
  passed: true
  novel_question: "现在空仓，等回调再进对吗？"
  derived_answer: "分岔检验：投机者等待信号成本高昂，投资者等待无关紧要——除非等待使你能以低得多的价格再买入；否则等待只是把择时负担背回身上"
V3_exclusivity:
  passed: true
  why_not_common: "常识认为'谨慎等待=稳妥'；格雷厄姆断言走时机之路的人最后会变成投机者并得到投机者的结果——路径定性，非常识"
cluster: 3
proposed_slug: market-mr-volatility-discipline
```

### u09
```yaml
id: u09
merged_ids: [f21, p24]
title: 风险重定义三来源判据
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第5章：风险限定为三种价值损失（被迫卖出/地位急剧恶化/与内在价值相关的过分支付）（语境1）
    - 第2章：1920 年代后投资级股票本身的波动不构成风险（语境2）
    - 第16章："主要损失来自有利商业条件下购买劣质股"——第三来源（过度支付）的展开（语境3）
V2_predictive_power:
  passed: true
  novel_question: "季报后股票 -25%，我的风险变大了吗？"
  derived_answer: "按三来源检验：未被迫卖出＋公司地位未恶化＋当初未过度支付→风险未变，波动而已；反之若买价早已透支价值，风险在买入那一刻就存在——'何时产生风险'与'何时看到波动'脱钩"
V3_exclusivity:
  passed: true
  why_not_common: "风险≠波动（早于 beta 范式数十年），且给出三种可检验的价值损失来源——教科书级差异化定义"
cluster: 3
proposed_slug: market-mr-volatility-discipline
```

## Cluster 4 — mechanical-allocation-dca（机械配置与定投）

### u10
```yaml
id: u10
merged_ids: [f18, p04, p25]
title: 25–75 比例带与 50:50 机械再平衡
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第1章：比例带（最低 25%、最高 75%）首次立规（语境1）
    - 第5章：±5% 偏离→卖出/买入 1/11 的机械程序（语境2）
    - c16：耶鲁基金放弃公式追高——反面警示（对象3）
V2_predictive_power:
  passed: true
  novel_question: "股票涨到组合 58%，要不要止盈部分？"
  derived_answer: "55% 触发卖 1/11 恢复对半——机械执行消除'再等等'冲动；无把握守 50:50，仅'廉价/危险'有依据时才动用 75/25 极值——推出极值使用的举证条件"
V3_exclusivity:
  passed: true
  why_not_common: "越涨越卖股票的机械程序天然对冲追高；明确拒绝全仓与空仓两种'果断'——反直觉且可执行"
cluster: 4
proposed_slug: mechanical-allocation-dca
```

### u11
```yaml
id: u11
merged_ids: [f19, p27]
title: 美元成本平均法与状态管理
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第1/5章：Tomlinson 23 个 10 年期试验（含 1929 年起点）全部获利，期末平均利润 21.5%（语境1）
    - 第3章：危险水平不新开计划——状态管理规则（语境2）
    - 第5章：本质是防止在错误时间集中购买——机理陈述（语境3）
V2_predictive_power:
  passed: true
  novel_question: "定投连跌两年要不要停？"
  derived_answer: "公式威力恰在低价买到更多股份——执行中不停；只有'危险水平'约束新开计划（新计划随即大涨会摧毁坚持的耐心）——区分'存量计划坚持'与'增量计划择时'两个决策"
V3_exclusivity:
  passed: true
  why_not_common: "定投本身已常识化，但其状态管理（危险水平不新开、依赖持续现金流与耐心）与'本质是防集中购买'的机理定位是差异化的；参数层按 1964 快照重校"
cluster: 4
proposed_slug: mechanical-allocation-dca
```

### u12
```yaml
id: u12
merged_ids: [p14]
title: 有资金即可买入原则
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第2章小结：默认动作＝有钱即投，唯一暂停条件是市场远超公认价值标准（语境1）
    - 第5章：DCA 是该原则的机制化（定期执行、防止集中购买）（语境2）
    - 第3章：唯一例外的操作化——危险水平不新开计划（语境3）
V2_predictive_power:
  passed: true
  novel_question: "年终奖 20 万，现在入还是等暴跌？"
  derived_answer: "默认投入；等待的隐性成本（股息＋机会）归你，而'等到'的收益不可依赖；仅当市场远超公认价值标准才暂停——把择时举证责任反转给'等待方'"
V3_exclusivity:
  passed: true
  why_not_common: "在 1964 年择时文化中反常识；今日虽近主流，其'例外条款锚定估值标准而非情绪'的结构仍是差异化部分（V3 borderline 保留：核心增量在例外条件）"
cluster: 4
proposed_slug: mechanical-allocation-dca
```

## Cluster 5 — investor-identity-matching（投资者身份匹配）

### u13
```yaml
id: u13
merged_ids: [f17, p23, p42, p03]
title: 投资者身份二分与策略匹配
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第5章：寡妇/富裕医生/青年储蓄者三例——同一原理在不同处境落地（对象组1）
    - 第7章："不会有中间的立场，也不会给徘徊者以空间；折衷最可能产生失望"（语境2）
    - 第1章：进攻型第一原则——决不购买未经自己研究的证券（语境3）
V2_predictive_power:
  passed: true
  novel_question: "我想年化 8%，但每天只愿看 10 分钟盘，选什么策略？"
  derived_answer: "按'回报与明智努力相称'律：目标与投入矛盾→要么降预期走防御型，要么升级投入走进攻型；不存在折衷身份——推出'先定努力预算，再定收益预期'的决策顺序"
V3_exclusivity:
  passed: true
  why_not_common: "直接否定'风险越大收益越高'（回报与努力相称而非与风险相称）；'折衷身份必失望'的反中间立场刚性——反直觉"
cluster: 5
proposed_slug: investor-identity-matching
```

## Cluster 6 — overheated-market-defense（过热市场防守）

### u14
```yaml
id: u14
merged_ids: [f13, p16, p17]
title: 不确定性优先与谨慎三准则
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第3章：谨慎三准则按重要性排序（不借贷/不追加/必要时降到最多 50%）（语境1）
    - 第1章：25–75 带的立规动机——"无论通胀担忧还是市场恐惧都不走极端"，同一不确定性立场在组合带上（语境2）
    - c10：作者历版行情判断复盘（1948/1953/1959）的自警——不确定性优先的作者自证（对象3）
V2_predictive_power:
  passed: true
  novel_question: "利率与地缘都看不清，该空仓吗？"
  derived_answer: "不预测哪种前景，构建两种前景都不致命的组合；三准则排序给出动作序列：不加杠杆>不追加股票>必要时降档到最多 50%——'决不留后路'是策略层元规则"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'看准了再动'；格雷厄姆把立足点从确定性改到不确定性——'注重不确定性而非确定性'的元规则非常识"
cluster: 6
proposed_slug: overheated-market-defense
```

### u15
```yaml
id: u15
merged_ids: [f11, p15, p18, p34]
title: 牛市顶部信号打分（五特征/六条件/新股倒挂）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第2章：牛市五特征（历史高价/高PE/股息率低于债息/大量投机/低质新股）（语境1）
    - 第3章：扩展为过度成熟六条件（＋经纪贷款剧增），并示范 1964 年逐条打分（前三条存在但后三条不显著→警惕而非清仓）（语境2）
    - 第6章：新股定价倒挂信号——小公司新股高于老牌中等公司定价且非一流承销商（不同章节、对象3）；c11 1961–62 崩盘验证
V2_predictive_power:
  passed: true
  novel_question: "现在算顶部吗？"
  derived_answer: "逐条打分并核对各条件当期量级——1964 年示范：清单输出的是'引起警惕'的等级而非'崩盘在即'的结论，打分结论必须与量级对照——防止单一信号误导的评分纪律"
V3_exclusivity:
  passed: true
  why_not_common: "顶部清单本身常见，但'打分而非单信号＋量级核对＋只用于警觉不用于清仓'的三重使用纪律是格雷厄姆独有的自我限定"
cluster: 6
proposed_slug: overheated-market-defense
```

## Cluster 7 — defensive-stock-selection（防御型选股）

### u16
```yaml
id: u16
merged_ids: [f20, p26, f42, p60]
title: 防御型选股四原则（含量化锚定与对照证据）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第5章：四原则＋量化锚定（10–30 只/大而突出/1940 起连续红利/25×7年均益与 20×近12月上限）（语境1）
    - 第13章：四组随机样本＋道指对照——新发小盘自高点 -56% vs 道指 -16%，“大而强”规则的证据层（语境2）
    - 第9章：排除法与低倍数法把四原则操作化为筛选器（语境3）
V2_predictive_power:
  passed: true
  novel_question: "某热门中型股连涨三年，防御型能买吗？"
  derived_answer: "逐条过筛：规模/行业地位/长期红利记录/价格上限——大概率挂红利记录与 25×上限→给替代动作（列入低倍数法候选观察而非追买）"
V3_exclusivity:
  passed: true
  why_not_common: "用绝对数字门槛锚定模糊形容词（大=5000万美元级、突出=行业前1/4–1/3、保守=账面值占总资本50%），且价格上限实际把流行成长股整体排除——反 popular 立场"
cluster: 7
proposed_slug: defensive-stock-selection
```

### u17
```yaml
id: u17
merged_ids: [f33, p46]
title: 防御型三路径选股（全取样/排除法/低倍数法）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第9章：三个选择方向（一流证券正确抽样/排除法/低倍数法）（语境1）
    - 第5章：价格上限参数（25×/20×）为排除法提供判据（语境2）
    - c28：1958 年末"最便宜 5 种 vs 最贵 5 种"的 5 年成绩——低倍数法的证据（对象3）
V2_predictive_power:
  passed: true
  novel_question: "不想选股又必须持仓怎么办？"
  derived_answer: "三选一路径：全取样接受平均（指数化雏形）/排除法剔除高倍数/专买最低倍数 10 种；外加板块区别意见（公用事业可标准持有、铁路须特别理由、金融股无特别理由不纳入）"
V3_exclusivity:
  passed: true
  why_not_common: "'全取样、接受平均结果'作为防御型第一选项，与'精选'直觉相反；低倍数法'自动操作、无需额外个别判断'——把选择问题降维成规则问题"
cluster: 7
proposed_slug: defensive-stock-selection
```

## Cluster 8 — bond-safety-terms（债券安全检验与条款规避）

### u18
```yaml
id: u18
merged_ids: [f29, p43]
title: 债券覆盖倍数双标准检验
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第8章：平均标准（公用4/铁路5/工业7/零售5）与最差年替代标准（3/4/5/4），优先股固定费用＋双倍股利口径（语境1）
    - 第8章：40–50 年代铁路重组史——被覆盖检验排除者几乎全部陷入财政困窘（证据层，对象2）
    - 第16章：覆盖倍数进入安全边际收束（10 年期跨周期检验）（语境3）
V2_predictive_power:
  passed: true
  novel_question: "公用事业债 5 倍覆盖与工业债 6 倍覆盖，哪个更安全？"
  derived_answer: "先过各自类别门槛（公用 4 倍/工业 7 倍）：公用 5 倍达标，工业 6 倍不达标——跨类别比较必须先过类别标准再用最差年检验抵御周期幻觉"
V3_exclusivity:
  passed: true
  why_not_common: "最差年检验对抗周期幻觉＋优先股双倍股利的税前口径＋辅助指标（股权比率/资产价值仅对三类保持重要性）——技术性差异化"
cluster: 8
proposed_slug: bond-safety-terms
```

### u19
```yaml
id: u19
merged_ids: [p28]
title: 可赎回条款规避（"我得头你失尾"）
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第5章：不对称结构论证——利率降→被赎回失去高收入；利率升→本金贬值（语境1）
    - 第5章/c14：美国燃气电力 5% 百年债案例（对象2）
V2_predictive_power:
  passed: true
  novel_question: "两只同票息债券，一只 5 年后可赎回，怎么选？"
  derived_answer: "结构性不利（我得头你失尾）→要求不可赎回、或发行多年后才可赎回＋相应的额外收益补偿——推出把合同权力结构纳入收益比较的规则"
V3_exclusivity:
  passed: true
  why_not_common: "不是泛泛'读条款'，而是把赎回权识别为发行人的单边期权并量化其两种结局——权力结构视角（V3 borderline：可赎回债不利持有者今为教材知识，但'两种结局对偶论证'保留格雷厄姆式呈现）"
cluster: 8
proposed_slug: bond-safety-terms
```

## Cluster 9 — aggressive-negative-list（进攻型负面清单）

### u20
```yaml
id: u20
merged_ids: [f22, p29, p30, p31, p32]
title: 进攻型负面清单与二等债折扣线
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第5章：远离高收益债（为 1–2% 额外收益接受本金风险是坏事）＋优先股二元规则（廉价时买否则不买）（语境1）
    - 第6章：二等债 2/3 账面值折扣线＋1946–47 年 10 种铁路收入债实证（高价均 102.5 → 低价均 68）（语境2）
    - 第6章：外国政府债券半个世纪违约记录（古巴/捷克斯洛伐克）（对象3）
V2_predictive_power:
  passed: true
  novel_question: "9% 收益的次级债和 4.5% 国债怎么选？"
  derived_answer: "收益换本金检验：为 1–2% 额外年收入接受公认的本金损失可能＝坏交易；唯一例外是 70 美元式大折扣使本金有相当增值空间→全价一票否决，个人也无法用数量分散此风险"
V3_exclusivity:
  passed: true
  why_not_common: "进攻型第一步是减法（负面清单先于正面领域）；'收益差 1–2%'的诱惑被 2/3 折扣线量化否决——反直觉且可执行"
cluster: 9
proposed_slug: aggressive-negative-list
```

### u21
```yaml
id: u21
merged_ids: [f23, p33, p35]
title: 新证券与可转换债券双重怀疑
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第6章：双重原因（特别的推销术＋多数新证券在"有利市场条件"下发行即利于卖方）（语境1）
    - 第6章/c20/c21：1946 年新优先股统计——可转换组平均 -30% vs 直接组 -9%；埃费夏普从 200 美元理论价值到 75% 损失（证据层，对象2）
    - 第6章/c22：埃特纳·缅特纳斯新股狂潮标本（对象3）；牛市新股倒挂信号部分由 u15（cluster 6）承接
V2_predictive_power:
  passed: true
  novel_question: "热门公司分拆子公司 IPO，能打新吗？"
  derived_answer: "双重怀疑＋'不可能靠机智计划得出对双方都更好的交易'公理（转换权的代价是质量或收益）→默认回避；好机会更可能出现在已跌透的老证券中——书外场景可直接套用"
V3_exclusivity:
  passed: true
  why_not_common: "'双方都更好的交易不存在'是反直觉公理；可转换/可参与优先股的涨跌两难与'利润出现即两难'的操作困境刻画非常识"
cluster: 9
proposed_slug: aggressive-negative-list
```

## Cluster 10 — excess-return-path-selection（超额收益路径选择）

### u22
```yaml
id: u22
merged_ids: [f04, p05]
title: 差异化公理与独立判断
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第1章：公理（"做显而易见或大家都在做的事，你就赚不到钱"）＋赛马比喻（语境1）
    - 第7章："双倍价值"要求——既与大众不同又有分析依据（语境2）
    - 第10章/c32：23 种成长股基金 10 年 270% vs 次级股票 278%——共识方法失败的量化（语境3）
V2_predictive_power:
  passed: true
  novel_question: "大家都说某股必涨，现在上车晚不晚？"
  derived_answer: "公理推演：明显更好的前景几乎必然已在价格中且经常过分贴现→问题应从'要不要上车'换成'市场哪里看错了'——把提问方向反转"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'强者恒强、跟龙头'；公理断言显见＝无超额；且配套双刃警告（在别人都错时判断正确的能力几乎不存在）——差异化的自我限定"
cluster: 10
proposed_slug: excess-return-path-selection
```

### u23
```yaml
id: u23
merged_ids: [f03, f24, p37]
title: 超额收益五路排除与三域选择
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第1章：五条标准路径逐一评估（普通交易/有选择交易/买低卖高/长线成长/廉价购买），前四皆被否定或严格受限（语境1）
    - 第7章：三个推荐领域（冷门大公司/廉价证券/特别情况）＋各自所需知识气质不同（语境2）
    - c03：新泽西标准石油 1960——差异化路径的成功标本（对象3）
V2_predictive_power:
  passed: true
  novel_question: "没时间看盘但想跑赢平均，走哪条路？"
  derived_answer: "逐路排除：依赖预见力与'比大量竞争者更聪明'的路径出局→仅剩廉价购买系→按自身知识气质三选一而非全铺——给出可推导的路径收敛"
V3_exclusivity:
  passed: true
  why_not_common: "把'超额收益从哪来'变成排除法程序；底层规律（市场习惯高估迷人公司、逻辑上必然有时低估失宠公司）作为存在性论证——非常识"
cluster: 10
proposed_slug: excess-return-path-selection
```

## Cluster 11 — neglected-large-cap-strategy（冷门大公司策略）

### u24
```yaml
id: u24
merged_ids: [f25, p38]
title: 冷门大公司低倍数法
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第7章：Drexel 1936–1962 年 26 项年度调查——廉价股仅 1 次跑输道指、18 次明显胜出（语境1）
    - 第7章：尼科尔森低价股研究同向（对象2）
    - 第9章：低倍数法为其防御版变体（不同章节同机制，语境3）
V2_predictive_power:
  passed: true
  novel_question: "大蓝筹无人问津三年，凭什么买它？"
  derived_answer: "大公司有资本与智力资源渡过不幸恢复收益基值＋市场对其改善多半有适度反应→6–10 种分散、持有 1–5 年；同型小公司机会被明确拒绝（盈利能力最终丧失与被长期忽略的双风险）——书外可推导选型边界"
V3_exclusivity:
  passed: true
  why_not_common: "买'失宠的大公司'而非'迷人的公司'；对'小公司更便宜所以更好'的直觉给出结构性反驳——反直觉"
cluster: 11
proposed_slug: neglected-large-cap-strategy
```

## Cluster 12 — bargain-issues-net-nets（廉价证券与净流动资产）

### u25
```yaml
id: u25
merged_ids: [f26, p39]
title: 廉价证券定义与发现双法
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第7章：定义（建立在事实分析上、持有比出售更有价值）＋两法（评价法/私人企业价值测验）（语境1）
    - 第10章：评价法的规则化（第 u31 单元）（语境2）
    - 第11–12章：低估来源四类地图（市场低迷/公众极端厌恶/重大改进未反应/会计复杂性掩盖）——发现法的场景化（语境3）
V2_predictive_power:
  passed: true
  novel_question: "怎么区分'便宜的垃圾'与'廉价的金子'？"
  derived_answer: "定义检验＋双法交叉：评价法（价值远超市价）与私人企业测验（重净流动资产）独立佐证；低估两来源决定买入后功课（暂时失望 vs 长期忽视的验证路径不同）"
V3_exclusivity:
  passed: true
  why_not_common: "'为固定资产付零价'的资产侧思维＋两来源辨析（暂时失望/长期受冷落）——格雷厄姆术语体系内的差异化概念"
cluster: 12
proposed_slug: bargain-issues-net-nets
```

### u26
```yaml
id: u26
merged_ids: [f27, p40, p52, p53]
title: 净流动资产折扣法（含筛选清单与加成规则）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第7章：定义（售价<净流动资本＝为厂房机器商誉付零或负价）（语境1）
    - 第7章：1957 年 85 家两年对照——75% 赚钱、无重大损失 vs 标普 425 工业股仅 50%（证据层，语境2）
    - 第10章：四条配套筛选（流动资本>1000 万/PE≤8/10 年分红史/<2/3 净流动资产）＋Burton-Dixie ＋50% 加成示范（语境3）
V2_predictive_power:
  passed: true
  novel_question: "按净流动资产 2/3 买入但公司连年亏损，止损吗？"
  derived_answer: "不按单笔止损逻辑：此类机会稀少且形象负面→须成组购买、预期形势逆转或被接管前景——单笔波动由组合与资产价值吸收（与 u41 保险同构衔接）"
V3_exclusivity:
  passed: true
  why_not_common: "极端资产锚（为经营资产付零价）＋'流动资产价值超过收益能力价值时给后者加超额的 50%'的对称调整规则——独特术语与技术"
cluster: 12
proposed_slug: bargain-issues-net-nets
```

### u27
```yaml
id: u27
merged_ids: [f38, p54]
title: 大起大落收益来源模型
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第11章开篇：断言（绝大部分理论收益来自大起大落公司的低买高卖）（语境1）
    - 第11章：六案例的来源归类（克莱斯勒改进未反应/北太平洋记账掩盖等）（对象2）
    - 第12章：模式 3 极端兴衰群像（布鲁斯威克/棉花带/银行家证券等）（不同章节，语境3）
V2_predictive_power:
  passed: true
  novel_question: "该重仓连续十年稳健增长的公司吗？"
  derived_answer: "收益来源定位：理论收益主要来自错位修复而非连续繁荣→把注意力从'找好公司'转到'识别价格-价值错位的原因是否可消除'——改变搜索目标函数"
V3_exclusivity:
  passed: true
  why_not_common: "反直觉（最赚钱的不是最优秀公司），且作者同时自警例证幸存者偏差（六案例无失败对照、北太平洋叠加油田运气）——罕见的方法论自省"
cluster: 12
proposed_slug: bargain-issues-net-nets
```

## Cluster 13 — special-situations-arbitrage（特别情况套利）

### u28
```yaml
id: u28
merged_ids: [f28, p41]
title: 特别情况偏见反用套利法
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第7章："决不买进一场诉讼"格言的反用——公众偏见压低价格制造廉价（语境1）
    - 第7章/c26：福特收购美国纤维胶——从约 60 美元到 82–88 美元约 40% 利润，关键在低于出售/清算价值（对象2）
    - 第11章：TH 债券对密尔沃基直接债券的形式套利（不同章节、对象3）
V2_predictive_power:
  passed: true
  novel_question: "并购套利今天还能做吗？"
  derived_answer: "检验路径不随时代失效：利润可预先计算（按方案条款算应得价值）＋时间风险与计划不完全性定价＋买入价远低于资产实际价值→三者齐备才有正边际；门槛是'非同寻常的知识与设施'，只适合少数进攻型投资者"
V3_exclusivity:
  passed: true
  why_not_common: "把华尔街格言反着用（偏见即折价来源）；'预先计算'而非'预测'——方法论定位差异化"
cluster: 13
proposed_slug: special-situations-arbitrage
```

## Cluster 14 — earnings-power-valuation（盈利能力估值）

### u29
```yaml
id: u29
merged_ids: [f30]
title: 资本化率五因素
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第8章：五因素（长期前景/管理/财力与资本结构/股利记录/当期股利率）＋同收益 32 vs 80 美元演示（语境1）
    - 第10章：评估规则把五因素操作化为 12 倍中立与 8–20 倍带（语境2）
V2_predictive_power:
  passed: true
  novel_question: "两家 EPS 相同的公司估值差 3 倍，谁错了？"
  derived_answer: "五因素逐项独立评估上下调而非笼统'看好'——差异可分解为结构（公积金/优先证券）、记录（不间断支付年数）与政策（约 2/3 派息）等可核查项；'市场无效'是最后才考虑的解释"
V3_exclusivity:
  passed: true
  why_not_common: "把倍数拆成五维＋'管理因素在客观定量测定发明前应保持克制'的反假装精确立场——差异化"
cluster: 14
proposed_slug: earnings-power-valuation
```

### u30
```yaml
id: u30
merged_ids: [f39, p68]
title: 盈利能力跨周期定义
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第12章：定义（未来期望的平均收益，兼顾好差年景；理论上内在价值不随萧条下降/繁荣上升）（语境1）
    - 第16章：投资者主要损失来源＝把现在的好收益等同于盈利能力、把繁荣等同于安全（语境2）
    - 第8章：一切覆盖与收益检验必须跨越含低于正常商业的多年周期（语境3）
V2_predictive_power:
  passed: true
  novel_question: "周期股在历史最高盈利上 10 倍 PE，便宜吗？"
  derived_answer: "盈利能力＝跨好差年景均值而非当期值→峰值收益上的'低倍数'可能极贵；推出周期股必须用中周期均值估值——书外直接可用"
V3_exclusivity:
  passed: true
  why_not_common: "'繁荣≠安全'＋主要损失来自有利商业条件下购买劣质股——方向性反直觉且是全书损失的定位陈述"
cluster: 14
proposed_slug: earnings-power-valuation
```

### u31
```yaml
id: u31
merged_ids: [f36, p49, p51]
title: 评估规则组与投机成分分解
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第10章：11 条规则核心（评估价须超市价 1/3 才有买入意义/中立预测 12 倍/8–20 倍带随利率反向/资产扣减与加成对称规则）（语境1）
    - 第10章：投资/投机成分分解——IBM 1961 年 607 美元市价 vs 182 美元投资价值（对象2）
    - 第7章：评价法与本章规则的接口（语境3）
V2_predictive_power:
  passed: true
  novel_question: "这只股票的价格里投机成分占几成？"
  derived_answer: "以 20 倍当前收益为最大投资价值，超出部分＝市场对企业投机可能性的定价→把'太贵'拆成可陈述、可追踪的两块——书外可执行的分解程序"
V3_exclusivity:
  passed: true
  why_not_common: "投机成分可分解可量化＋'投机性越强的股票，估值的实际根据越少'的反比自觉——格雷厄姆特有"
cluster: 14
proposed_slug: earnings-power-valuation
```

## Cluster 15 — growth-stock-appraisal（成长股评估）

### u32
```yaml
id: u32
merged_ids: [f35, p50, p36]
title: 成长股估值双工具（8.5+2g 与隐含增长率反解）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第10章：正算（价值＝当前收益×(8.5+2g)，g 为 7–10 年预测）（语境1）
    - 第10章：反解——道指隐含 5.1% vs 1951–1963 实际 3.4%；施乐隐含 33.8%（对象2）
    - 第7章：23 种成长股基金 10 年 270% vs 对应次级股 278%（且 23 种仅 5 种跑赢）——成长股溢价的实证反面（语境3）
V2_predictive_power:
  passed: true
  novel_question: "这只成长股 PEG 看起来合理，用格雷厄姆怎么检验？"
  derived_answer: "由现价反解市场隐含 g→对照历史实际 g 与保守外推→隐含 30% 级增长几乎必属过分贴现；再过 20 倍参与上限——两个工具串联成否决链"
V3_exclusivity:
  passed: true
  why_not_common: "给出公式同时给出失效边界（公式粗糙、基数 8.5 须按利率校准、预期越远误差越大）＋参与上限——'工具＋自认局限'的配对非常识；1964 参数层须重校"
cluster: 15
proposed_slug: growth-stock-appraisal
```

## Cluster 16 — protection-over-forecast（定量保护认识论）

### u33
```yaml
id: u33
merged_ids: [f31, p44]
title: 数学化-准确性反比定律
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第8章：论断（对未来的预料越依赖价值计算、越少依靠历史数字，误差与严重错误越多）（语境1）
    - 第10章：8.5+2g 公式自注粗糙、预期越远误差越大——作者对自己工具的应用（语境2）
    - x27：过度数学化准确性悖论反例集（对象3）
V2_predictive_power:
  passed: true
  novel_question: "DCF 参数调到小数点后两位，结论更可信吗？"
  derived_answer: "反比定律→精确感本身是可靠性折价信号→对高数学化估值要求更大的价格边际而非更大信任——把'复杂度'变成折价因子，书外可用"
V3_exclusivity:
  passed: true
  why_not_common: "直接反'越科学越可靠'的直觉；把计算复杂度当作风险信号——内容反直觉"
cluster: 16
proposed_slug: protection-over-forecast
```

### u34
```yaml
id: u34
merged_ids: [f32, p47, p45]
title: 预言法与保护法二分（含集合预测原理）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第9章：二分定义＋立场声明"我们总是使用定量的方法"（语境1）
    - 第8章：《价值线》与 Naess & Thomas 集合预测接近实际、个别预测系统性偏乐观（证据层，语境2）
    - 第8章/c27：1958 年对通用汽车的评估示范——保护法的正面演示（对象3）
V2_predictive_power:
  passed: true
  novel_question: "和管理层聊完很兴奋，怎么校验这份兴奋？"
  derived_answer: "预言法警报（强调前景与管理、几乎不看价格）→强制转译为定量问题：价格与收益/资产/股利的测量关系余量多大、能否吸收不利变化——把气质兴奋换成算术"
V3_exclusivity:
  passed: true
  why_not_common: "'预言/保护'是格雷厄姆术语体系；把投资定义为工程（确保余量）而非预测（命中前景）——定位差异化"
cluster: 16
proposed_slug: protection-over-forecast
```

### u35
```yaml
id: u35
merged_ids: [f34, p48]
title: 精选无用推理链
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第9章：100 个分析员思想实验＋共识抵消机制（都同意更好→价格迅速抵消全部先前利益）（语境1）
    - 第10章：普通股基金长期跑输标普 500，且两种解释（市场有效/按前景选股不问价格）都不支持个人轻易战胜专家（证据层，语境2）
    - c28：便宜组 vs 昂贵组的 5 年成绩（对象3）
V2_predictive_power:
  passed: true
  novel_question: "订阅了五星分析师的精选组合，该期待什么？"
  derived_answer: "共识机制→期待应设为'平均结果'，精选溢价不可依赖；防御型应强调多样化而非纠缠个别选择——四原则界限内的自由选择'从坏处想是无害的'"
V3_exclusivity:
  passed: true
  why_not_common: "对'挑最好'的正面否定＋'界限内自由选择无害'的宽人严律组合——非常识的姿态配对"
cluster: 16
proposed_slug: protection-over-forecast
```

### u36
```yaml
id: u36
merged_ids: [f40, p56]
title: 技巧中和定律
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第12章：论断（大量聪明人竞争使技术智力相互中和，信息充分的结论反而不如抛硬币）（语境1）
    - 卷首/x14：股市预测不如掷硬币（语境2）
    - 第10章：基金集体跑输指数——中和的机构级证据（语境3）
V2_predictive_power:
  passed: true
  novel_question: "我比一般散户信息更快，能赢吗？"
  derived_answer: "中和定律：对手是同等聪明且设备更好的群体，信息优势被抵消→唯一出路是把着眼点放在价格与潜在/核心价值的关系上，而非市场正做什么——'优势幻觉'的结构性检验"
V3_exclusivity:
  passed: true
  why_not_common: "把'聪明人难赢'归因于竞争结构（相互中和）而非市场随机——认识论差异化；'较少注意市场时反而获利'的反常识推论"
cluster: 16
proposed_slug: protection-over-forecast
```

## Cluster 17 — stock-diagnosis-techniques（个股诊断技术）

### u37
```yaml
id: u37
merged_ids: [f37]
title: 报表还原分析技术
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第11章：六案例四件套——联属收益并回（北太平洋 3.80→7.15）/表外资产还原（AHS 每股加约 14 美元）/跨国可比对标（荷兰王牌石油 vs 新泽西标准石油）/同一债务人证券形式套利（TH 债券）（多对象）
    - 第8章：非经常项目九类分离清单——还原技术的初级版（不同章节，语境2）
V2_predictive_power:
  passed: true
  novel_question: "公司账面 EPS 与现金流长期背离，怎么还原真实盈利？"
  derived_answer: "还原路径：非经常项目分离→联属未分配收益并回→表外资产与债权还原→可比公司对标——具体手法受 1964 会计制度约束（时效警示），但'复杂性掩盖真相＝价值机会来源'的问题结构永存"
V3_exclusivity:
  passed: true
  why_not_common: "'有效分析的任务是解开复杂因素'＋把会计复杂性识别为机会来源——反向利用，差异化"
cluster: 17
proposed_slug: stock-diagnosis-techniques
```

### u38
```yaml
id: u38
merged_ids: [f41]
title: 股价-收益四模式诊断
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第12章：四模式（稳定收益剧摆 Kress / 同步放大 GM / 极端兴衰布鲁斯威克、棉花带、银行家证券 / 成长股行为 3M、可口可乐 vs IBM 1:19）——多对象多结局
    - c40–c51 案例群跨模式交叉（语境2）
V2_predictive_power:
  passed: true
  novel_question: "我的持仓价格波动比收益波动大得多，正常吗？"
  derived_answer: "模式一诊断：内部价值稳定时牛市价常为熊市价的 2–3 倍，波动主要起因于心理变化→按模式一应对（复核计算后无视）而非恐慌——先归类再定反应"
V3_exclusivity:
  passed: true
  why_not_common: "给投资者'价格行为地图'的类型学——把'它为什么这么波动'变成可归类、可预置反应的问题——差异化框架"
cluster: 17
proposed_slug: stock-diagnosis-techniques
```

### u39
```yaml
id: u39
merged_ids: [p55]
title: 高增长公司财务预警清单
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第12章：布鲁斯威克 7 年涨 87 倍后 -87%——三查来源（降价扩张压力/巨额短长期外债/未收现挂账利润）（语境1）
    - 第12章：模式 3 群像（棉花带、Reo 等）——同一清单的历史复用（对象2）
V2_predictive_power:
  passed: true
  novel_question: "收入翻倍但应收账款也翻倍的高增长公司怎么查？"
  derived_answer: "三查逐项对照：降价换增长的结构性压力→巨额外债→利润挂在未收现账户——命中任一即预警；格言化：'几乎所有飞向理想高空的企业都以摔回地上为代价'"
V3_exclusivity:
  passed: true
  why_not_common: "把警句变成三条可核查的资产负债表/利润表交叉项——清单化差异化"
cluster: 17
proposed_slug: stock-diagnosis-techniques
```

## Cluster 18 — margin-of-safety-core（安全边际核心）

### u40
```yaml
id: u40
merged_ids: [f48, p66, p67]
title: 安全边际量化器（三领域）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第16章：三领域算法（债券覆盖/价值缓冲；普通股期望盈利能力大大高于债券利率，9% vs 4% 经典算例；议价证券≤2/3 评价价值）（语境1）
    - 第8章：覆盖倍数标准为其债券臂提供参数（语境2）
    - 第16章：1964 年现实自检——10 年超额仅约 1/5 不足，知名普通股也有真正风险（反面应用，语境3）
V2_predictive_power:
  passed: true
  novel_question: "国债 4.5% 的今天，股票多少预期回报才值得买？"
  derived_answer: "期望盈利能力须大大高于债券利率，10 年超额≥所付价格 50% 为佳→把'值不值得买'变成可计算门槛（参数按当期利率重查——通用时效警示）；答不出即投机"
V3_exclusivity:
  passed: true
  why_not_common: "把'安全'从感觉变成三领域算法＋'主要风险是高出市场水平集中购买或买非代表性普通股'的定位——格雷厄姆核心术语的行为化"
cluster: 18
proposed_slug: margin-of-safety-core
```

### u41
```yaml
id: u41
merged_ids: [f49, p69]
title: 保险同构多样化原理
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第16章：保险同构＋轮盘赌演示（31:1 负边际越多样越亏；35:1 正边际每轮确定赢 2 美元）（语境1）
    - 第9章：集合预测→多样化是逻辑必然（语境2）
    - 第7章：特别情况须成批操作（同一逻辑的场景化，语境3）
V2_predictive_power:
  passed: true
  novel_question: "只有 5 只不同行业的股票算分散吗？"
  derived_answer: "同构检验两问：各笔结果是否相互独立＋是否存在正边际→无正边际时多样化放大失败；有正边际时 20 种或更多才使'利润总和超过损失总和'接近确定——推出'先边际后数量'的顺序"
V3_exclusivity:
  passed: true
  why_not_common: "多样化不是美德只是放大器（方向由边际决定）——反'越分散越安全'的直觉；保险与轮盘的同构论证非常识"
cluster: 18
proposed_slug: margin-of-safety-core
```

### u42
```yaml
id: u42
merged_ids: [f50, p70, p65]
title: 安全边际试金石（可证明性判据）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第16章：试金石——真正的投资必须有真正的安全边际，且可由数据、有说服力的推理和实际经验证明（语境1）
    - 第1章：投资三判据的最终回扣（不同章节的定义闭环，语境2）
    - 第16章/c60：20 年代不动产债券跌去 90% 后成投资——试金石的泛化演示（对象3）
V2_predictive_power:
  passed: true
  novel_question: "我'感觉'这只票跌到位了，算投资吗？"
  derived_answer: "可证明性检验：感觉、自信、时机判断全部出局——只接受'基于统计数据的简单和确定的算术推理'；推出'写出边际由什么数据证明'作为操作前置"
V3_exclusivity:
  passed: true
  why_not_common: "分界线是可证明性而非自信程度——把哲学判据做成审计问题；'四个字座右铭'是作者本人对全书收束的自我命名"
cluster: 18
proposed_slug: margin-of-safety-core
```

### u43
```yaml
id: u43
merged_ids: [f44, p57]
title: 换股内在价值等价检验
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第13章：道指成分替换回测——实际历史 vs 从未换股清单 vs 标普工业指数，按流行度替换无净收益（语境1）
    - 第9章：实现方式（基本群体中找低市盈率/第二层次群体买廉价股）（语境2）
    - c53/x24：换股回测案例群（对象3）
V2_predictive_power:
  passed: true
  novel_question: "把持仓 A 换成'更好'的 B，什么条件下值得？"
  derived_answer: "唯一原则：买进的每一美元须显示比卖出的每一美元更高的内在价值→'质量升级''热门度'本身不构成理由；不做分析每种买一点也能取得同样结果——换股Default 是不换"
V3_exclusivity:
  passed: true
  why_not_common: "'提质换股无益'的反直觉回测＋唯一例外判据——非常识"
cluster: 18
proposed_slug: margin-of-safety-core
```

### u44
```yaml
id: u44
merged_ids: [p58]
title: 质量通过价值获得
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第13章：断言＋分割股涨太快后未来机会更差的回测证据（语境1）
    - 第16章：充分低价格改造劣质证券（同构逻辑，语境2）
    - 第5章：优先股只在廉价时买（语境3）
V2_predictive_power:
  passed: true
  novel_question: "宁买好公司贵一点，对吗？"
  derived_answer: "'如果价值是丰富的，质量或许注定是充分的'→在同等的质量愿望下价格维度优先；'任何正确的概括必须始终将价格考虑进去'——给出可操作的优先级反转"
V3_exclusivity:
  passed: true
  why_not_common: "直接对抗'质量优先'信条（后来巴菲特一脉的修正方向正是从此出发）——历史性差异化立场"
cluster: 18
proposed_slug: margin-of-safety-core
```

### u45
```yaml
id: u45
merged_ids: [p71]
title: 充分低价格改造劣质证券
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第16章：泛化规则＋20 年代不动产债券按面值推销到跌 90% 后反而安全（语境1）
    - 第6章：二等债 2/3 折扣线（同构，语境2）
    - 第5章：廉价优先股二元规则（语境3）
V2_predictive_power:
  passed: true
  novel_question: "垃圾债跌到 4 折，是机会吗？"
  derived_answer: "泛化检验三条件：顺差是否实质＋购买者是否情报/经验/多样化齐备＋公司前程是否并非真无望→三者缺一不可，'前程确实无望时无论多低都应避开'——书外可直接套用"
V3_exclusivity:
  passed: true
  why_not_common: "投资属性由价格-价值关系决定而非证券类别——对抗 1914 年前'与证券类型挂钩的永恒准则'式教条，反直觉"
cluster: 18
proposed_slug: margin-of-safety-core
```

## Cluster 19 — shareholder-governance（股东治理质询）

### u46
```yaml
id: u46
merged_ids: [f05, p06]
title: 所有者思维模型
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第1章："投资者整体是主人非交易商，通过企业而非从同伴赚钱"（语境1）
    - 第14章：管理低效三信号/公平回购/接管正当性——治理框架的展开（语境2）
    - 第15章：股利政策举证——所有者权利的另一战场（语境3）
V2_predictive_power:
  passed: true
  novel_question: "公司大量现金趴账不分红不回购，我能做什么？"
  derived_answer: "所有者路径：三信号核查→股东大会质询→金融效率主张（股东资产按其最大利益运作）——而非'不喜欢就卖'；'卖掉只改变所有权归属不改善经营'"
V3_exclusivity:
  passed: true
  why_not_common: "'如果你不喜欢管理，那就卖掉'被斥为愚昧有害——直接反华尔街主流；收益来自企业而非同伴钱包的结构性视角差异化"
cluster: 19
proposed_slug: shareholder-governance
```

### u47
```yaml
id: u47
merged_ids: [f45, p61]
title: 管理低效三信号与不充分市价判据
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第14章：三信号（繁荣期回报不满意/销售利润率低于同业/EPS 增长低于工业平均）＋四个指数即可检验（语境1）
    - 第14章/c56：菲利浦·莫里斯 1938–47 销售增长 170% 掩盖相对效率滑落（对象2）
    - 第14章："不充分的市场价格"（市价远低于账面值或市价/账面比率远低于行业平均）——市场面对园的投票（语境3）
V2_predictive_power:
  passed: true
  novel_question: "公司营收创新高，该满意管理层吗？"
  derived_answer: "销售指标被薪金结构扭曲→改查三个相对数（繁荣期股东回报/相对行业利润率/EPS 相对工业平均）＋市价判据——'管理好不好'从印象变成四个指数的相对比较"
V3_exclusivity:
  passed: true
  why_not_common: "把治理判断量化为相对数清单＋销售增长陷阱的显式警告——差异化"
cluster: 19
proposed_slug: shareholder-governance
```

### u48
```yaml
id: u48
merged_ids: [f46, p62]
title: 内外股东利益背离与公平回购
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第14章：结构性诊断（外部股东收回投资的唯一具体方式是分红与市价，内部人不依赖二者）＋经营效率≠金融效率（语境1）
    - 第14章/c57/c58：Mission 持股公司折扣困境与 FWO 董事会阻击收购（对象2）
    - 第14章：公平回购规则——公平价高于市价时必须竞争性招标（AHS 约 20% 资产被低价收回的反面）（语境3）
V2_predictive_power:
  passed: true
  novel_question: "公司以市价八折向大股东关联方回购，怎么办？"
  derived_answer: "金融效率判据：公司必须公平对待所有股东＋公平价高于市价时以竞争性招标进行→股东可主张的量化标准，而非道德抱怨"
V3_exclusivity:
  passed: true
  why_not_common: "'管理层天然想多拿资本'的结构假设＋内外股东利益背离作为股利/回购/治理问题的统一根源——结构性诊断非常识"
cluster: 19
proposed_slug: shareholder-governance
```

### u49
```yaml
id: u49
merged_ids: [p63]
title: 接管报价正当性
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 第14章：FWO 案例——董事会以"捍卫交易所价格"阻击 55 美元报价被判为无权（对象1）
    - 第14章：Mission 合并受阻——同一主题的第二案例（对象2）
V2_predictive_power:
  passed: true
  novel_question: "敌意收购＝掠夺吗？"
  derived_answer: "反主流：高于市价的报价是外部股东从董事会不公正待遇中解脱的唯一方法；没有被强迫卖出者，保留者反而受益；董事会想不被取代的正道是把公司处理好、防止股票低于真实价出售"
V3_exclusivity:
  passed: true
  why_not_common: "为'敌意收购'正名的罕见立场——历史性差异化（V3 borderline：结论绑定 1964 年制度环境，逻辑层保留）"
cluster: 19
proposed_slug: shareholder-governance
```

### u50
```yaml
id: u50
merged_ids: [f47, p64]
title: 股利政策举证二分法
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第15章：二选一规则（正常派息约 2/3 或证明低分配未压低市价）（语境1）
    - 第15章：1 美元股利对市价的拉动约为 1 美元未分配利润的 4 倍——实证基础（语境2）
    - 第15章：股票红利正名（再投资收益的有形凭证，通常 ≤5%，NYSE 以 25% 为界）——股利工具辨析（对象3）
V2_predictive_power:
  passed: true
  novel_question: "成长型公司零分红，合理吗？"
  derived_answer: "举证规则：要么正常派息，要么证明低分配未压价（公认成长公司通常能做到，其他情况下低股利是市价低于价值的原因）→'管理者最知情'不是免检理由——把风格之争变成举证责任分配"
V3_exclusivity:
  passed: true
  why_not_common: "把股利从'偏好之争'重构为举证责任；股票红利与拆分的概念辨析（拆分与特定再投资收益无关）——术语体系差异化；税收替代方案属 1964 税制（时效警示）"
cluster: 19
proposed_slug: shareholder-governance
```

## Cluster 20 — investment-advice-discipline（投资建议使用纪律）

### u51
```yaml
id: u51
merged_ids: [f15, f16, p20, p21, p22]
title: 投资建议使用纪律（双条件＋提问重构）
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 第4章：多对象（投资银行卖方/经纪行劝告/金融服务机构/亲朋好友非专业建议）——同一纪律的四个对象
    - 第6章：新证券推销术＝卖方偏见的极端例证（不同章节，语境2）
    - x10：华尔街劝告的结构性失灵（反例佐证，对象5）
V2_predictive_power:
  passed: true
  novel_question: "大 V 荐股/智能投顾推荐，怎么用？"
  derived_answer: "双条件：要么把行动严格限制在标准保守的投资形式上，要么与顾问有极其亲密的关系或相当了解；否则建议只用来增长知识、形成独立见解；提问重构——问安全性/吸引力/内在价值，不问'下几个月涨不涨'，并一开始声明自己对'小费'毫无兴趣"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'别全信'；格雷厄姆给出'限定行动空间 vs 深度了解顾问'的双条件结构＋'问题质量决定建议质量'的交互模型——操作化差异化"
cluster: 20
proposed_slug: investment-advice-discipline
```

---

# 聚类总表（20 个 skill → 阶段 2 构造清单）

| # | cluster / proposed_slug | 包含候选 id（单元） | 覆盖内容 | A1 素材案例 id | 反例 id | 术语 id |
|---|---|---|---|---|---|---|
| 1 | invest-vs-speculation-filter | u01 [f02,p01,p02]、u02 [f51,p72,p73] | 投资/投机三判据、三非理性、专款隔离；四大商业原理自检、抱负限定 | c04 | x01 | t01, t02 |
| 2 | rule-reliability-trend-skepticism | u03 [f01,p07]、u04 [f10]、u05 [f43,p59] | 准则寿命分类检验、策略更新/自我撤回；流行即失效；趋势逆转 2:1 与回报趋同 | c01, c08, c09, c10, c12, c54, c55 | x06, x07, x15, x23 | t11 |
| 3 | market-mr-volatility-discipline | u06 [f06,f07,p08,p11,p12,p13]、u07 [f08,p09]、u08 [f09,p10]、u09 [f21,p24] | 市场先生人格化、波动二义、下跌检视阈值、剧涨莫买暴跌莫卖、不以个股信号操作；浮盈不可兑现；时机/价格之路；风险三来源重定义 | c05, c06, c07 | x09, x26 | t07, t08, t09, t12 |
| 4 | mechanical-allocation-dca | u10 [f18,p04,p25]、u11 [f19,p27]、u12 [p14] | 25–75 带、50:50±5%→1/11 再平衡、极值使用举证；DCA 与危险水平状态管理；有资金即买入 | c16 | — | t05, t06 |
| 5 | investor-identity-matching | u13 [f17,p23,p42,p03] | 防御/进攻二分、无中间立场、回报与明智努力相称、进攻型第一原则 | — | x29 | t03, t04 |
| 6 | overheated-market-defense | u14 [f13,p16,p17]、u15 [f11,p15,p18,p34] | 不确定性优先、谨慎三准则、DCA 暂停规则；牛市五特征/六条件打分、新股倒挂信号、量级核对纪律 | c11, c13, c22 | x03, x04 | t10 |
| 7 | defensive-stock-selection | u16 [f20,p26,f42,p60]、u17 [f33,p46] | 四原则＋量化锚定、大而强的随机对照证据；全取样/排除法/低倍数法、板块区别意见 | c28, c52 | — | t13 |
| 8 | bond-safety-terms | u18 [f29,p43]、u19 [p28] | 覆盖倍数双标准（平均/最差年）、优先股双倍股利口径、辅助指标；可赎回条款规避 | c14, c15 | x12 | t21 |
| 9 | aggressive-negative-list | u20 [f22,p29,p30,p31,p32]、u21 [f23,p33,p35] | 负面清单四不碰、收益换本金检验、2/3 折扣线；新证券双重怀疑、可转债公理 | c18, c19, c20, c21, c22 | x04, x05, x11, x13 | t15, t16, t17 |
| 10 | excess-return-path-selection | u22 [f04,p05]、u23 [f03,f24,p37] | 差异化公理与双刃；五路排除、双倍价值、三域选择、按气质取舍 | c03, c32 | x20 | — |
| 11 | neglected-large-cap-strategy | u24 [f25,p38] | 冷门大公司低倍数法、6–10 种/1–5 年、大小公司边界论证 | c03, c23 | — | — |
| 12 | bargain-issues-net-nets | u25 [f26,p39]、u26 [f27,p40,p52,p53]、u27 [f38,p54] | 廉价定义与双法、低估两来源；净流动资产折扣、四条筛选、+50% 加成；大起大落收益来源与幸存者偏差自警 | c24, c25, c29, c31, c45, c46 | x30 | t18, t19 |
| 13 | special-situations-arbitrage | u28 [f28,p41] | 特别情况预计算、时间风险定价、偏见反用、门槛自限 | c26, c35, c39 | — | t20 |
| 14 | earnings-power-valuation | u29 [f30]、u30 [f39,p68]、u31 [f36,p49,p51] | 资本化率五因素；盈利能力跨周期定义、繁荣≠安全；评估规则组、1/3 线、投机成分分解 | c27, c30 | x16 | t22, t23, t24, t26 |
| 15 | growth-stock-appraisal | u32 [f35,p50,p36] | 8.5+2g 正算/反解、利率校准警告、20 倍参与上限、基金实证反面 | c17, c32 | x02 | t14 |
| 16 | protection-over-forecast | u33 [f31,p44]、u34 [f32,p47,p45]、u35 [f34,p48]、u36 [f40,p56] | 数学化反比；预言/保护二分、集合预测；精选无用推理链；技巧中和 | c02, c27, c28 | x14, x20, x27 | t25, t27 |
| 17 | stock-diagnosis-techniques | u37 [f37]、u38 [f41]、u39 [p55] | 报表还原四件套（参数过时警示）；股价-收益四模式地图；高增长三查预警 | c34, c36, c37, c38, c40, c41, c43, c45, c48, c50 | x21, x22 | — |
| 18 | margin-of-safety-core | u40 [f48,p66,p67]、u41 [f49,p69]、u42 [f50,p70,p65]、u43 [f44,p57]、u44 [p58]、u45 [p71] | 三领域边际量化、保险同构多样化、试金石可证明性、换股等价检验、质量通过价值、低价格改造论 | c53, c60 | x24, x25 | t27, t28 |
| 19 | shareholder-governance | u46 [f05,p06]、u47 [f45,p61]、u48 [f46,p62]、u49 [p63]、u50 [f47,p64] | 所有者思维、三信号＋不充分市价、内外股东背离与公平回购、接管正当性、股利举证二分、股票红利辨析 | c56, c57, c58, c59 | x17, x18, x19, x28 | t29, t30 |
| 20 | investment-advice-discipline | u51 [f15,f16,p20,p21,p22] | 顾问依赖双条件、卖方怀疑、小费免疫、提问重构 | — | x10 | — |

素材池使用说明：t27（多样化）主锚在 C18（保险同构），C16（集合预测→多样化逻辑）共用；c22 同时服务 C6（新股狂潮标本）与 C9（新证券怀疑）；c45/c46 同时服务 C12（大起大落）与 C17（模式 3 群像）；c27 服务 C14（评估示范）与 C16（保护法演示）。

---

# 降级素材注（未通过候选的去向）

| id | 标题 | 挂在 | 处置 |
|---|---|---|---|
| f12 | 市场水平评估框架（股债信号+多方法对照） | V1（第 3 章单一语境）＋第三章行情回顾类规则 | 装置整体淘汰；"多方法对照+量级核对"判断逻辑由 u15（C6）承接，"信号多年不验证即弃用"由 u03（C2）承接；c12/c13/x15 继续作 C2/C6 素材 |
| f14 | 三层认知过滤（事实/可能性/不可能性） | V1（仅一次出现）＋V3（通用认识论常识） | 不并入；可作 C6（overheated-market-defense）引言层金句素材 |
| p19 | 股息率低于债息是危险水平线索（附失效警告） | V1（信号有效性证据限于第 3 章）＋第三章行情信号类规则 | 信号本身作为 u15（C6）清单第 3 条保留；"7 年验证"元规则并入 u03（C2）；c13/c12/x15 作素材 |

另注（去重而非淘汰）：被并入其他单元的 70 条候选不写 rejected 文件，其去重账目见下节；阶段 2 构造各 skill 时应以合并单元为内容源。

---

# 去重合并账（70 条 → 承接单元）

- p01, p02 → u01（f02：三判据＋三非理性同属一个筛选器）
- p72, p73 → u02（f51：四原理的收束句即 p73 抱负限定）
- p07 → u03（f01：幸存准则与准则寿命判别同源）
- f07, p08, p11, p12, p13 → u06（f06：市场先生应对纪律的五个切面）
- p09 → u07（f08：浮盈不可兑现律双池同提取）
- p10 → u08（f09：时机/价格二分双池同提取）
- p24 → u09（f21：风险重定义双池同提取）
- p04, p25 → u10（f18：比例带 ch1 立规与 ch5 程序合一）
- p27 → u11（f19：DCA 双池同提取）
- p23, p42, p03 → u13（f17：努力相称律、无中间立场、进攻型第一原则同为身份二分的组成判据）
- p16, p17 → u14（f13：谨慎三准则与不确定性优先同段互证）
- p15, p18, p34 → u15（f11：五特征、六条件、新股倒挂同为顶部信号清单的层级）
- p26, f42, p60 → u16（f20：四原则的 ch5 规则、ch13 对照证据、大而强规则合一）
- p46 → u17（f33：三路径双池同提取）
- p43 → u18（f29：覆盖倍数双池同提取）
- p29, p30, p31, p32 → u20（f22：负面清单的 ch5/ch6 多章节同方法论）
- p33, p35 → u21（f23：新证券与可转债怀疑同章同框架）
- p05 → u22（f04：差异化公理双池同提取）
- f24, p37 → u23（f03：五路排除与三域选择同属路径选择框架）
- p38 → u24（f25：冷门大公司双池同提取）
- p39 → u25（f26：廉价证券定义与双法双池同提取）
- p40, p52, p53 → u26（f27：净流动资产折扣、+50% 加成、四条筛选同为 net-net 技术组）
- p54 → u27（f38：大起大落收益来源双池同提取）
- p41 → u28（f28：特别情况反用双池同提取）
- p68 → u30（f39：盈利能力定义的行为推论同段互证）
- p49, p51 → u31（f36：评估规则组与投机成分分解同属 ch10 规则组）
- p50, p36 → u32（f35：8.5+2g 与参与上限、基金实证同属成长股评估）
- p44 → u33（f31：数学化反比双池同提取）
- p47, p45 → u34（f32：预言/保护二分与其集合预测底座）
- p48 → u35（f34：精选无用推理链双池同提取）
- p56 → u36（f40：技巧中和与"着眼价格-核心价值"同段互证）
- p66, p67 → u40（f48：债券两算法与普通股算例同为三领域量化器组成）
- p69 → u41（f49：保险同构双池同提取）
- p70, p65 → u42（f50：试金石与"四个字座右铭"同章同判据）
- p57 → u43（f44：换股等价检验双池同提取）
- p06 → u46（f05：所有者思维双池同提取）
- p61 → u47（f45：三信号双池同提取）
- p62 → u48（f46：公平回购规则已含于内外股东背离框架的操作要求）
- p64 → u50（f47：股利举证二分双池同提取）
- f16, p20, p21, p22 → u51（f15：顾问双条件、提问重构、小费免疫同属"使用建议"方法论）

---

*阶段 1.5 完成于 2026-10-06。下一阶段：阶段 2 按 20 个 cluster 构造 SKILL.md（进入 skills/），每个 skill 头部写入通用时效警示，数字参数标注"1964 年快照，按当期重查"。*
