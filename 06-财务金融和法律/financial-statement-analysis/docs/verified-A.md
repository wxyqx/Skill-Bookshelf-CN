# 三重验证通过池 A（framework + principle）

> 验证官执行 V1/V2/V3，119 条候选 → 通过 58 条（48.7%，目标区间 30-50%）。
> 跨文件去重：27 条实质重复项已并入下列各条 orig_ids，未计入淘汰。编号按主题聚簇排列，与 skill 打包方案对应。

```yaml
id: v-A01
title: 战略视角财务状况质量综合分析路径（总览五步/操作四步）
type: framework
orig_ids: [f03]
V1_cross_domain:
  passed: true
  evidence:
    - 第1章第4节:五步版首次亮牌（背景→股权→资产质量→利润现金→整体评价）
    - 第7章第2节:四步操作版系统重述，北陆药业案例全程按此演练
    - 第3-6章:各章工具（战略分类/核心利润/获现率/差量分析）均挂接其第③步，构成贯穿性骨架
V2_predictive_power:
  passed: true
  novel_question: "一家跨界并购了游戏公司的建材上市公司年报，只有一天时间，按什么顺序看、重点在哪？"
  derived_answer: "四步强制排序：先背景（并购战略表述+商誉规模）→看审计意见是否非标（替代会计分析）→战略视角发现并购后属投资主导型，转母公司报表查控制性投资扩张效果→前景按投资线（子公司盈利与分红）而非经营线预测。书中未讨论跨界并购，路径仍能输出完整的优先级与检查清单。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是'看报表算比率'；本路径明确规定'会计分析不单独做、以审计意见整体替代''前景预测按资产功能分三线''以母公司报表为起点'——这些程序性设计是作者体系特有。"
```

```yaml
id: v-A02
title: 战略与竞争力分析八步法（资产负债表的战略解读总装程序）
type: framework
orig_ids: [f56]
V1_cross_domain:
  passed: true
  evidence:
    - 第7章第2节:八步清单系统陈述
    - 第3章:其构件（战略三分类/四大动力/资产金融性负债率）各自独立成型
    - 第6章:第⑧步母公司与合并对照即差量分析法在八步中的落位
V2_predictive_power:
  passed: true
  novel_question: "某上市公司母公司报表其他应收款80亿、合并报表仅10亿，母公司资产300亿、合并500亿，八步法给出什么诊断路径？"
  derived_answer: "第①步四大动力归因看资产增量来源→第⑧步差量识别：其他应收款'越合并越小'差额62亿是对子公司资金输送，资产差200亿=控制性投资撬动的子公司资产，随后转入扩张效果与四大动力归因——八步法直接给出诊断顺序而非孤立读数。"
V3_exclusivity:
  passed: true
  why_not_common: "'分析资产负债表'是常识，但'必须从母公司报表开始而非合并报表''第一步先做四大动力归因''负债融资潜力用资产金融性负债率衡量'是作者的总装程序。"
```

```yaml
id: v-A03
title: 企业发展前景预测三路径（经营线/投资线/重组并购线）
type: framework
orig_ids: [f57]
V1_cross_domain:
  passed: true
  evidence:
    - 第7章第2节:三路径系统陈述
    - 第3-4章:分线依据（经营性/投资性资产重分类）在第3章成型、第4章用于利润结构
    - 第4/6章:"母公司控制性投资就是子公司经营性资产"两次独立表述，支撑投资线方法
V2_predictive_power:
  passed: true
  novel_question: "一家持有多家盈利子公司股权的控股平台，母公司利润表连年微亏，前景怎么预测？"
  derived_answer: "不能按经营线判死——成本法下母公司业绩只反映子公司分红政策；应按投资线考察子公司核心利润与经营现金流（借合并报表比照经营线方法），再按分红政策折算母公司真实回流量。"
V3_exclusivity:
  passed: true
  why_not_common: "常识预测看收入利润趋势外推；作者的'按资产功能分线+重组并购线专业化/多元化权衡'是独特分类，且明确各线检查变量。"
```

```yaml
id: v-A04
title: 项目质量分析法（本书招牌方法）
type: framework
orig_ids: [f04]
V1_cross_domain:
  passed: true
  evidence:
    - 第1章第3节:方法定义与"重大/异动项目"切入原则
    - 第2章:明确"只有对重大项目和异动项目用附注解读才能个性化"
    - 第3-7章:货币资金到商誉逐项展开，北陆案例全程应用
V2_predictive_power:
  passed: true
  novel_question: "某公司固定资产原值几乎没变，但折旧费用率明显下降，查什么？"
  derived_answer: "按例外原则锁定折旧政策异动→附注查折旧年限/方法变更（作者列名的操纵点之一），并核对其对利润的贡献是否构成'非经营性变化'。统一比率体系不会触发这个检查。"
V3_exclusivity:
  passed: true
  why_not_common: "比率体系是通用工具；'为每个企业量身定做个性化分析方案、重大异动项目+附注+操纵手法配对'在方法论上与统一指标体系对立，是作者招牌。"
```

```yaml
id: v-A05
title: 资产质量三维分析框架（盈利性/周转性/保值性）
type: framework
orig_ids: [f09]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:三性总纲定义
    - 第3章各节:货币资金/应收/存货/固定资产/长投逐项框架均为三性具体化
    - 第7章:综合分析中"不良资产区域"是保值性的落地应用
V2_predictive_power:
  passed: true
  novel_question: "某企业一条产线账面净值5亿，对应产品毛利率连年为负——三性哪个维度报警，推出什么？"
  derived_answer: "盈利性报警：资产实际效用低于预期；连带保值性存疑（减值风险），且非流动资产减值不得转回，未来计提将直接冲击利润——从单一项目推出利润表后果。"
V3_exclusivity:
  passed: true
  why_not_common: "常识看资产'值多少钱'；三性把质量操作化为情境化三维标尺（同一资产在不同企业预期效用不同），保值性以'减值可能性'而非市价为判据——作者体系术语。"
```

```yaml
id: v-A06
title: 审计意见判读框架与异常信号（会计分析的替代入口）
type: framework
orig_ids: [f06, pr40]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章第1节:五类型严重度排序与判读
    - 第7章第2节:"以审计意见类型与措辞整体判断会计质量、不再单独做会计分析"的方法化应用
    - 第4章:非标意见/报告异常长/频繁换所/披露晚列为利润质量恶化信号
V2_predictive_power:
  passed: true
  novel_question: "审计报告为标准无保留意见但带强调事项段（持续经营重大不确定性），这批债券能买吗？"
  derived_answer: "强调事项段类型直接指向偿债疑虑，叠加'频繁换所、年报披露晚、报告异常长'等信号交叉验证即可低成本初筛出局，不必逐项会计分析——框架给出的是初筛程序而非担保。"
V3_exclusivity:
  passed: true
  why_not_common: "五类型名称是审计常识，但'用意见类型+措辞替代整个会计分析'及'报告长度/换所/披露日期都是信号'的廉价初筛方法论是作者的用法。"
```

