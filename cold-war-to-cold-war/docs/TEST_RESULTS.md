# TEST_RESULTS — 《从"老冷战"到"新冷战"》阶段 4 压力测试结果

> 测试方式：以各 skill 的 description 与 E 段为基准，对 test-prompts.json 全部 54 条用例（9 skill × 6 条）做触发判定盲测；诱饵容错为 0。

## 总体结果

- **9 / 9 skill 通过**（minimum_pass_rate = 0.8，实际全部 100%）
- should_trigger：27 条全部通过
- should_not_trigger：18 条全部通过（含 9 条兄弟混淆诱饵，全部正确指向）
- edge_case：9 条均给出判定理由

## 兄弟混淆诱饵一览（9 条，全部通过）

| 本 skill | 混淆场景 | 正确指向 |
|---|---|---|
| globalization-stage-analysis | "民主对抗威权"叙事的服务对象 | ideology-softpower-analysis |
| financial-exclusion-mechanism | 对美元体系的依附程度评估 | re-dependency-analysis（跨书） |
| industrial-transfer-fate | 外资突然撤离会怎样 | foreign-capital-dependency-risk（跨书） |
| monetization-sovereignty | 政府债务超 GDP 会出事吗 | sovereign-currency-discipline（跨书） |
| crisis-harvesting-mechanism | 渐进货币化为何比休克疗法安全 | monetization-sovereignty（同书） |
| currency-bloc-competition | 人民币国际化的推进路径 | rmb-internationalization-five-pools（跨书） |
| demand-engine-structure | 政府债务对应资产还是消费 | state-asset-monetization（同书） |
| state-asset-monetization | 财政赤字货币化的红线 | sovereign-currency-discipline（跨书） |
| ideology-softpower-analysis | 欧元为何被视为美元挑战 | currency-bloc-competition（同书） |

跨书诱饵集中检验了温铁军卷与黄奇帆卷的边界（机制解剖 vs 纪律红线、对抗分析 vs 建设路径），全部通过。

## 边界用例需关注的 2 处

1. `re-dependency-analysis` edge"三个无解难题为什么说无解"——书内 example 直接询问，合法调用并须标注框架边界（宣言式断言的局限）。
2. `currency-bloc-competition` 与 `ideology-softpower-analysis` 在"话语与货币"上真实相邻——话语权是竞争链第一环，两 skill 可先后调用；description 已按"货币利益归因 vs 话语机制"分工。

## 回炉记录

无需回炉。全部 SKILL.md 满足质量红线（六段完整、引用 ≤150 字、description 含 trigger 与不适用场景）。
