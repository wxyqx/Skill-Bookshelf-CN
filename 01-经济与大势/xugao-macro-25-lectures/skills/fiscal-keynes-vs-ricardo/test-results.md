# test-results — fiscal-keynes-vs-ricardo（财政政策：凯恩斯 vs 李嘉图（产能闲置度裁决仪））

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
乘数取值题与 edge 题重复，lure 改写为公司财务题后通过；乘数 edge 保留（拒绝点估计）。
