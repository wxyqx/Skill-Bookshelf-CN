# INDEX — 《精益创业》13 Skill 主题索引

> cangjie-skill 流水线 · 阶段 3（链接器）产出 · 2026-10-07
> 书：《精益创业：新创企业的成长思维》（埃里克·莱斯）
> 全部条目来自 `skills/` 目录下 13 个已完成的 SKILL.md，链接均为相对路径。

---

## 一、总纲与元判断（体系入口与"该不该做"）

- [lean-startup-five-principles](../skills/lean-startup-five-principles/SKILL.md) — **精益创业五项原则**：判断精益创业是否适用于你的处境（新创企业定义、创业即管理、火箭发射 vs 汽车驾驶、愿景—战略—产品），整本书的根目录与入口。
- [anti-waste-discipline](../skills/anti-waste-discipline/SKILL.md) — **反浪费纪律**：识别 21 世纪的新浪费（高效地做根本不该做的事），并防止精益创业自身教条化、伪科学化；站在全部执行 skill 之上的元判断。

## 二、学习循环与假设实验（"驾驭"篇前半：循环怎么转）

- [bml-validated-learning](../skills/bml-validated-learning/SKILL.md) — **经证实的认知与 BML 循环**：以经证实的认知为进展单位，把开发—测量—认知循环跑对跑快；计划顺序与执行顺序相反，对顾客的假设拉动开发。
- [leap-of-faith-assumptions](../skills/leap-of-faith-assumptions/SKILL.md) — **信念飞跃假设**：动手之前把"我们在赌什么"说清楚——价值假设与增长假设、类比与反证、现地现物、柯达四问、找早期使用者。
- [mvp-design-patterns](../skills/mvp-design-patterns/SKILL.md) — **MVP 设计模式**：把假设变成最小实验——视频式、贵宾式、绿野仙踪、冒烟测试的选型，以及法律/竞争/品牌/士气四大减速路障的排障。
- [startup-quality-philosophy](../skills/startup-quality-philosophy/SKILL.md) — **新创企业质量观**：化解"要不要做到完美再上线"之争——不知顾客即不知质量、早期使用者接受八成产品、尽早发布，但不为时间牺牲会拖慢循环的质量。

## 三、衡量与核算（"驾驭"篇后半：进展怎么证明）

- [innovation-accounting](../skills/innovation-accounting/SKILL.md) — **创新核算**：三步问责体系（定基准线→调整引擎→转型或坚持）与认知的阶段性目标，回答"怎么向老板/投资人证明有进展"。
- [actionable-vs-vanity-metrics](../skills/actionable-vs-vanity-metrics/SKILL.md) — **可执行指标 vs 虚荣指标**：同期群分析、对比测试、漏斗衡量与"可执行/可使用/可审查"三标准；看方向和程度而非当前数值。

## 四、方向与增长（决策与扩张）

- [pivot-or-persevere](../skills/pivot-or-persevere/SKILL.md) — **转型还是坚持**：方向性裁决的机器——常规转型会议、十种转型类型、跑道=剩余转型次数、拖延转型的三大原因。
- [growth-engine-selection](../skills/growth-engine-selection/SKILL.md) — **增长引擎的选择与运营**：黏着式（流失率/复合率）、病毒式（病毒系数）、付费式（LTV/CPA）三引擎判据、可持续增长四来源、一次只专注一种引擎。

## 五、加速与组织（"加速"篇：规模化后仍跑得快）

- [small-batch-acceleration](../skills/small-batch-acceleration/SKILL.md) — **小批量加速**：用精益生产工具（单件流、SMED、看板四阶段、持续部署、产品免疫系统）压缩循环总时间；要义是更快学习，不是高效生产。
- [five-whys-adaptive-org](../skills/five-whys-adaptive-org/SKILL.md) — **五个为什么与自适应组织**：连问五次"为什么"追到人的问题、按比例投入、五大罪状陷阱与自动速度调节器。
- [internal-innovation-sandbox](../skills/internal-innovation-sandbox/SKILL.md) — **内部创新沙盒**：大企业创新机制设计——三种架构特征、反向框定、沙盒七规则、管理组合四阶段与"创业企业家"头衔。

---

## 引用关系汇总

以下内容摘自各 SKILL.md frontmatter 之后的"相关 skills"段（depends-on / contrasts-with / composes-with），均为真实存在的 skill 引用。

| Skill | depends-on（依赖） | contrasts-with（对照/张力） | composes-with（组合使用） |
|---|---|---|---|
| lean-startup-five-principles | 无（全体系入口） | — | 其余全部 12 个 skill |
| bml-validated-learning | lean-startup-five-principles | anti-waste-discipline | leap-of-faith-assumptions、mvp-design-patterns、innovation-accounting、actionable-vs-vanity-metrics、pivot-or-persevere、small-batch-acceleration |
| leap-of-faith-assumptions | lean-startup-five-principles | growth-engine-selection | bml-validated-learning、mvp-design-patterns、innovation-accounting |
| mvp-design-patterns | leap-of-faith-assumptions | pivot-or-persevere | bml-validated-learning、actionable-vs-vanity-metrics、innovation-accounting、startup-quality-philosophy、lean-startup-five-principles |
| innovation-accounting | bml-validated-learning | anti-waste-discipline | mvp-design-patterns、actionable-vs-vanity-metrics、pivot-or-persevere、internal-innovation-sandbox |
| actionable-vs-vanity-metrics | innovation-accounting | anti-waste-discipline | bml-validated-learning、pivot-or-persevere、growth-engine-selection、internal-innovation-sandbox |
| pivot-or-persevere | innovation-accounting、actionable-vs-vanity-metrics | bml-validated-learning | leap-of-faith-assumptions、growth-engine-selection、lean-startup-five-principles |
| growth-engine-selection | leap-of-faith-assumptions | actionable-vs-vanity-metrics、pivot-or-persevere | innovation-accounting、bml-validated-learning、lean-startup-five-principles |
| small-batch-acceleration | bml-validated-learning | startup-quality-philosophy、anti-waste-discipline | mvp-design-patterns、innovation-accounting、actionable-vs-vanity-metrics、five-whys-adaptive-org |
| five-whys-adaptive-org | small-batch-acceleration | startup-quality-philosophy | internal-innovation-sandbox、mvp-design-patterns、anti-waste-discipline |
| startup-quality-philosophy | leap-of-faith-assumptions | mvp-design-patterns、small-batch-acceleration | five-whys-adaptive-org、pivot-or-persevere、bml-validated-learning |
| internal-innovation-sandbox | lean-startup-five-principles | anti-waste-discipline | bml-validated-learning、mvp-design-patterns、innovation-accounting、actionable-vs-vanity-metrics、five-whys-adaptive-org、pivot-or-persevere |
| anti-waste-discipline | —（stands-above：全部执行 skill） | bml-validated-learning | lean-startup-five-principles、innovation-accounting、pivot-or-persevere、small-batch-acceleration |

**引用结构速读**：五个 skill 以 lean-startup-five-principles 为 depends-on 根；衡量组（innovation-accounting → actionable-vs-vanity-metrics）构成决策组（pivot-or-persevere）的数据上游；small-batch-acceleration → five-whys-adaptive-org 构成加速链条；anti-waste-discipline 与多个执行 skill 形成 contrasts-with（"该不该做"与"怎么做"的元/执行张力），并 stands-above 全部执行 skill。

---
*本索引与 GLOSSARY.md、DIGEST.md 同为阶段 3 链接器产出；术语表见 [GLOSSARY.md](GLOSSARY.md)，全书执行摘要见 [DIGEST.md](DIGEST.md)。*