```yaml
id: v-A07
title: 货币资金三维质量分析（运用/构成/生成）
type: framework
orig_ids: [f11]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:三维框架定义（三种持有动机、四因素规模判断）
    - 第5章:受限资金与"自由度"口径呼应构成质量
    - 第7章:闲置现金恶化总资产类比率呼应运用质量；茅台/格力为生成质量正例
V2_predictive_power:
  passed: true
  novel_question: "某公司货币资金占总资产45%，同时短期借款30亿——三维框架给什么判断？"
  derived_answer: "运用质量报警（过大现金=生财无道或资金受限）；构成质量查受限比例（保证金/质押/司法冻结）；生成质量查经营性流入占比——'存贷双高'三解释（保证金、多子公司分散、融资环境）逐项排除，而非一见双高就喊造假。"
V3_exclusivity:
  passed: true
  why_not_common: "'现金越多越安全'是常识；作者的'过大即问题+三渠道生成质量（造血功能）+受限自由度'是反向判据体系。"
```

```yaml
id: v-A08
title: 核心利润含金量检验程序（与经营现金流比较+差异五类归因）
type: framework
orig_ids: [f32, pr42]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第4节:比较程序与五类原因排查首次提出
    - 第5章:正式化为核心利润获现率（经验底线>1，1.2~1.5倍充足）
    - 第7章:北陆案例沿用；第5章乐视案例为反面应用
V2_predictive_power:
  passed: true
  novel_question: "某制造企业核心利润3亿、经营现金净流量0.5亿，且当期原材料存货大增——缺口怎么归因？"
  derived_answer: "五类归因逐项排查后落在'付款不正常增加'，但作者要求区别对待：囤料属战略性付款，会提升未来含金量——同一缺口可得'恶化'与'备战'两种相反结论，判据在付款的性质而非金额。"
V3_exclusivity:
  passed: true
  why_not_common: "'利润要看现金含量'近常识，但'用核心利润而非净利润做分母''1.2~1.5倍经验线''缺口必须五类归因且区分战略性付款'是作者的可操作检验程序。"
boundary_note: "经验数值（1.2~1.5倍）无统计依据，跨行业照搬有风险（对应 BOOK_OVERVIEW 批判项）。"
```

```yaml
id: v-A09
title: 现金购销比率应大体对应营业成本率
type: principle
orig_ids: [pr43]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章第2节:比率定义与判据提出
    - 第5章第3节:在经营现金流"合理性"维度双向使用（收现对收入、付现对成本）
    - 第7章:综合案例中作为三表对表校验工序
V2_predictive_power:
  passed: true
  novel_question: "某零售企业现金购销比率0.95、营业成本率0.80，怎么解读？"
  derived_answer: "付现相对收现偏高0.15——预付占款、战略囤货或偿付前期应付；结合应付款项与存货余额变化定位，若是主动囤料则性质完全不同。通用比率体系没有这个对表判据。"
V3_exclusivity:
  passed: true
  why_not_common: "自创比率、非准则指标；把利润表与现金流量表逐项'对表校验'的判据设计是作者方法。"
```

```yaml
id: v-A10
title: 应收账款（商业债权）质量分析框架（真实性-周转性-保值性三步）
type: framework
orig_ids: [f12, pr17]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:三步框架与"常理解释不通即报警"
    - 第4章:商业债权周转率修正、应收激增列为恶化信号
    - 反面案例:万福生科/银广夏虚构收入挂账的后果印证
V2_predictive_power:
  passed: true
  novel_question: "某消费品牌应收账款激增50%但毛利率稳定——按框架查什么、结论是什么？"
  derived_answer: "先相对规模（应收增速远超收入增速即警报）→账龄是否被'洗短'→债务人构成是否关联方集中→坏账计提政策是否突变。毛利率稳定恰恰排除了低转成本配合，指向单纯虚增收入挂账；按后果模型，虚假应收挂不长，来年销售退回或坏账核销将致业绩跳水——可前瞻预判。"
V3_exclusivity:
  passed: true
  why_not_common: "'应收激增要小心'半常识；但'账龄可被人为洗短''与存货周转联动考察''先找经营性解释再报警'的成套程序+造假后果模型是作者判据。"
```

```yaml
id: v-A11
title: 债务人（客户）构成六维分析与客户集中度双刃剑
type: framework
orig_ids: [f13, pr34]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:六维清单（行业/区域/性质/关联/稳定/集中度）
    - 第4章:同一集中度问题从收入质量角度再次展开（双刃剑）
V2_predictive_power:
  passed: true
  novel_question: "某零部件公司前五大客户占收入85%且均为整车厂，债权与收入质量各是什么判断？"
  derived_answer: "集中度双刃剑：回款稳定、销售费用低，但大客户议价力强——降价与延付侵蚀毛利率、'敲竹杠'风险推高坏账；行业构成单一使行业下行共振。同一维度同时给债权质量与收入质量打分。"
V3_exclusivity:
  passed: true
  why_not_common: "'客户集中有风险'是常识；六维清单（区域构成看法制环境、所有制性质、'稳定客户过多=经营无起色'的反直觉判据）是作者细化。"
```

```yaml
id: v-A12
title: 向关联方打预付款潜藏利益输送（预付款项操纵配对）
type: principle
orig_ids: [pr22]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:预付款项质量分析与输送警报
    - 第6章:预付款项同时是控制性投资"藏身处"（越合并越小）——同一科目的第二种语境
    - 万福生科案例:虚增预付账款与在建工程的造假科目选择
V2_predictive_power:
  passed: true
  novel_question: "某公司预付账款一年增3倍，前五名收款方均为'非关联'供应商——能放心吗？"
  derived_answer: "先排除行业付款惯例与自身信用弱势（议价力弱被迫预付），再查供应商与实控人的实质关联（名义非关联）；两者都不成立即为输送通道，日后沦为不良资产。"
V3_exclusivity:
  passed: true
  why_not_common: "作者把预付款项与在建工程、其他应收款并列为'审计难度大、叙事上天然正面'的造假高危科目配对——这一科目-手法配对是作者的经验资产。"
```

```yaml
id: v-A13
title: 其他应收款过高即不正常——盯防大股东占用与集权例外
type: principle
orig_ids: [pr23]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:"既为'其他'，不应过大"判据与占用识别
    - 秋林集团案例:近40亿其他应收款几乎全额计提的极端样本
    - 第6章:集权资金管理下母公司大额其他应收款为正常输送——例外判据的第二语境
V2_predictive_power:
  passed: true
  novel_question: "母公司其他应收款60亿、合并仅5亿，子公司盈利良好——是大股东占用吗？"
  derived_answer: "'越合并越小'→差额属集权资金输送，质量取决于子公司盈利能力，不是占用；反之合并层面仍超常的部分才指向不良资产。同一科目、两种性质，差额判据完成分诊。"
V3_exclusivity:
  passed: true
  why_not_common: "这是作者的标志性经验判据（'银广夏后造假者爱上了其他应收款'），且集权例外防止一刀切误杀——外行只会看到'其他应收款大'就报警。"
```

