# verified.md — 阶段 1.5 三重验证产出

> 验证对象：阶段 1 的 39 条框架/原则候选（案例 25 条、反例 10 条、术语 15 条按其 bound_to 直接进入 A1/B/共享词典，不参与独立 skill 验证）。
> 去重合并：f05+p01、f14+p02、f09+p11、f15+p20、f19+p17+p05+p06、p16 并入 f05。
> 通过 19 个，淘汰/降级 14 个。通过率 49%（方法论密集型书的正常区间）。用户已选全自动模式，本名单自动确认。

## 通过名单（→ 进入阶段 2）

```yaml
- id: f01
  title: 黄奇帆五步分析法
  V1_cross_domain: {passed: true, evidence: [第2章: 双循环堵点分析, 第6章: 房地产拐点分析, 第12章: 脱钩推演]}
  V2_predictive_power: {passed: true, novel_question: "分析一个地方政府新能源汽车招商方案是否靠谱", derived_answer: "按五步走：现有产能与渗透率数据→充电/补贴/土地边界条件→本地配套率机制→与光伏过剩周期类比推演→分级建议；可判定其是产能重复建设还是集群补链"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'具体问题具体分析'；此法给出固定五步与每步证据类型（数据/边界条件/机制/推演/对策），是可执行的分析骨架"}
- id: f02
  title: 边界条件分析法
  V1_cross_domain: {passed: true, evidence: [第6章: 房地产十大拐点, 第2章: 外贸依存度64%→32%→25%的格局判断, 第3章: 光伏成本交叉点判断]}
  V2_predictive_power: {passed: true, novel_question: "当前国内咖啡连锁行业是周期低谷还是结构性拐点？", derived_answer: "列边界条件：人均杯数远低于成熟市场（未触顶）、商圈点位密度（渐触顶）、资本杠杆（触顶）、价格带（击穿）→ 结论：扩张模式到拐点但需求未到拐点，是'供给侧出清'而非'需求见顶'"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'看周期'；此法把工程学'边界条件'引入行业分析，要求列慢变量清单并逐项判触顶，区分'结构性'与'周期性'有明确判别程序"}
- id: f03
  title: 兵棋推演式对抗分析
  V1_cross_domain: {passed: true, evidence: [第12章: 十大脱钩逐项推演, 第6章: 房企破产传导链推演, 第3章: 清洁能源替代节奏推演]}
  V2_predictive_power: {passed: true, novel_question: "若某国禁止向我国出口高端光刻机服务，售后维权情景如何演化？", derived_answer: "清单化后推演：对我冲击（存量设备折旧加速）→对对方反冲击（丢失维保现金流与备件市场）→按三维度定级为高风险但'半脱钩'形态→应先保存量维约、加快自检修体系"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'换位思考'；此法要求双向冲击测算+'杀敌一千自损八百/三千'相对代价判据+按发生可能性（非危害度）分级的完整程序"}
- id: f05
  title: 先立后破节奏控制（含'窄起步轻负担'的立制度节奏）
  V1_cross_domain: {passed: true, evidence: [第3章: 能源替代3:1节奏, 第7章: 遗产税'征税面从窄税负从轻', 第6章: 预售制'不交楼不月供'的渐进改革]}
  V2_predictive_power: {passed: true, novel_question: "公司要从自建机房全面迁移上云，节奏怎么定？", derived_answer: "先立：云上跑影子流量并建双活冗余→爬行钉住按每季度20%迁移→旧机房保留为灾备冗余直至云上SLA连续4个季度达标才退；退出节奏由建成进度而非目标日期决定"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'稳步推进'；此法给出'爬行钉住+保留安全冗余'的量化节奏控制与'退出节奏由建成进度决定'的硬规则"}
- id: f06
  title: 产地销/销地产二分法
  V1_cross_domain: {passed: true, evidence: [第5章: 跨国公司选址基本原则, 第9章: RCEP给在华日企扩大市场, 第12章: 问答中判断产业转移传言]}
  V2_predictive_power: {passed: true, novel_question: "关税上涨后，一家出口型家电企业会迁厂东南亚吗？", derived_answer: "用二分法+时间常数判断：整机厂（搬厂1-2年）若销地产优势占优可能部分迁；但配套模具/注塑产业链搬迁需3-5年且集群效应在原址，完全迁走概率低→判断为'组装环节部分外移、集群留守'"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'看成本'；此法把布局归结为两种基本盘+各自的成立条件清单，并给出搬迁时间常数作证伪工具"}
- id: f07
  title: 产业链权力五类型与链头三链
  V1_cross_domain: {passed: true, evidence: [第5章: 五类型+苹果案例, 第12章: 产业链为王牌中的王牌的权力来源论证]}
  V2_predictive_power: {passed: true, novel_question: "一家新能源车代工厂如何提升自己的利润分成？", derived_answer: "按五类型定位：现在处于外包代工型（总装20%价值）；升级路径是向龙头带动型爬升——先掌握一两个核心环节（电池/智驾）做50%价值环节，或沉淀供应链纽带能力（集采、结算）再谋链头"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'微笑曲线'；此法给出五种管控类型谱系与'三链'（标准/纽带/枢纽）判据，比曲线更可操作"}
- id: f08
  title: 超大规模市场三效应
  V1_cross_domain: {passed: true, evidence: [第5章: 六项成本摊薄30-40%, 第2章: 引力场效应与内需体系, 第1章: 城市化与内循环动力]}
  V2_predictive_power: {passed: true, novel_question: "为什么越南难以复制中国的全产业链吸引力？", derived_answer: "越南缺'超大规模单一市场'三要素：体量不足以摊薄六项固定成本、无引力场（需求虹吸产能）、内部市场规则不单一→结论：它只能做'销地产'节点而非'产地销'母港"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'规模经济'；此法拆出全门类×超大规模×单一市场三位一体与可检验的六项成本摊薄机制"}
- id: f09
  title: 数据产权四权分层
  V1_cross_domain: {passed: true, evidence: [第4章: 四权分层设计, 第8章: 数据'1+3+3'产品体系与交易所国有控股]}
  V2_predictive_power: {passed: true, novel_question: "智能汽车行驶数据归谁？车企能否出售脱敏后路况数据？", derived_answer: "按四权分层：原始个人驾驶数据所有权归车主、车企仅持使用权且不得杀熟式差别定价；脱敏聚合后的路况数据车企可拥有并出售，车主无收益主张权；数据交易所须经监管准入"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'数据归用户'或'数据归平台'二极管；此法给出按脱敏与流转环节分层的四权结构，且交代了个人无脱敏收益主张权的现实理由（举证成本不可操作）"}
- id: f11
  title: 滚雪球战略
  V1_cross_domain: {passed: true, evidence: [第9章: RCEP为雪核逐层扩大朋友圈, 第12章: 反制措施十'FTA滚雪球助入CPTPP']}
  V2_predictive_power: {passed: true, novel_question: "一个新兴开发者社区如何扩大生态伙伴？", derived_answer: "以最大存量合作方为雪核签深度互认→按由易到难逐层吸收（工具商→内容商→竞对社区），每层以存量雪球规模为谈判筹码，'以我为主'定义接入标准"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'多交朋友'；此法强调雪核选择、滚动次序与'以存量规模为筹码'的累积博弈结构"}
- id: f12
  title: 制度基因分析法
  V1_cross_domain: {passed: true, evidence: [第11章: 香港三大制度基因+历史验证, 第8章: 土地三次改革（制度变革解释增长）]}
  V2_predictive_power: {passed: true, novel_question: "海南自贸港能否取代香港？", derived_answer: "用基因清单对照：自由港体系可移植、税制可移植，但普通法系与国际公信法治（判例体系+仲裁生态）数十年难复制，且血脉（内地需求与资本通道）不可替代→短期是分流，长期是互补"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'营商环境重要'；此法要求找出一组'可遗传、难复制、经危机验证'的制度组合并与外部输血分开归因"}
- id: f14
  title: 源头治理思维
  V1_cross_domain: {passed: true, evidence: [第7章: '凡是广泛存在、长期存在的问题一定要从制度、基础土壤的角度去分析求解', 第2章: 六类体制堵点溯源, 第8章: 要素市场化治本论]}
  V2_predictive_power: {passed: true, novel_question: "公司销售团队常年虚报 pipeline，屡罚不止怎么办？", derived_answer: "广泛+长期→制度土壤问题：查 CRM 考核规则、线索分配机制与提成确认时点等基础规则，而非加强惩罚；改'签约确认收入'为'回款确认'等源头规则重构"}
  V3_exclusivity: {passed: true, why_not_common: "'治本不治标'是常识，但此法给出可操作的判别触发器（广泛存在+长期存在→必是制度问题）与上溯路径（生产力源头/要素配置/产权），把格言变成检查程序"}
- id: f15
  title: 长周期'不会变'判断法
  V1_cross_domain: {passed: true, evidence: [第12章: 五个不会变, 第1章: 三大台阶的结构性依据]}
  V2_predictive_power: {passed: true, novel_question: "政策寒冬里该不该继续投入职业教育内容创业？", derived_answer: "列十年级结构趋势：技能半衰期缩短（技术革命）、制造业升级对技能人才需求、政策对技能薪酬制度的改革方向→短期整顿是噪声，结构性趋势支持继续，但须按'先立后破'调整合规形态"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'看长期'；此法要求先显式列出结构趋势清单、再以'与趋势同向放大/反向视为噪声'的规则过滤短期波动"}
- id: f16
  title: 技术创新三环节
  V1_cross_domain: {passed: true, evidence: [第8章: 0-1/1-100/100-100万+拜杜法案, 第4章: 六大短板与核心装备研发, 第5章: 基础研究占比6%的短板]}
  V2_predictive_power: {passed: true, novel_question: "某高校科技成果转化率低，卡在哪一环？", derived_answer: "逐段检查：0→1看基础研究投入与评价导向；1→100看产权分成与技术经理人（最常见断点：无1/3分成安排、无转化经纪人）；100→100万看中试资金与场景——诊断出断点后再对症投入"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'产学研结合'；此法把链条切成三段并给每段配置判别指标与制度工具（拜杜1/3分成、技术经理人、独角兽培育）"}
- id: p03
  title: 一次分配优先原则（三次分配次序）
  V1_cross_domain: {passed: true, evidence: [第7章: 三次分配格局+六方面入手, 第1章: 居民可支配收入占GDP 42%→52%目标]}
  V2_predictive_power: {passed: true, novel_question: "行业协会倡议'企业家多捐款缩小贫富差距'有效吗？", derived_answer: "按次序判断：三次分配是配套辅助，捐赠占比提升依赖税制激励（中美捐赠差异在财产税抵扣制度而非道德）；真正杠杆在一次分配——提高劳动报酬占比与劳动者持股，倡议收效有限"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'富人多捐点'；此法明确'一次分配讲效率兼顾公平是基础'的次序与'捐赠差异在制度不在道德'的反直觉归因"}
- id: p07
  title: 制造业占比红线诊断
  V1_cross_domain: {passed: true, evidence: [第5章: 国际经验四特征+25%/20%红线, 第12章: 全门类产业链是'王牌中的王牌'的支柱论证]}
  V2_predictive_power: {passed: true, novel_question: "某沿海城市服务业占比升到70%，该高兴还是警惕？", derived_answer: "查四特征：是否迈入高收入后才降、下降是否渐进、科研是否同期领先、生产性服务业是否同步；若靠房地产金融推高服务业占比且制造业加速外流→警惕空心化而非庆祝"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'产业结构高级化=服务业占比升'；此法给出反直觉红线与四特征判别器"}
- id: p10
  title: 自主可控的边界（反'小而全'）
  V1_cross_domain: {passed: true, evidence: [第9章: '绝不追求任何技术100%自给', 第12章: 科技脱钩推演中'先保卡脖子环节'+日用消费自保即可]}
  V2_predictive_power: {passed: true, novel_question: "公司该不该自研全部中间件？", derived_answer: "用'断供是否一剑封喉'筛：数据库/核心调度等封喉环节自研+开源双备份；通用报表/消息中间件保持采购——全部自研会把资源从关键环节稀释掉"}
  V3_exclusivity: {passed: true, why_not_common: "常识有两派（全自研 vs 全采购）；此法给出按'封喉程度'分配自主化投入的判据，反'小而全'"}
- id: p14
  title: 相对成本判断政策转向
  V1_cross_domain: {passed: true, evidence: [第3章: 光伏度电成本与火电交叉点, 第4章: 数字人民币替代SWIFT'漫长历史过程'的成本论证]}
  V2_predictive_power: {passed: true, novel_question: "钠离子电池补贴退坡后会死掉吗？", derived_answer: "看钠电与磷酸铁锂的度电成本曲线交叉预期：若在3年内交叉，退坡是技术成熟的确认信号，行业反而进入自主成长；若远未交叉，退坡即是出清开始"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'盯补贴文件'；此法反直觉：补贴取消是交叉点过后的确认信号而非利空"}
- id: p26
  title: 金融开放次序与护身符
  V1_cross_domain: {passed: true, evidence: [第10章: 货币自由兑换两前置条件, 第12章: 三个护身符+广场协议/休克疗法反例]}
  V2_predictive_power: {passed: true, novel_question: "某新兴市场被游资冲击，为何有的崩盘有的扛住？", derived_answer: "查护身符清单：资本项下是否管制、外债/外资头寸是否过度、贸易体量是否形成引力；广场协议式汇率急升+资本自由化次序错误→崩盘；有盾牌者可承受冲击"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'开放好、管制坏'二极管；此法把资本管制定位为博弈盾牌并给出可检验的开放前置条件清单"}
- id: f19
  title: 城市层级齿轮与土地标尺
  V1_cross_domain: {passed: true, evidence: [第1章: 城市群五约束+1:3梯次+1500万天花板, 第6章: 人均100平米/住宅25%/楼面地价1/3+深圳缺口案例, 第6章问答: 京津冀缺中等城市反证]}
  V2_predictive_power: {passed: true, novel_question: "两个相邻省会城市都喊人口破千万，谁的房子更值得长期持有？", derived_answer: "查齿轮与土地标尺：首位城市是否已达1500万天花板、腹地是否有1:3梯次承接（缺齿则辐射断档）、人均建设用地是否超100平米（透支）、住宅用地占比与楼面地价/房价比是否在1/3内→标尺健康者更可持续"}
  V3_exclusivity: {passed: true, why_not_common: "常识是'看人口流入'；此法给出一组可核查的量化标尺（100平米/25%/1/3/1:3/1500万）与齿轮啮合结构判据"}
```

## 淘汰/降级名单（审计记录，详见 rejected/REJECTED.md）

f04 增速倍率法（V3：敏感性分析属通用方法，降级为 f01 的 example）· f10 数字化四步骤（V1：仅第4章单一语境，降级为 example）· f13 三个三定位（V3：三层三点属通用定位清单，降级）· f17 改革三类型（降级为 f14 的 example）· f18 要素市场五功能（V1 单一语境，降级）· p04 法拍指标（并入 f02 的 E 段与 A1）· p08 杠杆警戒线（V3：50%/80% 阈值近常识）· p09 不交楼不月供（V1 单一语境，并入 f05 的 A1）· p11 数据两规则（并入 f09）· p12 平台重罚十倍（V1：仅第4章同一语境，降级为 example）· p13 战略藐视战术重视（V3：格言近常识，并入 f03 的 B 段）· p15+p20（合并为 p26）· p17（并入 f19）· p01/p02（分别并入 f05/f14）
