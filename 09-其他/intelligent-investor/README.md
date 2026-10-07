# 聪明的投资者：安全边际与投资纪律

由本杰明·格雷厄姆《聪明的投资者》（*The Intelligent Investor*，第 4 版老译本，数据截至 1964 年）蒸馏出的一组**可被 AI Agent 调用的技能**（Skills）。

> 投资的成败不取决于智力或预测，而取决于以"安全边际"（价格与价值之间经统计可证明的足够顺差）为核心的态度与纪律——普通投资者把抱负限于能力之内、活动限于安全的狭窄范围，就能用最小的努力取得可信的结果。20 个技能覆盖从投资/投机过筛与防御/进攻身份判定，到市场波动纪律与过热防守，再到选股、估值、廉价证券与套利，最后收束于安全边际与建议纪律的完整决策链。

---

## 来源

| | |
|---|---|
| **书名** | 聪明的投资者（The Intelligent Investor） |
| **作者** | 本杰明·格雷厄姆（Benjamin Graham，"价值投资之父"） |
| **出版** | 第 4 版 1965；本 EPUB 为 16 章 4 篇老译本，无 Zweig 点评 |
| **蒸馏工具** | cangjie-skill（仓颉：把长内容蒸馏成可调用技能的流水线） |
| **蒸馏方法** | RIA-TV++：EPUB 提取约 17.4 万字（16 章+卷首）；原始候选 244 条 → 三重验证 51 单元通过 → 聚类 20 个 skill |
| **质量验证** | 集中盲测 180 题：should_trigger 60/60、should_not_trigger 45/45、兄弟诱饵 59 条 0 跷跷板；2 对触发冲突按跷跷板法修复并干净复测 18/18；详见 [docs/TEST_RESULTS.md](docs/TEST_RESULTS.md) |

> **时效提示：本包基于 1964 年数据版本，所有估值参数/绝对门槛（覆盖倍数、PE 上限、2/3 折扣线等）按当期重查，禁止机械照抄（各 skill B 段已内嵌警示）。**

---

## 20 个技能

**投资哲学与身份**
- [`invest-vs-speculation-filter`](skills/invest-vs-speculation-filter/SKILL.md) — **投资/投机过筛**：三判据（全面分析/本金安全/满意回报）逐条过筛任何一笔操作，附投机三非理性检验与专款隔离处置。
- [`investor-identity-matching`](skills/investor-identity-matching/SKILL.md) — **投资者身份匹配**：防御/进攻二分定身份：回报与明智努力相称律、无中间立场（折衷最可能产生失望）、先定努力预算再定收益预期。

**市场波动与纪律**
- [`rule-reliability-trend-skepticism`](skills/rule-reliability-trend-skepticism/SKILL.md) — **准则可靠性与趋势怀疑**：判别一条准则/因子/趋势还能否依赖：类型挂钩 vs 人性挂钩的分类检验、流行即失效定律、趋势逆转 2:1。
- [`market-mr-volatility-discipline`](skills/market-mr-volatility-discipline/SKILL.md) — **市场先生波动纪律**：把市场当仆人不当向导：波动二义、1/3 检视阈值、浮盈不可兑现律、风险三来源重定义（风险≠波动）。
- [`overheated-market-defense`](skills/overheated-market-defense/SKILL.md) — **过热市场防守**：牛市顶部信号逐条打分（五特征/六条件/新股倒挂）＋谨慎三准则，输出警惕等级而非崩盘预测。

**组合策略**
- [`mechanical-allocation-dca`](skills/mechanical-allocation-dca/SKILL.md) — **机械配置与定投**：25–75 股债比例带与 50:50±5%→调 1/11 的机械再平衡，定投去留与"有资金即可买入"原则。
- [`defensive-stock-selection`](skills/defensive-stock-selection/SKILL.md) — **防御型选股**：防御型选股四原则（10–30 只、大而突出、连续红利、25×/20× 价格上限）与全取样/排除法/低倍数法三路径。
- [`aggressive-negative-list`](skills/aggressive-negative-list/SKILL.md) — **进攻型负面清单**：进攻型先做减法：四不碰负面清单、收益换本金检验、2/3 账面值折扣线是唯一例外通道。
- [`excess-return-path-selection`](skills/excess-return-path-selection/SKILL.md) — **超额收益路径选择**：超额收益从哪来：差异化公理→五路排除→冷门大公司/廉价证券/特别情况三域按气质三选一。