```yaml
id: v-A14
title: 存货质量分析框架（构成-盈利性-周转性-保值性）
type: framework
orig_ids: [f14]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:四维框架与构成比例的管理含义
    - 第4章:毛利率诊断清单与低转成本操纵联动
    - 第7章:存货跌价准备作为不良资产区域
V2_predictive_power:
  passed: true
  novel_question: "某公司原材料占比骤降、产成品骤升、毛利率却持平——判读？"
  derived_answer: "滞销减产嫌疑或低转成本：产成品积压本应压低毛利率，持平说明成本结转可能被人为调低；查产销率与同行毛利率即可二选一，同时可变现净值减值风险上升（保值性报警）。"
V3_exclusivity:
  passed: true
  why_not_common: "'存货多压资金'是常识；构成比例译码（囤料vs滞销vs低转成本）与盈利性/周转性的战略取舍（茅台式高毛利vs薄利多销）是作者判据。"
```

```yaml
id: v-A15
title: 毛利率异常诊断清单（高五种原因/低三种原因）与"波动即证据"判据
type: framework
orig_ids: [f38, pr19]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:"产品结构未调整而毛利率巨幅波动=操纵显性证据"判读原则
    - 第4章第4节:高五种/低三种原因的系统化诊断清单
    - 蓝田/银广夏案例:低转成本操纵的点名印证
V2_predictive_power:
  passed: true
  novel_question: "某充分竞争行业企业毛利率连续两年高出同行10个百分点且产品结构未变——排除法剩什么？"
  derived_answer: "五种原因中垄断、竞争力、行业周期均可由行业数据排除，剩'产大于销摊薄固定成本'与'会计处理故意调高'二选一：查存货余额与产量数据即可定位，同时查审计报告。"
V3_exclusivity:
  passed: true
  why_not_common: "'高毛利好'是常识；作者给出'产大于销也能推高毛利'的反直觉归因与'波动即证据'的操纵判据（当期营业成本+期末存货=可供出售成本，此消彼长应大体不变）。"
```

```yaml
id: v-A16
title: 长期股权投资质量分析（盈利性四因素+权益法"泡沫"理论）
type: framework
orig_ids: [f15, pr20]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:四因素框架与泡沫资产概念
    - 第4章:投资收益含金量三分法落到检验程序
    - 第6章:控制性投资识别（长投口径之外藏身科目）同一概念家族
V2_predictive_power:
  passed: true
  novel_question: "某母公司权益法确认投资收益8亿，被投企业当年只分红1亿——母公司真实可支配收益多少？"
  derived_answer: "约1亿：7亿是泡沫（无现金支撑且同步做大长期股权投资账面）；评价其效益应看分红政策而非账面收益，且泡沫部分构成未来减值隐患。"
V3_exclusivity:
  passed: true
  why_not_common: "'投资收益要看现金'常识；'权益法收益必然有泡沫、泡沫大小=分红函数、成本法下母公司业绩只反映子公司分红政策'是作者的泡沫资产理论。"
```

```yaml
id: v-A17
title: 固定资产六维质量分析（含原值周转率口径）
type: framework
orig_ids: [f16]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:六维框架与三条配置合理性标准
    - 第4章:"必须用原值计算周转率"的系统论证
    - 第7章:固定资产减值作为不良资产区域
V2_predictive_power:
  passed: true
  novel_question: "某公司固定资产净值周转率3.0高于同行2.0——是效率更高吗？"
  derived_answer: "不一定：若同行折旧年限更长或减值计提更多，净值口径失真；用原值重算后可能反而落后——此时'虚增收入'与'虚增固定资产'二选一排查。"
V3_exclusivity:
  passed: true
  why_not_common: "'周转率高好'常识；原值口径、配置三标准（技术装备匹配行业定位/产能匹配份额/工艺匹配需求）、折旧-资本化-减值三个操纵点是作者的修正与配对。"
```

```yaml
id: v-A18
title: 在建工程质量分析两个切入点（未来利润指示器+长期不决算警报）
type: framework
orig_ids: [f18]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:明细预示盈利潜力+不决算三大好处
    - 万福生科案例:虚增在建工程的造假手法解剖
    - 第7章:募集资金变更用途检验的综合应用
V2_predictive_power:
  passed: true
  novel_question: "某公司募投项目已投产两年仍挂在建工程12亿——能推出什么？"
  derived_answer: "三重操纵通道同时打开：利息继续资本化、推迟折旧、当期费用混入工程成本——当期利润被虚增；工期过长的'合理解释'须以附注与投产证据验证。"
V3_exclusivity:
  passed: true
  why_not_common: "'在建工程要关注进度'常识；'迟迟不决算的三大好处'的操纵机理配对是作者解剖。"
```

```yaml
id: v-A19
title: 无形资产质量分析（披露结构决定分析起点：账内多为外购、自创游离表外）
type: framework
orig_ids: [f19]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:披露特点与两维分析
    - 第2章:货币计量局限（表外资源不可见）的理论呼应
    - 第4章:"无形资产/开发支出不正常增加=费用资本化、虚盈实亏"恶化信号
V2_predictive_power:
  passed: true
  novel_question: "某药企研发人员与专利众多但账面无形资产仅2000万——资产质量很差吗？"
  derived_answer: "恰恰不能这样判：自创无形资产支出全部费用化、游离表外，表内基本都是外购的——应转看开发支出、费用化研发投入与人力资本等账外资源，账面小可能是披露结构的产物而非质量差。"
V3_exclusivity:
  passed: true
  why_not_common: "'无形资产不好估值'常识；'账内无形资产基本都是外购的'这一披露结构判断及由此设定的分析起点是作者洞见。"
```

```yaml
id: v-A20
title: 减值准备双刃剑判读（挤水分工具同时是注水工具；不得转回使操纵向前端转移）
type: principle
orig_ids: [pr11, pr28]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章第3节:谨慎性原则双刃剑的制度分析
    - 第3章:各资产保值性评价中"计提恰当性"逐项应用；非流动资产减值不得转回的规则
    - 第4章:集中巨额计提（洗大澡）、扭亏年"小项目大贡献"列为恶化信号
V2_predictive_power:
  passed: true
  novel_question: "某公司连亏两年后第三年巨额计提商誉减值巨亏，第四年小幅盈利——链条怎么解读？"
  derived_answer: "洗大澡画像：第三年一次性出清+做低基数，第四年'扭亏'成色必须查核心利润与含金量而非净利润翻转；由于减值不得转回，操纵已转移到计提时点与比例的选择——第三年提100%还是60%就是利润安排。"
V3_exclusivity:
  passed: true
  why_not_common: "'减值可能洗大澡'在A股语境半常识；'挤水分工具同时是注水工具、不得转回只是把操纵推向计提时点'的制度层面分析是作者深化。"
```

```yaml
id: v-A21
title: 资产重分类（经营性/投资性）与资源配置战略三分类
type: framework
orig_ids: [f20]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第4节:重分类与三分类定义（判断入口在母公司报表）
    - 第4章:利润战略吻合性分析以之为底座
    - 第7章:八步法第②步与前景预测三线均以其为分线依据
V2_predictive_power:
  passed: true
  novel_question: "某家电企业资产中45%是长期股权投资与金融资产，核心利润占比却不足10%——归类与判断？"
  derived_answer: "投资主导型（或并重），但利润结构与资产结构严重不吻合→多元化战略实施效果差；转入母公司报表查控制性投资扩张效果与子公司分红回流量。"
V3_exclusivity:
  passed: true
  why_not_common: "'看资产结构'常识；按利润贡献方式重分类（现金归经营性、被占用款项归投资性）并据此给战略归类，准则口径与通用教材均无此体系——全书最具原创性的框架之一。"
```

