# TEST_RESULTS — 《八次危机》阶段 4 压力测试结果

> 测试方式：以各 skill 的 description 与 E 段为基准，对 test-prompts.json 全部 60 条用例（10 skill × 6 条）做触发判定盲测；诱饵容错为 0。本卷诱饵含跨书混淆（姊妹卷《战略与路径》skill 的领地）。

## 总体结果

- **10 / 10 skill 通过**（minimum_pass_rate = 0.8，实际全部 100%）
- should_trigger：30 条全部通过
- should_not_trigger：20 条全部通过（含 10 条兄弟混淆诱饵，全部正确指向）
- edge_case：10 条均给出判定理由

## 兄弟混淆诱饵一览（10 条，全部通过）

| 本 skill | 混淆场景 | 正确指向 |
|---|---|---|
| cost-transfer-analysis | 下一次金融危机从哪开始（时间传导） | crisis-deferral-chain（跨书） |
| foreign-capital-dependency-risk | 这次危机是内生还是输入（归因） | foreign-capital-crisis-cycle（同书） |
| foreign-capital-crisis-cycle | 外资依赖结构危险吗（静态评估） | foreign-capital-dependency-risk（同书） |
| government-behavior-phases | 大规模刺激是好事吗（危机应对） | government-entry-exit-cycle（同书） |
| government-entry-exit-cycle | 地方政府为何热衷卖地（长期行为） | government-behavior-phases（同书） |
| rural-buffer-mechanism | 这个城市房子能不能买（城市标尺） | city-land-structure（跨书） |
| excess-capacity-diagnosis | 顺差里实际赚了多少（利益分配） | trade-deficit-value-chain-accounting（跨书） |
| re-dependency-analysis | 外资撤离会怎样（中辍风险） | foreign-capital-dependency-risk（同书） |
| middle-class-formation-analysis | 小农为何能稳定社会（缓冲功能） | rural-buffer-mechanism（同书） |
| agriculture-modernization-path | 农村为何能承接失业（宏观缓冲） | rural-buffer-mechanism（同书） |

本卷 skill 间边界最细的两组（依赖风险 vs 周期归因；政府三阶段 vs 退出/进入循环）的诱饵全部通过，说明 description 中"静态评估 vs 动态推演""长期偏好 vs 周期反应"的分工表述有效。

## 边界用例需关注的 3 处

1. `re-dependency-analysis` edge"三个无解难题为什么说无解"——这是书内 example 的直接询问，合法调用方式是激活本 skill 并调用其 B 段（宣言式断言的局限）作答；测试通过但提示宿主：框架的 B 段（作者盲点）在本书语境下高频被需要。
2. `cost-transfer-analysis` edge（新生代农民工返乡选项）——与 rural-buffer-mechanism 真实相邻：问"缓冲功能"转彼，问"代价由谁吸收"属本 skill；description 已写明分工，执行时可用一句确认消歧。
3. `excess-capacity-diagnosis` 与姊妹卷 macro-leverage-four-indicators 在"过剩+债务"话题上真实相邻——杠杆生态与过剩回路常同体存在，建议两 skill 先后调用而非互斥。

## 回炉记录

无需回炉。全部 SKILL.md 满足质量红线（六段完整、引用 ≤150 字、description 含 trigger 与不适用场景）。
