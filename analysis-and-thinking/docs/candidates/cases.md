# candidates/cases.md — 《分析与思考》阶段 1 案例提取

> 引文与关键数字经与 full.txt 定点核对。宁多勿漏，待阶段 1.5 验证。

```yaml
- id: c01
  title: 宝能杠杆放大链
  type: case
  source_chapter: 第1讲
  source_quote: |
    宝能：70亿万能险经通道嵌套+存一贷二+融资融券放大至450多亿购万科25%——六种杠杆工具全用上的典型。
  summary: |
    事实：70 亿万能险资金经六种杠杆工具层层放大至 450 多亿收购万科股份。
    论证：六工具组合的放大威力与穿透式监管的必要性。
    迁移：解剖任何"小钱撬大钱"结构的模板。
  bound_to: ["金融乱象六工具识别"]
  tags: [leverage, case-study]

- id: c02
  title: 蚂蚁 ABS 循环 40 次
  type: case
  source_chapter: 第1讲
  source_quote: |
    蚂蚁：30多亿资本金循环发ABS 40次形成3600多亿放贷、上百倍杠杆——个案协商出新规则（资本金增至300亿、循环4次、总杠杆约10倍）。
  summary: |
    事实：30 多亿资本金循环发 ABS 40 次放贷 3600 亿，监管后协商出新规则。
    论证：ABS 循环次数是杠杆的隐形放大器。
    迁移：ABS/资产滚动产品的杠杆审计方法。
  bound_to: ["数字信贷五原则", "ABS循环纪律"]
  tags: [fintech, abs]

- id: c03
  title: 重庆京东方资本招商
  type: case
  source_chapter: 第2讲
  source_quote: |
    重庆京东方定增210亿+银行118亿，16个月投产，政府股票收益超200亿——政府与市场双赢的资本招商范式。
  summary: |
    事实：重庆以 210 亿定增入股+撬动 118 亿银行贷款，16 个月建成投产，政府股票收益超 200 亿。
    论证：资本招商（入股共享成长）优于补贴招商（白给）。
    迁移：产业项目落地方案设计。
  bound_to: ["资本招商范式"]
  tags: [investment, local-government]

- id: c04
  title: 2000 年债转股重组回收率
  type: case
  source_chapter: 第1讲
  source_quote: |
    2000年1.3万亿债转股，银行核销60%—70%后AMC回收60%—70%债权，实际坏账约40%——重组法可行性。
  summary: |
    事实：1.3 万亿不良中真实坏账约 40%，重组后有回收。
    论证：收购重组豁免是去杠杆可行动作而非市场崩溃。
    迁移：不良资产处置的预期回收率锚点。
  bound_to: ["宏观杠杆四指标与结构分解"]
  tags: [npl, deleverage]

- id: c05
  title: 500 美元笔记本拆账
  type: case
  source_chapter: 第12讲
  source_quote: |
    一台销售价500美元的笔记本电脑：原材料零部件250+美国研发品牌110+物流销售80+中国代工60——区区12%的代工附加收入。
  summary: |
    事实：笔记本价值链拆账，中国代工仅得 12%；中国对美出口 60% 是美企在华返销。
    论证：贸易顺差的价值分配与账面顺差严重错位。
    迁移：一切贸易失衡争议的利益分解工具。
  bound_to: ["贸易失衡的价值链拆账法"]
  tags: [trade, value-chain]

- id: c06
  title: 美国两次危机对冲史
  type: case
  source_chapter: 第13讲
  source_quote: |
    2001年股市183%崩盘靠房地产对冲→2007年房地产173%崩盘→靠政府举债QE对冲→下一站政府债务/美元信用。
  summary: |
    事实：美国 20 年危机后移链条的完整复盘（各泡沫峰值/GDP 数据齐全）。
    论证：对冲式救市只是转移泡沫位置。
    迁移：预测"下一场危机震中"的复盘模板。
  bound_to: ["危机后移链条", "宏观泡沫四指标"]
  tags: [crisis, us-economy]

- id: c07
  title: 外汇占款 83% 峰值
  type: case
  source_chapter: 第4讲
  source_quote: |
    外汇占款占央行资产：2013年末峰值83%，2019年7月59.35%——人民币近六成仍靠外汇发行。
  summary: |
    事实：央行资产负债表结构数据。
    论证："汇兑本位制"诊断的核心证据——货币发行的锚在外汇而非本国信用。
    迁移：货币制度诊断的资产负债表检查法。
  bound_to: ["货币锚与发行制度诊断"]
  tags: [currency, central-bank]

- id: c08
  title: 美国守纪律与失控两段
  type: case
  source_chapter: 第4讲
  source_quote: |
    美国1970-2007守纪律期：货币与GDP同步增长（12倍 vs 13倍）；2008后受MMT影响：基础货币增5倍 vs GDP增1.5倍。
  summary: |
    事实：美国两段货币发行对照。
    论证：主权信用货币可行但纪律是生死线——同一体制纪律在则稳、失则乱。
    迁移：评估任何央行放水可持续性的对照基线。
  bound_to: ["主权信用货币的刚性纪律"]
  tags: [monetary, us-economy]

- id: c09
  title: 惠普重庆结算拉锯
  type: case
  source_chapter: 第10讲
  source_quote: |
    惠普重庆建厂谈判：以15%所得税率＋离岸账户两条件拉结算——中国大陆1.8万亿美元加工贸易结算均在境外。
  summary: |
    事实：重庆用低税率+离岸账户把惠普结算拉到重庆；全国 1.8 万亿加工贸易结算仍在境外（新加坡 4000 亿、香港 3000 亿）。
    论证：结算枢纽即财富中心——三链框架中"价值链枢纽"的落地版。
    迁移：离岸结算中心建设、招商引资的结算维度。
  bound_to: ["三零原则与中间品贸易时代"]
  tags: [settlement, value-chain]

- id: c10
  title: 李嘉诚世纪雅园持有模式
  type: case
  source_chapter: 第9讲
  source_quote: |
    李嘉诚世纪雅园：2000年1万/㎡持有出租至2010年，8万/㎡售出——持有模式优于快销。
  summary: |
    事实：持有出租十年后售价 8 倍于成本价。
    论证：开发商从快销转向持有运营的价值。
    迁移：不动产经营模式选择、售租并举的论证。
  bound_to: ["住房负担六分之一标尺（售租结构）"]
  tags: [real-estate, business-model]

- id: c11
  title: 上海钻石交易所治走私
  type: case
  source_chapter: 附录
  source_quote: |
    全国钻石交易唯一通道+国际规则（零关税、增值税征17退13只收4%）：整个中国钻石市场走私基本消失，交易量2018年达26亿美元。
  summary: |
    事实：以唯一通道+与国际接轨的税则替代高关税管制，走私消失、交易所 20 年成世界最快。
    论证：规范渠道比堵截有效——"开正门、堵偏门"的制度设计。
    迁移：任何灰色市场治理的机制设计。
  bound_to: ["三零原则与中间品贸易时代"]
  tags: [institutional-design, market-governance]

- id: c12
  title: 浦东三管齐下筹资
  type: case
  source_chapter: 附录
  source_quote: |
    市政府只给每区3000万开办费：土地批租+三大公司股份制引入外资+1993年上市融资——到2000年三大公司实际投资七八百亿元。
  summary: |
    事实：3000 万开办费撬动百亿级开发、十年 5000 亿开发资金。
    论证：政策（而非拨款）是最大的启动资金——土地资本化+股权融资+证券市场的组合杠杆。
    迁移：开发区/新城开发融资方案。
  bound_to: ["资本招商范式"]
  tags: [urban-development, financing]

- id: c13
  title: 华为五大围剿与五大自保
  type: case
  source_chapter: 第12讲
  source_quote: |
    美国五大围剿（孟晚舟、实体清单、芯片断供、安卓停供、除名IEEE）vs 华为五大自保（5G基站、终端、六类芯片、鸿蒙、备胎）。
  summary: |
    事实：科技战攻防的完整清单对照。
    论证：备胎体系在断供时的实际价值。
    迁移：（与书架已有 war-game、self-reliance 配套）供应链攻防的攻守清单模板。
  bound_to: ["书架已有 self-reliance-boundary 的案例补充"]
  tags: [tech-war, supply-chain]

- id: c14
  title: 斯蒂格利茨怪圈
  type: case
  source_chapter: 第12讲
  source_quote: |
    发展中国家辛辛苦苦给发达国家打工，好不容易收入了美元，又将这些美元低利息借给发达国家，发达国家再投资回发展中国家赚取10%以上回报。
  summary: |
    事实：国际资本流动的双向利益结构。
    论证：购美债"操纵汇率"论的荒谬与储备货币体系的中性解释。
    迁移：理解外汇储备、本币国际化必要性的经典框架。
  bound_to: ["人民币国际化五个蓄水池"]
  tags: [forex, international-finance]

- id: c15
  title: 阿里巴巴 VIE 出走
  type: case
  source_chapter: 第7讲
  source_quote: |
    阿里巴巴因VIE被港拒之门外跑赴美国——制度不迁就企业的代价案例；散户持股市值占25%却贡献80%交易量。
  summary: |
    事实：港交所因 VIE 结构拒绝阿里，阿里赴美上市；中国股市散户市结构数据。
    论证：发行制度落后会把最优质资产赶去对手市场。
    迁移：制度竞争力分析、上市地选择。
  bound_to: ["资本市场三功能诊断"]
  tags: [capital-market, institution]

- id: c16
  title: 美国 5G 四大劣势
  type: case
  source_chapter: 第12讲
  source_quote: |
    5G通信设备商美国为零；中低频率波段被军方占用；4G基站仅40万个（中国370万）；肢解贝尔实验室后基础科研下降。
  summary: |
    事实：美国在 5G 竞争中结构性落后的四个原因。
    论证：领先者的路径依赖与结构性失误。
    迁移：技术代际竞争分析、基础设施先行价值的论证。
  bound_to: ["书架已有 war-game-scenario-analysis 的案例补充"]
  tags: [5g, tech-competition]
```
