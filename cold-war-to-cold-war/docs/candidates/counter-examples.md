# candidates/counter-examples.md — 《从"老冷战"到"新冷战"》阶段 1 反例提取

```yaml
- id: ce01
  title: 苏东非货币化陷阱
  type: counter-example
  source_chapter: 第二章
  source_quote: |
    不进入货币化，不代表不发行主权货币，只是他们不把货币作为主要交易手段……其可调配的资本无法与金融化后的西方国家相比，其各领域的投资都将严重滞后。
  failure_mode: 拒绝货币化使实体经济无法参与金融竞争——生产虽好，但投资能力、增长计量、话语权全面落败，最终在军备竞赛与粮油价操纵下财政崩溃。
  mechanism: 金融竞争时代，货币是调配资源的杠杆；放弃这个杠杆=用步兵对抗骑兵。
  warning_signs: [货币仅计价不交易, 金融产业停滞, 增长计量体系被人定义]
  bound_to: ["货币化主权"]
  tags: [counter-example, monetization]

- id: ce02
  title: 休克疗法式激进转轨
  type: counter-example
  source_chapter: 第三章
  source_quote: |
    当原有体制骤然发生改变，而非渐进改变时，其代价是巨大的——实体资产迅速的以十分低廉的价格被交易出去。
  failure_mode: 无定价体系骤然市场化，资产被硬通货低价收割，产业配套体系被打散，技术资本人才全方位流失。
  mechanism: 交易需要定价经验与金融体系；一步到位的开放等于把无定价资产摆上货架。
  warning_signs: [激进私有化时间表, 资本账户骤开, 生活必需品匮乏与资产甩卖并存]
  bound_to: ["危机收割机制", "货币化主权"]
  tags: [counter-example, transition]

- id: ce03
  title: 三来一补打乱产业体系
  type: counter-example
  source_chapter: 第三章
  source_quote: |
    大量低端外资进入，将沿海城市变为了靠外部设备来形成生产能力的"三来一补"发展模式……国内上游装备制造业失去了下游市场。
  failure_mode: 危机压力下无门槛引入低端加工贸易，短期换汇长期摧毁上游装备制造业的下游市场，产业体系被外部定义。
  mechanism: 低端嵌入打乱上下游配套，本地装备失去内需验证与迭代场景。
  warning_signs: [加工贸易占比畸高, 本地装备业订单萎缩, 技术引进限于组装环节]
  bound_to: ["产业转移的双向命运"]
  tags: [counter-example, industrial]

- id: ce04
  title: 荷兰病——金融暴利挤死实体
  type: counter-example
  source_chapter: 第四章
  source_quote: |
    由于一个行业的暴利，将另一个行业挤死……实体产业由于资本的不断外逃，出现严重的萎缩——美国金融业和服务业占 GDP 85% 以上。
  failure_mode: 金融获利远超实体，资本持续外逃，实体萎缩与就业流失不可逆， QE 流动性进不了实体。
  mechanism: 资本逐利性使高收益虚拟部门虹吸低收益实体；体制（私人央行、党争）使自我纠正不可能。
  warning_signs: [金融业占比畸高, 制造业就业持续流失, 宽松货币进不了实体]
  bound_to: ["金融排斥机制"]
  tags: [counter-example, financialization]

- id: ce05
  title: 承接国用西方话语描述自己
  type: counter-example
  source_chapter: 第一章、第二章
  source_quote: |
    发展中国家在面对种种矛盾和剥削时，用修饰过的西方话语来描述自己，更加丧失了在话语上的主动权，迷失在了所谓自由，民主，人权等毫无意义的辩论中。
  failure_mode: 引进产业同时全盘接受西方知识体系，遭遇剥夺时只能用剥夺者的话语抗争，诉求无法成立。
  mechanism: 知识体系是软实力载体；话语不自立则利益表达失语。
  warning_signs: [理论概念全盘移植, 本国经验无法自我解释, 争论困在对方设定的议程]
  bound_to: ["意识形态软实力分析"]
  tags: [counter-example, discourse]

- id: ce06
  title: 强意图推断的叙事风险
  type: counter-example
  source_chapter: 全书（作者方法的自反风险）
  source_quote: |
    伊拉克改用欧元结算被灭国、科索沃战争为打欧元、肯尼迪遇刺与美联储——作者以强意图推断串联事件，相关性叙事被呈现为因果机制。
  failure_mode: 把金融竞争框架过度延伸，用意图推断替代证据链，削弱框架的可信度与可检验性。
  mechanism: 单一范式吸收一切反例（对称性差）；叙事连贯性被误认为解释力。
  warning_signs: [每个事件都被同一框架解释, 意图推断无文件级证据, 反例被再解释吸收]
  bound_to: ["所有本源skill的Boundary"]
  tags: [counter-example, meta]
```
