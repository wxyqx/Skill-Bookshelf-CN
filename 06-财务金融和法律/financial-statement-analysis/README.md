# 财务报表分析(简明版·立体化数字教材版)

由张新民、钱爱民《财务报表分析(简明版·立体化数字教材版)》(*Financial Statement Analysis*)蒸馏出的一组**可被 AI Agent 调用的技能**(Skills)。

> 看财务报表不能只看规模和比率,要把每张表、每个项目还原成**质量**和**战略**问题——资产有没有实际效用、利润是不是真金白银、资本结构在支持还是拖累企业——从而从公开报表反推出管理质量与企业质地。18 个原子化技能覆盖从审计意见入口、逐项资产质量、核心利润与获现率,到差量分析法、四步综合路径与造假手法识别的完整链条。

---

## 来源

| | |
|---|---|
| **书名** | 财务报表分析(简明版·立体化数字教材版) |
| **作者** | 张新民(对外经济贸易大学,"财务状况质量分析理论"创立者)、钱爱民 |
| **出版** | 中国人民大学出版社(教育部经济管理类核心课程教材);贯穿案例为北陆药业 2019 年报 |
| **蒸馏工具** | cangjie-skill(仓颉:把长内容蒸馏成可调用技能的流水线) |
| **蒸馏方法** | RIA-TV++(整书理解 → 并行提取 → 三重验证 → RIA++ 构造 → 链接 → 压力测试 → 交付) |
| **文本来源** | PDF(292 页,文本层完整)直接提取全文后蒸馏 |

---

## 18 个技能

**总纲与入口**
- [`strategic-analysis-path`](skills/strategic-analysis-path/SKILL.md) — **战略视角综合分析路径**:拿到一份年报的四步标准作业流程(背景→会计→战略→前景),北陆药业全程演练
- [`project-quality-entry`](skills/project-quality-entry/SKILL.md) — **项目质量分析总纲**:按重要性/例外原则圈定重大与异动项目,以审计意见+附注开路

**资产与负债质量**
- [`cash-quality-funding-risk`](skills/cash-quality-funding-risk/SKILL.md) — **货币资金与获现率**:受限资金自由度、存贷双高三解释、核心利润获现率五类归因、短贷长投
- [`receivables-and-funneling`](skills/receivables-and-funneling/SKILL.md) — **商业债权与资金占用**:应收三步、债务人六维、关联预付输送警报与集权例外
- [`inventory-and-margin`](skills/inventory-and-margin/SKILL.md) — **存货与毛利率**:构成比例译码、毛利率高低归因清单、"波动即证据"
- [`long-term-asset-quality`](skills/long-term-asset-quality/SKILL.md) — **长期资产与减值**:长投泡沫、在建不决算三重好处、"账内皆外购"、减值不得转回

**战略透视**
- [`asset-allocation-strategy`](skills/asset-allocation-strategy/SKILL.md) — **资源配置战略**:经营性/投资性重分类与经营主导/投资主导/并重三分类
- [`capital-structure-four-forces`](skills/capital-structure-four-forces/SKILL.md) — **资本结构与四大动力**:强制性分层、输血/盈利二分、五关注、资本引入战略五型

**利润与现金验证**
- [`profit-quality-3d`](skills/profit-quality-3d/SKILL.md) — **利润质量三维**:核心利润口径、含金量/持续性/战略吻合性、扭亏必须双重翻转
- [`revenue-quality-three-questions`](skills/revenue-quality-three-questions/SKILL.md) — **收入质量三问**:卖什么/卖给谁/靠什么
- [`non-operating-income-quality`](skills/non-operating-income-quality/SKILL.md) — **非经营性损益**:投资收益三分法、浮盈监管盲区、政府补助四要点
- [`cash-flow-three-activities`](skills/cash-flow-three-activities/SKILL.md) — **现金流量三性**:禁止符号化判断、经营三性、投资看战略吻合、筹资看主动还是被迫

**集团与比率工具**
- [`consolidation-pitfalls`](skills/consolidation-pitfalls/SKILL.md) — **合并报表陷阱**:混合物原理、真金白银决策回母公司报表、比率三大失真
- [`differential-analysis`](skills/differential-analysis/SKILL.md) — **差量分析法**:"越合并越小"双向差额、撬动倍数、两种"三高"、母子业务三模式
- [`ratio-revision-rules`](skills/ratio-revision-rules/SKILL.md) — **比率修正纪律**:OPM 低流动比率悖论、利息保障倍数失灵、原值口径、预收偿付修正

**风险扫雷**
- [`earnings-manipulation-tactics`](skills/earnings-manipulation-tactics/SKILL.md) — **造假手法十法**:虚构收入消化路径、低转成本、资产端造假、账龄洗短等,各配核查动作
- [`profit-deterioration-sweep`](skills/profit-deterioration-sweep/SKILL.md) — **恶化扫雷**:12 种恶化外在表现四组分级、洗大澡两阶段剧本、扭亏成色双检
- [`off-statement-strategy-blindspots`](skills/off-statement-strategy-blindspots/SKILL.md) — **报表外盲区**:治理失效使分析前提失效的终止条件、多元化并购的关联度机制链

