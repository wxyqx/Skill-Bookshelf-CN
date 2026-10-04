# TEST_RESULTS — 阶段 4 压力测试结果

> 测试方式：以各 skill 的 description（触发条件）与 E 段（执行步骤）为基准，对 test-prompts.json 全部 114 条用例（19 skill × 6 条）做触发判定盲测；诱饵（should_not_trigger）容错为 0。
> 全自动模式下由流水线执行盲测并记录；每条用例的判定理由在 JSON 的 notes 字段。

## 总体结果

- **19 / 19 skill 通过**（minimum_pass_rate = 0.8，实际全部 100%）
- should_trigger：57 条，通过 57 条（各 skill 的 3 条正面场景均命中 description 中的语言信号）
- should_not_trigger：38 条，通过 38 条（含 19 条同书兄弟 skill 混淆诱饵，全部正确指向兄弟 skill）
- edge_case：19 条，全部给出明确判定理由

## 兄弟混淆诱饵一览（19 条，全部通过）

| 本 skill | 混淆诱饵场景 | 正确指向 |
|---|---|---|
| five-step-structural-analysis | 咖啡连锁关店潮是周期还是拐点 | boundary-condition-analysis |
| boundary-condition-analysis | 杭州房子值不值得长期持有 | city-land-structure |
| war-game-scenario-analysis | 数据库自研还是采购 | self-reliance-boundary |
| first-build-then-demolish | 钠电池补贴退坡还能活吗 | relative-cost-judgment |
| origin-sale-vs-local-production | 产业为何向大市场集聚 | scale-market-three-effects |
| chain-power-analysis | 工厂留中国还是迁墨西哥 | origin-sale-vs-local-production |
| scale-market-three-effects | 我们在链上有没有话语权 | chain-power-analysis |
| data-rights-layering | 数据造假屡禁不止怎么治 | source-governance-thinking |
| snowball-alliance-strategy | 被断供环节是否全自研 | self-reliance-boundary |
| institutional-gene-analysis | 这个城市的房子还能不能买 | city-land-structure |
| long-cycle-constants-filter | 煤炭是周期回暖还是结构拐点 | boundary-condition-analysis |
| source-governance-thinking | 系统分析养老产业机会 | five-step-structural-analysis |
| innovation-three-stages | 用户数据能不能变现 | data-rights-layering |
| first-allocation-order | 报销舞弊屡禁不止 | source-governance-thinking |
| manufacturing-share-diagnosis | 大市场为何能摊薄成本 | scale-market-three-effects |
| self-reliance-boundary | 断供 EDA 会怎样 | war-game-scenario-analysis |
| relative-cost-judgment | 迁移节奏怎么排 | first-build-then-demolish |
| financial-opening-sequencing | 香港金融中心靠什么制度 | institutional-gene-analysis |
| city-land-structure | 全国楼市是不是到拐点了 | boundary-condition-analysis |

## 边界用例需关注的 3 处

1. `long-cycle-constants-filter` edge"这次是不是不一样了"——与 boundary-condition-analysis 存在真实灰区：若用户追问"当前处于什么阶段"应转切边界条件法；description 已写明"方向感 vs 阶段判断"的分工，测试通过但属调用时需继续甄别的场景。
2. `self-reliance-boundary` edge"怎么降低IT运维成本"——不触发判定依赖"自主可控"语境缺失；若用户在成本优化中引出"外包 vs 自建"，可能误激活，建议宿主在执行时先做一问确认。
3. `city-land-structure` edge"这个小区的学校好不好？"——学区属配套信息查询，与标尺分析无关；判定不触发正确，但若用户后续追问"学区房值不值"需转入标的级分析而非城市级标尺。

## 回炉记录

无需回炉的 skill。全部 SKILL.md 在构造阶段已满足质量红线（六段完整、引用 ≤150 字、description 含 trigger 与不适用场景）。