```yaml
id: v-A22
title: 控制性投资为主体的企业的替代分析脉络
type: framework
orig_ids: [f30]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第4节:替代脉络（控制性投资→子公司核心利润→子公司经营现金净流量）提出
    - 第6章:差量分析法为其提供差额识别工具
    - 第7章:"母公司的控制性投资就是子公司的经营性资产"理论化表述
V2_predictive_power:
  passed: true
  novel_question: "投资控股型母公司报表连年'亏损'，子公司群实际盈利良好且分红正常——矛盾吗？"
  derived_answer: "不矛盾：成本法只认分红，母公司利润表业绩与子公司效益脱钩；用替代脉络（母公司长期股权投资/其他应收款/预付与合并对应项目之差→合并核心利润-母公司核心利润→子公司经营现金净流量）评估真实效益。"
V3_exclusivity:
  passed: true
  why_not_common: "'看合并报表'常识；为控股型母公司单设一条分析脉络、用三个报表差额构造替代指标，是作者独特设计。"
```

```yaml
id: v-A23
title: 利润结构与资产结构匹配性分析（战略吻合性操作程序）
type: framework
orig_ids: [f36]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第4节:双比例对照操作程序
    - 第3章:以资源配置战略分类为底座
    - 第7章:综合分析中检验战略实施效果
V2_predictive_power:
  passed: true
  novel_question: "母公司经营性资产：投资性资产=70:30，核心利润：投资收益=20:80——结论？"
  derived_answer: "结构错配：投资收益占比远超投资资产占比，可能是权益法泡沫或收益确认激进；核对投资收益含金量（分红回流）验证，长期看战略实施效果不佳。"
V3_exclusivity:
  passed: true
  why_not_common: "'结构与战略要匹配'是抽象常识；双比例对照、三个小项目的归置规则、控制性投资大时改三分类的具体程序是作者操作化。"
```

```yaml
id: v-A24
title: 负债质量分析框架（强制性分层+经营性负债信号）
type: framework
orig_ids: [f21]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第5节:流动负债四切入点+非流动负债三方面
    - 第6章:存贷双高三解释与两种三高互证
    - 第7章:预收款项偿付压力、资产金融性负债率的应用
V2_predictive_power:
  passed: true
  novel_question: "某公司流动负债中合同负债（预收）占40%、流动比率1.1——实际短期偿债压力如何？"
  derived_answer: "强制性分层：预收用存货偿付且含毛利折扣、属非强制性负债，实际压力远低于账面；真实风险在短期借款与应付票据部分——同一流动比率1.1，负债构成不同结论完全不同。"
V3_exclusivity:
  passed: true
  why_not_common: "'流动比率低于2危险'是经验常识；作者的强制性分层（沉淀性负债不算流动性风险）与'经营性负债=议价能力与行业生态信号'是反向判据。"
```

```yaml
id: v-A25
title: 所有者权益质量分析（输血性/盈利性变化二分+动态五关注）
type: framework
orig_ids: [f22]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第6节:静态两项目+动态五关注+输血/盈利二分
    - 第5章:现金流量的造血隐喻与之同构
    - 第7章:北陆"自力更生"型评价的应用
V2_predictive_power:
  passed: true
  novel_question: "某公司净资产三年翻倍但全部来自定增——质量如何？"
  derived_answer: "输血性变化：规模扩张≠盈利能力增强，须查入资用途（是否投向承诺项目）与ROE摊薄；若控股股东同时高质押，控制权风险叠加。同为净资产增加，输血与盈利的信号相反。"
V3_exclusivity:
  passed: true
  why_not_common: "'净资产增长是好事'常识；输血/盈利二分使同一增量信号方向反转——作者术语体系。"
```

```yaml
id: v-A26
title: 资本结构质量五关注（成本匹配/期限协调/财务弹性/控制权治理/利益相关者和谐）
type: framework
orig_ids: [f23, pr25, pr26, pr27]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第7节:五关注系统陈述
    - 第4章:ROA与借款利率比较的操作化（格力杠杆创造价值案例）
    - 第7章:"资产负债率过低也是问题"的双向评价为五关注延伸
V2_predictive_power:
  passed: true
  novel_question: "某公司资产负债率75%但几乎全是应付账款与预收款，ROA 8%、借款利率5%——高杠杆=高风险吗？"
  derived_answer: "五关注逐条：经营性负债主导→实际偿付压力低于账面；ROA>利率→杠杆在为股东创造价值；但须查期限协调（有无短融长投）与利益相关者和谐（对上游占款的可持续性）——结论从'高风险'变为'低金融风险+供应链依赖风险'。"
V3_exclusivity:
  passed: true
  why_not_common: "'负债率低更安全'是常识；五关注把资本结构拓展为成本/期限/弹性/控制权/和谐五维、明确反对单向评价——作者体系（含'过度权益融资=控制权旁落、招致野蛮人'的反直觉对偶）。"
```

```yaml
id: v-A27
title: 资本四分类与资本引入战略五类型（四大动力）
type: framework
orig_ids: [f24]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第7节:四分类五型定义与各型财务效应
    - 第6章:四大动力延伸到子公司层面做扩张归因
    - 第7章:八步法第⑤步与北陆"自力更生"分析
V2_predictive_power:
  passed: true
  novel_question: "某公司几乎没有有息负债、应付账款占负债80%、留存收益占权益90%——什么型？隐含什么风险？"
  derived_answer: "经营驱动+利润驱动并重：最稳健、实际偿债压力远低于账面负债率；但过于保守的利润驱动型可能沦为'野蛮人'猎物，且杠杆效应未发挥。"
V3_exclusivity:
  passed: true
  why_not_common: "传统分负债/权益；按融资渠道四分（经营性负债/金融性负债/股东入资/留存）并给出每型的治理与风险后果，是作者原创的读右边体系。"
```

```yaml
id: v-A28
title: 资产负债率过低也是问题——双向评价纪律
type: principle
orig_ids: [pr59]
V1_cross_domain:
  passed: true
  evidence:
    - 第7章第3节:北陆案例中"偿债指标极好≠状态最优"
    - 第3章:财务弹性关注（过高杠杆堵塞融资通道）构成另一端
V2_predictive_power:
  passed: true
  novel_question: "某公司资产负债率8%、账上现金充裕——该表扬吗？"
  derived_answer: "不：经营理念保守、财务杠杆效应未发挥、ROE被压低；应查有无增长机会——低金融性负债率同时意味着巨大的举债潜力未被使用，低杠杆本身是一项未动用的战略资源。"
V3_exclusivity:
  passed: true
  why_not_common: "'低负债安全'是大众常识；作者要求对任何偿债指标都问'这个水平的另一面是什么'——双向评价纪律。"
```