---

## 常见问题 → 对应技能

| 你的问题 | 用哪个 |
|---|---|
| 拿到一份年报,整体分析这家公司 | `strategic-analysis-path` |
| 它账上那么多钱,是真的吗 | `cash-quality-funding-risk` |
| 应收账款突然翻倍,正常吗 | `receivables-and-funneling` |
| 毛利率比同行高一大截,可信吗 | `inventory-and-margin` |
| 商誉/在建工程/固定资产怎么查 | `long-term-asset-quality` |
| 高负债率就是高风险吗 | `capital-structure-four-forces` |
| 净利润大增,该高兴吗 | `profit-quality-3d` |
| 政府补贴算真利润吗 | `non-operating-income-quality` |
| 经营现金流是正是负怎么看 | `cash-flow-three-activities` |
| 母公司和合并报表该用哪套 | `consolidation-pitfalls` / `differential-analysis` |
| 这个比率跟教科书标准矛盾 | `ratio-revision-rules` |
| 怀疑它造假,怎么逐项排查 | `earnings-manipulation-tactics` |
| 扭亏为盈,明年会不会变脸 | `profit-deterioration-sweep` |
| 实控人出事了,报表还能信吗 | `off-statement-strategy-blindspots` |

---

## 安装

每个技能目录都包含 `SKILL.md`(+ `test-prompts.json` / `test-results.md` 测试产物),可直接复制到宿主环境:

```bash
# Claude Code(用户级,所有项目可用)
cp -r skills/* ~/.claude/skills/

# 或 Claude Code(项目级)
cp -r skills/* <project>/.claude/skills/

# Trae(项目级)
cp -r skills/* <project>/.trae/skills/

# Cursor(项目级)
cp -r skills/* <project>/.cursor/skills/
```

---

## 完整文档

`docs/` 目录保留了完整的蒸馏产物与审计轨迹:

| 文件 | 说明 |
|---|---|
| [`DIGEST.md`](docs/DIGEST.md) | 面向读者的精华长文(约 8000 字,不读全书看这篇) |
| [`GLOSSARY.md`](docs/GLOSSARY.md) | 共享术语词典(47 个核心术语,作者本人用法) |
| [`INDEX.md`](docs/INDEX.md) | 技能总览 + 引用图 + 推荐学习顺序 |
| [`BOOK_OVERVIEW.md`](docs/BOOK_OVERVIEW.md) | 整书理解(结构/解释/批判/应用潜力) |
| [`verified.md`](docs/verified.md) | 三重验证结果(144 条候选 → 81 单元 → 18 技能) |
| [`verified-A.md`](docs/verified-A.md) / [`verified-B.md`](docs/verified-B.md) | V1/V2/V3 逐条判定记录 |
| [`PIPELINE_STATE.md`](docs/PIPELINE_STATE.md) | 流水线各阶段状态 |
| [`candidates/`](docs/candidates/) | 5 个提取组的原始候选池(224 条) |
| [`rejected/`](docs/rejected/) | 未通过验证的候选及原因 |

---

## 目录结构

```text
financial-statement-analysis/
├── README.md
├── skills/                      # 18 个可安装技能(核心交付物)
│   └── <skill-slug>/
│       ├── SKILL.md             # 技能定义(R/I/A1/A2/E/B 六段)
│       ├── test-prompts.json    # 触发/诱饵测试集
│       └── test-results.md      # 盲测结果
└── docs/                        # 蒸馏文档与审计轨迹
    ├── DIGEST.md / GLOSSARY.md / INDEX.md
    ├── BOOK_OVERVIEW.md / verified.md / PIPELINE_STATE.md
    └── candidates/              # 5 组提取候选池(框架/原则/案例/反例/术语)
```

---

## 关于内容与版权

本项目是**方法论蒸馏产物**,不含原书全文:

- 原书 PDF 的提取文本仅用于本地蒸馏,**不随本仓库分发、不长期留存**;
- 每个技能对原书的引用严格控制在**≤60 字/处**,属于评论与教学方法论范畴;
- 原文的版权归原作者张新民、钱爱民及中国人民大学出版社所有;
- 建议购买正版书籍配合使用。

---

## 如何重新生成

本项目由 cangjie-skill(仓颉蒸馏流水线)自动生成。若要复现或调整:

1. 准备书籍文本(PDF 文本层直接提取 → 按章切分,PDF 页 = 书页 + 16)
2. 运行 RIA-TV++ 流水线(阶段 0–5,详见 `docs/PIPELINE_STATE.md`)
3. 通过三重验证(144 条候选 → 81 单元)+ 集中盲测(111/111,含全部同书混淆诱饵)的 18 个技能被构造为独立技能

如需让技能持续进化,可喂给 `darwin-skill`:`darwin evolve financial-statement-analysis/`
