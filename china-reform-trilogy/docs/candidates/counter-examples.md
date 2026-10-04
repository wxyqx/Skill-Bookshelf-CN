# candidates/counter-examples.md — 《中国改革三部曲》阶段 1 反例提取

```yaml
- id: ce01
  title: 匈牙利价格扭曲恶性循环
  type: counter-example
  source_chapter: Ⅰ第二讲
  source_quote: |
    匈牙利败于竞争性市场未确立——价格越随意→再分配越广→价格越随意（科尔奈）；资本市场缺位致预算软约束。
  failure_mode: 只放开部分价格而不建立竞争性市场与硬预算约束，政府被迫反复再分配干预，改革循环倒退。
  mechanism: 局部市场化在扭曲环境中自我强化扭曲。
  warning_signs: [部分价格放开部分管制, 补贴与再分配不断扩大, 软预算约束未破]
  bound_to: ["经济体制四象限"]
  tags: [counter-example, transition]

- id: ce02
  title: 双轨制的权力货币化
  type: counter-example
  source_chapter: Ⅱ第二章
  source_quote: |
    双轨并存造成寻租环境——租金总额占 GDP 20%-30%；行政管制创租—寻租—设租的恶性循环。
  failure_mode: 过渡性双轨制固化为利益结构，权钱交易制度化，改革动力被既得利益俘获，滑向权贵资本主义。
  mechanism: 价差即租金；掌握分配权者既得租金又有动力维持并新增管制。
  warning_signs: [租金/GDP 比率居高, 官商结合制度化, 改革议程被既得利益主导]
  bound_to: ["增量改革与双轨制寻租"]
  tags: [counter-example, rent-seeking]

- id: ce03
  title: 国企承包制的内部人控制
  type: counter-example
  source_chapter: Ⅱ第四章
  source_quote: |
    放权让利三种形式共同失败：剩余权被内部人分享导致产权更模糊；"剥离上市"留下存续企业掏空上市公司的治理缺陷。
  failure_mode: 不改变产权框架只改善治理（或只放权），剩余索取权与控制权错配，内部人短期化与掏空并存。
  mechanism: 所有权虚置时，扩权=内部人控制，收权=回到行政束缚——两难反复。
  warning_signs: [承包指标博弈, 存续企业掏空上市公司, 五龙治水的多头干预]
  bound_to: ["国企改革两难"]
  tags: [counter-example, soe]

- id: ce04
  title: "苏联现象"——高研发低 TFP
  type: counter-example
  source_chapter: Ⅲ第二章、第六章
  source_quote: |
    苏联建立了世界上规模最为宏大的官办教育体系和科研体系……全要素生产率逐年下降——庞大的研发体系在缺乏适宜制度条件时无法提供激励。
  failure_mode: 以政府规划、国家投资、重点攻关推动技术进步，结果投入巨大而效率下降。
  mechanism: 封闭僵硬的行政科研体制压抑科学家创造性；缺少市场竞争筛选与产权激励。
  warning_signs: [研发占比高而 TFP 为负, 科研行政化官本位, 重点攻关依赖症]
  bound_to: ["增长模式转变"]
  tags: [counter-example, innovation]

- id: ce05
  title: 后发劣势的模仿捷径
  type: counter-example
  source_chapter: Ⅲ第六章（引杨小凯）
  source_quote: |
    后发国家往往选择简单模仿技术和管理方法的"捷径"……没动力在根本性制度上做变革，结果牺牲了长久繁荣的机会——"后发优势"反倒成了"后发劣势"。
  failure_mode: 用技术模仿替代制度变革取得短期成就，长期被制度短板锁死。
  mechanism: 技术模仿的收益立现、制度变革的成本立现而收益远期——激励天然偏向捷径。
  warning_signs: [增长靠投入堆积, 制度改革议程一再推迟, 增长模式反复回潮]
  bound_to: ["增长模式转变", "法治的市场经济"]
  tags: [counter-example, latecomer]

- id: ce06
  title: 理论先驱的执行落差
  type: counter-example
  source_chapter: 全书（作者方法的自反风险）
  source_quote: |
    整体协调改革论的方案（1986 价税财金贸联动等）三次设计三次夭折——方案自认"一环出错全盘打乱"却无失败预案；"效率优先"表述与后期的社会公正强调存在张力。
  failure_mode: 规范性理论体系的可行性论证弱于其批判力——方案设计者的角色使评估偏向自身范式。
  mechanism: 理论自洽不等于政治可行；方案设计者评估自身方案存在利益与认知偏差。
  warning_signs: [方案依赖理想执行者, 失败归因于环境而非方案, 概念体系免于检验]
  bound_to: ["所有本源skill的Boundary"]
  tags: [counter-example, meta]
```