```yaml
id: v-A29
title: 利润质量三维分析框架（含金量/持续性/战略吻合性）
type: framework
orig_ids: [f25]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第4节:三维定义与"数量维度之外加质量维度"
    - 第5章:含金量以现金流量正式验证（获现率）
    - 第7章:三维综合评价在北陆案例落地
V2_predictive_power:
  passed: true
  novel_question: "某公司净利润大增50%，其中政府补助与投资收益占70%——三维各说什么？"
  derived_answer: "含金量：分项对现金（补贴回款账龄、投资收现）；持续性：非经常占比过高，扣非可能负增长；战略吻合性：利润结构与资产结构错配——三维合成为'规模增长不改变盈利质量差'的结论。"
V3_exclusivity:
  passed: true
  why_not_common: "'利润高好'常识；三维质量框架与'扭亏必须数量质量双翻转'的价值立场是作者对盈利评价的差异化重构。"
```

```yaml
id: v-A30
title: 利润表分层阅读（毛利→核心利润→营业利润）与口径纪律
type: framework
orig_ids: [f26, pr06]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第1节:三大支柱分层与核心利润定义
    - 第1章:"与营业收入无关的利润项目不得与收入对比"的口径纪律
    - 第4-7章:核心利润率/获现率/经营性资产报酬率全以其为口径
V2_predictive_power:
  passed: true
  novel_question: "甲公司营业利润5亿/营收100亿，乙公司核心利润6亿/营收80亿——谁的经营盈利能力强？"
  derived_answer: "营业利润含投资收益、补助等与收入无关项目，与营收不可比；以核心利润配对口径后：甲若核心利润仅3亿则3% vs 乙7.5%——乙更强。甲的'领先'可能全靠非经营项目美化。"
V3_exclusivity:
  passed: true
  why_not_common: "核心利润是作者自创概念（准则无此口径）；'营业利润的营业≠营业收入的营业、直接对比不可比'的口径纪律是其差异化贡献。"
```

```yaml
id: v-A31
title: "资产→利润→现金流量"三表对应总图（分线勾稽）
type: framework
orig_ids: [f29, f17]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:固定资产盈利性思路链（价值链版本，最早落点）
    - 第4章第4节:升格为三表对应总图（表4-20）
    - 第5章:现金验证线与总图衔接；第7章综合分析按线走
V2_predictive_power:
  passed: true
  novel_question: "经营性资产200亿/核心利润8亿/经营现金净额5亿；投资性资产100亿/投资收益6亿/投资收现0.5亿——三条线怎么诊断？"
  derived_answer: "经营线获现率0.63偏低→五类归因；投资线收益含金量极低→权益法泡沫或类别转换收益；两线结论合成：整体盈利质量差且问题主要在投资端——禁止跨线对比（如投资收益/营业收入）。"
V3_exclusivity:
  passed: true
  why_not_common: "'三表联动'是常识说法；'经营性资产→核心利润→经营现金'与'投资性资产→投资收益→投资收现'的严格分线对应与禁跨线纪律是作者的勾稽设计。"
```

```yaml
id: v-A32
title: 利润成长性分析（核心利润增长率优先+生命周期经验判据）
type: framework
orig_ids: [f34, pr36]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第4节:三个观察量与"非经营性变化"关注
    - 第3章:毛利率走势作为竞争力观察面的先行论述
    - 第7章:前景预测经营线的成长性输入
V2_predictive_power:
  passed: true
  novel_question: "某公司收入增速从35%降到8%、核心利润率同步下滑——生命周期判据说什么、还要查什么？"
  derived_answer: "从高成长（>30%）跌入稳定期（5-10%），核心业务竞争力走弱；关键动作是核对核心利润年度间'非经营性变化'（会计调整人为安排利润），只看收入增速会漏掉利润注水。"
V3_exclusivity:
  passed: true
  why_not_common: "增长率高好是常识；核心利润增长率优先+10%/30%生命周期判据+'过快成长等于加速灭亡'的双向风险观是作者判读。"
boundary_note: "10%/30%经验数值无统计依据，跨行业照搬有风险（BOOK_OVERVIEW 批判项）。"
```

```yaml
id: v-A33
title: 扭亏为盈必须是数量与质量的双重翻转
type: principle
orig_ids: [pr38]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章引例:ST卖房保壳被误判"扭亏"的引例
    - 第4章第4节:理论化（数量维度vs质量维度）
    - 第1章:传统比率局限中"扭亏根源是盈余管理与政府买单"首尾呼应
V2_predictive_power:
  passed: true
  novel_question: "某ST公司年报净利润转正，靠处置房产2亿——算扭亏吗？明年怎么预判？"
  derived_answer: "数量翻转≠质量翻转：核心利润仍为负、含金量看处置收现、持续性一次性——保壳式扭亏，来年大概率再亏；预判从'利好'反转为'警报'。"
V3_exclusivity:
  passed: true
  why_not_common: "'扭亏为盈是利好'是大众认知；作者以质量维度重新定义扭亏——反直觉且直接可操作。"
```

```yaml
id: v-A34
title: 营业收入质量"三问"框架（卖什么/卖给谁/靠什么）
type: framework
orig_ids: [f27, pr37]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第3节:三问展开为五维度
    - 第3章:债务人构成（卖给谁）在债权质量中的先行论述
    - 第7章:竞争力分析中五维度的应用
V2_predictive_power:
  passed: true
  novel_question: "某公司收入70%来自关联方购销，价格与市场价持平——三问给什么结论？"
  derived_answer: "'靠什么'维度：即便价格公允，交易实现时间的市场化仍存疑，且持续性依赖关联方存续——市场化能力不足；再以合并与母公司收入构成对比判断多元化/国际化程度。"
V3_exclusivity:
  passed: true
  why_not_common: "'看收入构成'常识；卖什么/卖给谁/靠什么的五维拆解及'行政手段贡献的收入的可持续性'判据是作者框架。"
```

```yaml
id: v-A35
title: 投资收益含金量三分法（持有收益/处置收益/类别转换收益）
type: framework
orig_ids: [f33]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第4节:三分法与现金回款公式
    - 第3章:泡沫资产概念先行
    - 第7章:北陆案例（权益法收益含金量0.61、类别转换收益1398万零现金流）标准示范
V2_predictive_power:
  passed: true
  novel_question: "某公司投资收益4亿=处置子公司股权3亿+权益法收益1亿——真实现金贡献多少？"
  derived_answer: "处置收益按售价定且一次性（剔除）；权益法1亿看对方分红与应收股利变动；类别转换部分零现金流——按公式重算后真实投资现金贡献可能不足1亿，与账面4亿差4倍。"
V3_exclusivity:
  passed: true
  why_not_common: "'投资收益有水分'泛常识；三类收益含金量截然不同的区分+现金回款公式（取得投资收益收到的现金±应收股利/利息变动）是作者的检验程序。"
```

```yaml
id: v-A36
title: 利润波动性与非经常性损益识别清单（含浮盈、资产处置的识别规则）
type: framework
orig_ids: [f35, pr32, pr33, pr41]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第4节:按活动列示的非经常候选清单与实质性判断规则
    - 第4章第3节:公允价值变动收益（浮盈）、资产处置收益逐项分析
    - 第3章:权益法/处置收益案例印证；ST卖房保壳贯穿
V2_predictive_power:
  passed: true
  novel_question: "某公司公允价值变动收益占净利润60%，监管口径不算非经常性损益——要不要紧？"
  derived_answer: "更要紧：浮盈未实现、零现金、市场不活跃时公允价值主观，且正是'花样扭亏'惯用通道；按作者原则，监管盲区里的占比过大项目要额外警惕并检验持续性。"
V3_exclusivity:
  passed: true
  why_not_common: "'扣非净利润更真实'已是市场常识；但'哪些算/不算的实质性判断规则+公允价值变动的监管盲区+资产处置2017年升格营业利润后的识别'是作者的清单化贡献。"
```

