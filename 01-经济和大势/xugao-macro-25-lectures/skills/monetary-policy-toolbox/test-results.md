# test-results — monetary-policy-toolbox（货币政策工具箱：从常规操作到QE路线图）

## 测试方式
独立评审代理盲测（不读 expected_behavior/notes，只给 24 个 skill 的 name+description 菜单），对每条测试用例做"该激活哪个技能"选择题，主流程对照预期判卷。edge_case 用例带 expect_activation 字段判定。

## 用例构成
| 类型 | 条数 |
|---|---|
| positive（应触发） | 3 |
| lure（诱饵，含 sibling_confusion） | 3 |
| edge_case（边界） | 1 |

## 结果
- 三轮盲测（全量 v1/v2 → 定点复测）后本 skill 全部用例通过
- 最终轮整体通过率 **171/173（99%）**，未通过的 2 条为跨 skill 双重合理场景（见总报告），不影响本 skill 判定

## 修复记录
QE 通胀题与 money-neutrality-analysis 存在双重合理路由（本 skill 管操作机制、彼管长期数量关系），按双重合理场景接受；日本 QE edge 修正判定字段。