**证券选择与估值**
- [`stock-diagnosis-techniques`](skills/stock-diagnosis-techniques/SKILL.md) — **个股诊断技术**：报表还原四件套、股价-收益四模式地图、高增长公司三查预警——只还原真相，不做买卖判断。
- [`earnings-power-valuation`](skills/earnings-power-valuation/SKILL.md) — **盈利能力估值**：盈利能力（跨好差年景均值）×资本化率五因素：评估价须超市价 1/3、投资/投机成分分解、繁荣≠安全。
- [`growth-stock-appraisal`](skills/growth-stock-appraisal/SKILL.md) — **成长股评估**：8.5+2g 正算与隐含增长率反解：前景几乎必然已在价中、进攻型 20 倍参与上限、防御型整体回避。
- [`neglected-large-cap-strategy`](skills/neglected-large-cap-strategy/SKILL.md) — **冷门大公司策略**：失宠大公司低倍数法：Drexel 26 项年度调查、6–10 种持 1–5 年、为何明确拒绝同型小公司。
- [`bargain-issues-net-nets`](skills/bargain-issues-net-nets/SKILL.md) — **廉价证券与净流动资产**：廉价证券定义与发现双法、净流动资产 2/3 折扣（为厂房机器商誉付零价）、成组购买不按单笔止损。
- [`special-situations-arbitrage`](skills/special-situations-arbitrage/SKILL.md) — **特别情况套利**：兼并清算重组中利润可预先计算的事件价差：时间风险定价、"决不买进一场诉讼"偏见反用。

**保护主义与安全边际**
- [`bond-safety-terms`](skills/bond-safety-terms/SKILL.md) — **债券安全检验**：债券安全双标准检验（类别覆盖倍数门槛＋最差年）与可赎回条款"我得头你失尾"的结构性规避。
- [`protection-over-forecast`](skills/protection-over-forecast/SKILL.md) — **预言法与保护法**：预言法/保护法二分：定量优先的认识论、数学化-准确性反比定律、集合预测优于个别预测、技巧中和定律。
- [`margin-of-safety-core`](skills/margin-of-safety-core/SKILL.md) — **安全边际核心**：全书收束：安全边际三领域量化（债券覆盖/普通股盈利超额/议价 2/3）、可证明性试金石、保险同构多样化。

**治理与建议纪律**
- [`shareholder-governance`](skills/shareholder-governance/SKILL.md) — **股东治理质询**：所有者思维：管理低效三信号、内外股东利益结构性背离、公平回购与接管正当性、股利政策举证二分。
- [`investment-advice-discipline`](skills/investment-advice-discipline/SKILL.md) — **投资建议使用纪律**：外部建议使用双条件：卖方利益结构审视、小费免疫、提问重构（问内在价值，不问下月涨跌）。

---

## 测试

每技能目录内含 `test-prompts.json`（should-trigger / should-not-trigger（含同书兄弟混淆诱饵）/ edge-case）与 `test-results.md`（集中盲测逐例记录）。

## docs

- [docs/BOOK_OVERVIEW.md](docs/BOOK_OVERVIEW.md) — 阶段 0 整书理解
- [docs/DIGEST.md](docs/DIGEST.md) — 面向读者的精华长文（不读全书看这篇）
- [docs/INDEX.md](docs/INDEX.md) — 技能总览、引用图与推荐学习顺序
- [docs/GLOSSARY.md](docs/GLOSSARY.md) — 共享术语词典
- [docs/TEST_RESULTS.md](docs/TEST_RESULTS.md) — 集中盲测报告（180 题，should 类全绿，冲突修复复测通过）
- [docs/verified.md](docs/verified.md) — 三重验证逐条判定（51 单元＋聚类总表＋时效警示）
- [docs/stage0-chapter-notes.md](docs/stage0-chapter-notes.md) — 卷首+16 章四组精读笔记
- [docs/candidates/](docs/candidates/) — 去重后候选池 · [docs/rejected/](docs/rejected/) — 淘汰记录 · [docs/PIPELINE_STATE.md](docs/PIPELINE_STATE.md) — 流水线状态