```yaml
id: v-A37
title: 政府补助（其他收益）质量四要点与含金量例外
type: framework
orig_ids: [f39, pr39]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第3节:四要点与"双刃剑"判断
    - 第4章第4节:补贴确认与收款脱节的含金量例外（长安28.73亿其他收益对应27.28亿未收回）
    - 光伏/新能源汽车行业评述:不当补贴后果
V2_predictive_power:
  passed: true
  novel_question: "某新能源车企其他收益30亿、应收补贴款28亿且账龄一年以上——补助质量？"
  derived_answer: "'有补贴收入、无补贴现金'：核对其他应收款中补贴款规模与账龄即可证实；政策阶段性决定其不可作为持续盈利基础——按'靠补贴生存的企业无持续竞争力'判据下调整体盈利质量。"
V3_exclusivity:
  passed: true
  why_not_common: "'补助不算真利润'半常识；四要点（政策关联度/研究能力/主业竞争力/阶段性）+'补贴挂账'含金量例外是作者细化。"
```

```yaml
id: v-A38
title: 经营活动现金流量质量"三性"分析（充足性-合理性-稳定性）
type: framework
orig_ids: [f42, pr45]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章第3节:三性定义与各性检查变量
    - 第7章:北陆按三性逐项展开
    - 乐视案例:三性缺失的反面标本；交易所对现金流量剧变问询的制度印证
V2_predictive_power:
  passed: true
  novel_question: "某公司经营现金净额连续三年为正且增长，但'收到其他与经营活动有关的现金'每年占流入35%——三性怎么说？"
  derived_answer: "合理性与稳定性报警：流入结构偏离'以销售收现为主'的行业常态，可能混入资金运作或关联往来；净额为正且增长不构成质量结论——必须拆结构。"
V3_exclusivity:
  passed: true
  why_not_common: "'经营现金流为正好'常识；三性把'为正'细化为充足/合理/稳定三维，流入构成与行业特征匹配、剧变即可疑是作者判据。"
```

```yaml
id: v-A39
title: 投资活动现金流量：匹配性分析无意义，应看战略吻合性（三线索）
type: framework
orig_ids: [f43, pr47]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章第3节:否定匹配性分析+三线索方法
    - 第3章:资源配置战略（对内/对外）为解读提供框架
    - 第7章:前景预测投资线与之衔接
V2_predictive_power:
  passed: true
  novel_question: "某制造业公司连续三年'购建长期资产支付现金'远小于'处置长期资产收回现金'——判读？"
  derived_answer: "收缩主业或被动收缩：结合经营净额是否同步改善定性——回款改善=战略退出（主动），经营不济=失血（被动）；后续用以后期间核心利润与经营现金流检验退出效果。"
V3_exclusivity:
  passed: true
  why_not_common: "'投资现金流要看平衡'是常见误读；作者先否定匹配性（投资回收有滞后性）、再立战略吻合性三线索——反向判据。"
```

```yaml
id: v-A40
title: 筹资活动现金流量质量（多样性+融资行为恰当性：主动vs被迫）
type: framework
orig_ids: [f44, pr48]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章第3节:两维度评价
    - 第6章:集权模式下母公司统一融资再输送的形态呼应
    - 乐视案例:被迫融资续命的反面标本
V2_predictive_power:
  passed: true
  novel_question: "某公司筹资净流入连续三年大额为正，同期经营净额为负、合并其他应收款大增——判断？"
  derived_answer: "被迫输血型融资+资金被无效益占用（筹资当期合并其他应收款大增正是作者列名的排查项）：筹资未纳入发展规划，属不良融资行为，高危。"
V3_exclusivity:
  passed: true
  why_not_common: "'能融到钱是本事'大众观；'主动扩张vs被迫输血'定性、过度融资与占款排查、多样性降本的行为恰当性判据是作者的。"
```

```yaml
id: v-A41
title: 现金流量表附注质量信息解读（间接法调节表+非现金交易双向解读）
type: framework
orig_ids: [f45, pr50]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章第3节:三块读法与双向解读原则
    - 第2章:附注作为个性化分析关键资料的定位
    - 第5章第3节:间接法调节表检验利润含金量与"净利润-经营现金"差异归因
V2_predictive_power:
  passed: true
  novel_question: "附注披露公司以一栋厂房抵偿供应商货款3亿，公司现金其实充裕——怎么解读？"
  derived_answer: "双向规则：若现金紧→困境信号（被动抵债、透支未来现金流）；若现金真充裕→可能是主动置换处置不良资产。结合现金存量与筹资活动定方向——同一笔非现金交易，两种相反结论。"
V3_exclusivity:
  passed: true
  why_not_common: "'看附注'是常识建议；间接法调节表做含金量归因+非现金交易不作单向结论的双面解读规则是作者的具体化。"
```

```yaml
id: v-A42
title: 现金流量变化归因清单与"禁止符号化判断"纪律
type: framework
orig_ids: [f46, pr44]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章第4节:表5-2按三类活动的归因清单
    - 第5章第3节:"不能仅凭净额正负下结论"的方法论定调
    - 第5章第3节:三类活动各有专属评价维度（三性/吻合性/恰当性）
V2_predictive_power:
  passed: true
  novel_question: "某公司经营现金净额由-2亿转为+9亿，媒体称'实质性改善'——先做什么？"
  derived_answer: "先归因：若改善来自压缩采购付款或占用上游（付款异常变化）则透支未来、非真改善；若来自回款正常化则为真改善——净额转正≠质量改善，必须进入变化过程。"
V3_exclusivity:
  passed: true
  why_not_common: "'现金流转正是好事'是大众判读；归因清单+禁止符号化结论的方法论纪律是作者的。"
```

```yaml
id: v-A43
title: 负的经营现金流量净额仅在特殊发展阶段可接受
type: principle
orig_ids: [pr46]
V1_cross_domain:
  passed: true
  evidence:
    - 第5章第3节:免责条件（初创期/转型期/危机期）
    - 乐视案例:连续大额为负靠借款续命的反面应用
    - 第4章:成熟企业获现不足即含金量问题的对照——发展阶段相对性
V2_predictive_power:
  passed: true
  novel_question: "一家转型期的传统零售，经营现金净额-3亿但投资活动大额流出建新业态——该惩罚它吗？"
  derived_answer: "转型期负净额可接受，但须验证新业态投资的方向吻合性与以后期间核心利润表现；若持续超预期年限且靠短期借款输血，免责失效转警报。"
V3_exclusivity:
  passed: true
  why_not_common: "'负现金流=差'是直觉；作者给出阶段性免责条件，防止对初创/转型企业误判——差异化判读。"
```

