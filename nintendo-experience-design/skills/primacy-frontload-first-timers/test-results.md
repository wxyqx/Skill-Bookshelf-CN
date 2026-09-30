# test-results — primacy-frontload-first-timers

- **测试方式**: fallback（主流程自测）。

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ 通过 | "平均铺开科学吗"正是 ce09 反例的原题；V2 推演场景即此 |
| should-trigger-02 | 激活 | ✅ 通过 | "砍教程 vs 新用户需要"命中规则二+E5 跳过口 |
| should-trigger-03 | 激活 | ✅ 通过 | "资深用户功能 vs 上手流程"是 ce34 开发者偏差的 roadmap 版 |
| should-not-trigger-01 | 不激活 | ✅ 通过 | 遗忘曲线复习属间隔效应——B 段明写"间隔复习场景不适用"，正确拒答并提示区分初学/巩固 |
| cross-decoy-01 | 转兄弟 skill | ✅ 通过 | "内容已前置但学了挫败"=微循环设计问题（10秒确认/成功率）→ intuition-design-loop。分界清晰：何时教（本 skill）vs 怎么教会（那个） |
| edge-01 | 边界回答 | ✅ 通过 | 受众全熟练者→规则失效，B 段直接覆盖 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与间隔效应的区分（初学 vs 巩固）是最易混点，用例验证 B 段可守住。
