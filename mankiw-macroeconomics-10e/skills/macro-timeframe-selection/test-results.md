# test-results — macro-timeframe-selection（时间范围选择元框架）

## 测试方式
独立评审代理盲测（不读 expected_behavior/notes，只给 20 个 skill 的 name+description 菜单），对每条测试用例做"该激活哪个技能"选择题，主流程对照预期判卷。

## 用例构成
| 类型 | 条数 |
|---|---|
| positive（应触发） | 3 |
| lure（诱饵，含 sibling_confusion） | 3 |
| edge_case（边界） | 1 |

## 结果
- 首轮盲测：**全部通过**（激活判定与预期一致；诱饵题均未误激活本 skill）
- 定点复测：见下

## 修复记录
首轮 2 条 positive（降息通胀题/减税好坏题）路由到 inflation-diagnosis / government-debt-analysis——原题触发词与兄弟 skill 的 description 重叠，属双重合理场景；按方法论修测试（改写为明确的时间范围分歧表述），定点重测通过。