```yaml
id: v-A44
title: 合并报表只是会计主体的混合物——真金白银决策必须回到母公司报表
type: principle
orig_ids: [pr12]
V1_cross_domain:
  passed: true
  evidence:
    - 第2章第1节:法律主体vs会计主体的区分
    - 第6章:双重披露制的制度红利与差量分析法的前提
V2_predictive_power:
  passed: true
  novel_question: "集团合并流动比率2.5，母公司发行的20亿债券明年到期——合并口径能证明能还吗？"
  derived_answer: "不能：求偿权针对法律主体，合并数包含子公司资源且集团资源划拨受少数股东利益限制；必须回到母公司个别报表看可动用资源、存量现金与授信。"
V3_exclusivity:
  passed: true
  why_not_common: "'合并报表代表集团实力'是普遍认知；作者点破其法律主体局限并把'偿债、分红、付酬等真金白银决策以母公司报表为基础'定为纪律——反直觉判据。"
```

```yaml
id: v-A45
title: 合并报表编制质量仅体现逻辑关系的正确性
type: principle
orig_ids: [pr52]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章第3节:抵销在账外完成、无凭证账簿链条
    - 第6章第4节:由此推出应在差额与逻辑层面下功夫（差量分析的方法论依据）
V2_predictive_power:
  passed: true
  novel_question: "怀疑合并报表某项目有错，能否像审个别报表那样追凭证？"
  derived_answer: "不能——合并报表没有'报表-账簿-凭证-实物'可验证链条，只有逻辑关系一层保证；分析应在差额层面（抵销是否完整、越合并越小能否解释）并以母子公司个别报表交叉验证。"
V3_exclusivity:
  passed: true
  why_not_common: "一般人默认合并报表与个别报表同等可验证；作者点明其'弹性化'并据此选择分析方法——认识论层面的差异化判断，且是差量分析法的正当性来源。"
```

```yaml
id: v-A46
title: 常规比率分析在合并报表层面的三大失真（偿债/风险/营运）
type: principle
orig_ids: [pr53, pr56]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章第4节:三类失真系统论述
    - 第2章/第6章:偿债失真与"混合物"原理互证
    - 第7章:行业对标时降低信息聚合度的应用
V2_predictive_power:
  passed: true
  novel_question: "母公司外贸、子公司房地产开发的集团，合并存货周转率4次——能跟纯外贸同行比吗？"
  derived_answer: "不能：两类存货性质与周转标准完全不同，合并口径掩盖行业差异（另有未实现损益全额抵销使存货与成本同少数股东权益不配比）；应分个别报表口径分别对标。"
V3_exclusivity:
  passed: true
  why_not_common: "'合并比率可直接对标同行'是常见做法；作者列出偿债/风险/营运三类系统性失真及其机理（担保转贷抵销、多元化聚合）——差异化批判。"
```

```yaml
id: v-A47
title: 担保融资与转贷融资：合并数相同、风险不同
type: principle
orig_ids: [pr54]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章第4节:机制阐述（子公司融资两条路）
    - 第6章第4节:作为"合并信息存在显著差异"的核心例证用于方法论论证；与有限责任原理互证
V2_predictive_power:
  passed: true
  novel_question: "两家集团合并报表一模一样：一家子公司贷款全由母公司担保、一家是母公司借款转贷——谁的集团真实风险大？"
  derived_answer: "担保式：母公司以自身资产为全额贷款兜底（含少数股东应占份额）；转贷式：实际负担仅限持股比例部分。仅看合并报表无法区分，必须查附注担保信息与母公司报表。"
V3_exclusivity:
  passed: true
  why_not_common: "外行不可能从'抵销后报表相同'推出'风险不同'——高度反直觉的制度分析，是作者论证合并信息局限的招牌例证。"
```

```yaml
id: v-A48
title: 差量分析法（合并报表分析的特有方法）
type: framework
orig_ids: [f47]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章第4节:方法定义与定调（差量是信息而非误差）
    - 第4章:控制性投资替代脉络为其先声
    - 第7章:八步法第⑧步收口应用；特变电工/茅台/卫光三案例分证
V2_predictive_power:
  passed: true
  novel_question: "某集团合并毛利率18%、母公司毛利率35%，母公司销售费用仅0.3亿——集团是什么结构？"
  derived_answer: "三模式判别→母销子售型（类茅台销售公司结构）：合并毛利率高于母公司属业务结构使然而非异常；此后毛利率比较应在合并口径做，盈利比较前必须先定模式。"
V3_exclusivity:
  passed: true
  why_not_common: "'合并母公司对照看看'人人会说；作者把'差额本身是信息'方法论化并发展出四类结构化分析——招牌方法，无通用教材对应物。"
```

```yaml
id: v-A49
title: "越合并越小"双向差额法（资产端=控制性投资；负债端=子公司汇交资金）
type: framework
orig_ids: [f48, f59, pr24]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第3节:其他应收款语境的雏形（合并数远小于母公司数）
    - 第6章第4节:资产端系统化（控制性投资占用资源）+负债端（方大特钢约16.25亿汇集资金）
V2_predictive_power:
  passed: true
  novel_question: "母公司其他应收款70亿/合并8亿；母公司预收款项30亿/合并12亿——两个差额各是什么含义？"
  derived_answer: "资产端62亿=母公司对子公司资金输送（控制性投资的可能藏身处，质量取决于子公司盈利能力）；负债端18亿=子公司汇交母公司的资金规模，反推集权管理程度与统一融资降本空间。"
V3_exclusivity:
  passed: true
  why_not_common: "没有任何通用教材教'同一项目合并数小于母公司数，其差额即母子公司资金关系'——作者原创口诀，且资产端/负债端方向相反。"
```

```yaml
id: v-A50
title: 控制性投资的资产扩张效果分析（撬动倍数）
type: framework
orig_ids: [f49]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章第4节:合并与母公司资产差额的算法
    - 卫光生物案例:1.87亿仅撬动0.08亿的判读示范
    - 第7章:八步法第②步应用
V2_predictive_power:
  passed: true
  novel_question: "母公司控制性投资40亿，合并资产仅比母公司多45亿——效果评价与下一步？"
  derived_answer: "1元约撬动1.1元，扩张效果差；随后转入四大动力归因，查子公司经营性负债、借款、少数股东入资、利润积累哪个趋零。"
V3_exclusivity:
  passed: true
  why_not_common: "'扩张要看规模'常识；'控制性投资撬动倍数'的量化口径与'差额=杠杆出的子公司资产'的算法是作者设计。"
```

```yaml
id: v-A51
title: 子公司发展四大动力归因分析
type: framework
orig_ids: [f50]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章第4节:四个动力与判零程序
    - 第3章:四大动力理论的子公司层面延伸
    - 第7章:综合案例应用
V2_predictive_power:
  passed: true
  novel_question: "扩张效果差的企业：合并与母公司应付账款几乎相同、少数股东权益近零、合并与母公司未分配利润几乎相同——诊断？"
  derived_answer: "四动力逐项判零：经营性负债动力弱、少数股东入资零、子公司利润积累近零→只剩子公司金融性负债（查借款差额）——结论：杠杆驱动的扩张，风险最高的一种。"
V3_exclusivity:
  passed: true
  why_not_common: "'子公司发展靠什么'通常泛泛而谈；作者给出四个可从报表差额直接读出的动力及判零程序——结构化归因。"
```

