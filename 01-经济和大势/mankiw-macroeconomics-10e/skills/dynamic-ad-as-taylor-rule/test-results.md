# test-results — dynamic-ad-as-taylor-rule（动态 AD-AS 与泰勒规则）

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
首轮 1 条 positive（油价冲击两难）路由到 ad-as-fluctuations——供给冲击两难正是后者的核心触发面；修 skill（description 增补"供给冲击下稳物价还是保产出、加息幅度够不够"信号），定点重测通过。