```yaml
id: v-A52
title: 资金集权/分权管理模式的报表识别（两种"三高"）
type: framework
orig_ids: [f51]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章第4节:两种三高形态定义
    - 第3章:存贷双高三解释与之互证
    - 卫光/多数集团对照案例:分权与集权辨析
V2_predictive_power:
  passed: true
  novel_question: "某集团合并报表货币资金90亿、短期借款85亿、财务费用4亿；母公司货币资金5亿、其他应收款80亿——是存贷双高危机吗？"
  derived_answer: "母公司'三高'（借款高/利息高/其他应收款高且合并数远低）→集权模式：子公司资金汇缴、母公司统一融资下拨；合并端'存贷双高'是体制形态而非风险信号——与康得新式造假双高的区分在差额结构。"
V3_exclusivity:
  passed: true
  why_not_common: "'存贷双高=造假嫌疑'是市场流行判读；作者给出资金管理体制解释，使同一形态可能完全正常——反直觉且防止误杀。"
```

```yaml
id: v-A53
title: 母子公司业务关联度三模式判别与盈利费用比较
type: framework
orig_ids: [f52, f53]
V1_cross_domain:
  passed: true
  evidence:
    - 第6章第4节:三模式判别特征与费用比较程序
    - 特变电工/贵州茅台/卫光生物:三种模式各一正例
    - 第7章:集团管理特征分析应用
V2_predictive_power:
  passed: true
  novel_question: "合并销售费用8亿而母公司0.2亿，合并毛利率高于母公司——先判断什么、再比较什么？"
  derived_answer: "先定模式：母销子售型（消费税筹划的销售公司结构）→毛利率比较应在合并口径而非母公司口径做；研发/管理费用率差异指向职能在集团内的分布——不先定模式直接读合并毛利率会得出错误竞争力结论。"
V3_exclusivity:
  passed: true
  why_not_common: "差量口径下的业务模式判别表（费用分布、毛利率方向、成本倒挂）是作者独有；'模式判断决定比较方法适用性'是其方法论纪律。"
```

```yaml
id: v-A54
title: 流动比率经验值不能一刀切——龙头企业的OPM低流动比率悖论
type: principle
orig_ids: [pr15]
V1_cross_domain:
  passed: true
  evidence:
    - 第3章第2节:判据提出
    - 格力电器案例:第1章引例（被传统比率误判高风险）→第4章杠杆分析→第7章修正，贯穿使用
V2_predictive_power:
  passed: true
  novel_question: "某白电龙头流动比率1.1连续十年，供应商账期180天——按2:1标准该回避吗？"
  derived_answer: "OPM类金融模式：商业债务远大于商业债权，低流动比率是议价能力的主动安排而非偿债风险；真实检验在现金流与盈利能力——同时须警惕渠道模式被击穿时占款优势瞬间反转为风险。"
V3_exclusivity:
  passed: true
  why_not_common: "教科书2:1标准 vs 作者的OPM竞争力解释——明确反常识，且以格力被误判为主证案例，是'传统比率误判企业'论证链的钥匙。"
boundary_note: "经营性负债（占款）优势在供应链关系断裂情景下会显性化为风险（BOOK_OVERVIEW 批判项）。"
```

```yaml
id: v-A55
title: 利息保障倍数不能真正反映偿债能力
type: principle
orig_ids: [pr29]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第2节:指标功能重定义论证
    - 第3章:偿债能力=比率+项目质量+现金的框架互证
    - 第7章:修正比率线的组成部分
V2_predictive_power:
  passed: true
  novel_question: "某公司EBIT/利息=10，可以放心放一年期贷款吗？"
  derived_answer: "该倍数只说明借债政策对股东是否有利；一年期偿付取决于现金支付能力与债务结构——利息保障倍数高而货币资金受限、短债集中的公司照样违约。指标用途从'偿债'重定义为'借债政策评价'。"
V3_exclusivity:
  passed: true
  why_not_common: "教科书把利息保障倍数列为长期偿债指标；作者直接否定其偿债含义并重定义用途——对标准指标体系的公开修正。"
```

```yaml
id: v-A56
title: 周转率的口径修正纪律（原值计价/商业债权合并/增值税调整）
type: principle
orig_ids: [pr30]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第2节:三项修正系统提出
    - 第3章:应收/存货/固定资产周转分析中的口径要求
    - 第7章:可比性调整工序联动（格力商业债权周转率案例）
V2_predictive_power:
  passed: true
  novel_question: "某公司应收票据占商业债权60%，应收账款周转率显示回款很快——信吗？"
  derived_answer: "失真：应改用商业债权周转率（赊销净额/平均应收账款+应收票据）；同理周转率必须用减值前原值，否则得出'计提越多周转越快'的悖谬——先做口径配对修正再使用。"
V3_exclusivity:
  passed: true
  why_not_common: "常规用法直接取报表净值与单一科目；作者成套的口径配对修正（原值/票据并入/增值税）是其'修正传统比率'批判线的代表性资产。"
```

```yaml
id: v-A57
title: 总资产口径指标被非经营性资产稀释——改用经营性资产口径与"相对盈利区域"
type: principle
orig_ids: [pr31]
V1_cross_domain:
  passed: true
  evidence:
    - 第4章第2节:分母口径修正与分线报酬率
    - 第3章:经营性/投资性重分类为其底座
    - 第7章:经营性资产报酬率在综合分析中的应用
V2_predictive_power:
  passed: true
  novel_question: "某公司总资产300亿中100亿是闲置现金与理财，总资产报酬率2.5%——经营能力差吗？"
  derived_answer: "先拆分母：经营性资产报酬率（核心利润/经营性资产）可能达8%——诊断从'盈利差'反转为'资金使用差'（闲置现金拉低一切总资产口径指标且有机会成本）；经营与投资分线找'相对盈利区域'。"
V3_exclusivity:
  passed: true
  why_not_common: "总资产报酬率是通用指标；作者的'分母口径纪律+相对盈利区域识别'是对标准指标的差异化修正，与其重分类体系绑定。"
```

```yaml
id: v-A58
title: 预收款项的实际偿付压力小于账面金额（偿付=存货，含毛利折扣）
type: principle
orig_ids: [pr58]
V1_cross_domain:
  passed: true
  evidence:
    - 第7章第3节:量化修正机制提出
    - 第3章:预收款项/合同负债作为非强制性负债与业绩晴雨表的论述
V2_predictive_power:
  passed: true
  novel_question: "某白酒企业预收款项80亿占流动负债50%、流动比率1.3——真实短期偿付压力多大？"
  derived_answer: "预收以存货偿付且账面金额含毛利折扣（需偿付的商品成本=预收/(1+毛利率)），实际现金偿付压力远低于账面——其流动比率被结构性低估，这是商业模式质量与议价能力的信号而非风险。"
V3_exclusivity:
  passed: true
  why_not_common: "把预收当普通负债计算流动比率是通用做法；作者给出'偿付=存货/(1+毛利率)'的修正机制——非显然的量化判据，与强制性分层配合使用。"
```
