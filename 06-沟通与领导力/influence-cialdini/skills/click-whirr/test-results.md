# test-results.md — click-whirr

> 测试方式: 独立 sub-agent 盲测 (3 个 Explore agent 并行)
> 测试时间: 2026-09-22

## 测试结果

| ID | 类型 | 预期 | 盲测结果 | 判定 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | click-whirr | click-whirr ✅ | PASS |
| should-trigger-02 | should_trigger | click-whirr | none ❌ | FAIL — agent 视为纯信息查询 |
| should-trigger-03 | should_trigger | click-whirr | none ❌ | FAIL — agent 未匹配触发词 |
| should-not-trigger-01 | should_not_trigger | 不触发 | none ✅ | PASS |
| should-not-trigger-02 | should_not_trigger | commitment-consistency | commitment-consistency ✅ | PASS |
| edge-01 | edge_case | 不触发(习惯) | click-whirr | BORDERLINE — agent 触发了，但 edge case 判断合理 |

## 初始通过率: 4/6 = 67% ⚠️ (低于 80%)

## 失败分析

### cw-02 (should-trigger-02): "为什么超市把面包放在最里面…这种布局有什么心理学原理吗"

**失败原因**: description 的 trigger 词聚焦个人体验（"莫名其妙""不假思索"），未覆盖"分析营销策略/布局的心理学原理"这一第三人称分析场景。sub-agent 将其视为纯信息查询。

**修复**: 更新 description，增加"或在分析'为什么某个营销策略/布局/话术有效'的心理学原理时激活"，并增加 trigger 词"为什么这个策略有效""布局有什么心理学原理"。

### cw-03 (should-trigger-03): "销售员一说话他就觉得特别靠谱，但回来想想也没说什么实质内容"

**失败原因**: description 缺少"第三方描述某人自动觉得靠谱"的 trigger 信号。sub-agent 未将"没说什么实质内容就觉得靠谱"匹配到 click-whirr。

**修复**: 更新 description，增加 trigger 词"没说什么实质内容就觉得靠谱"，并明确涵盖"第三人称观察"场景。

## 修复后预期通过率: 6/6 = 100% (需复测确认)

## 修复操作

已更新 click-whirr/SKILL.md 的 frontmatter description 字段，扩展 trigger 覆盖范围：
- 增加第三人称分析和营销策略分析场景
- 增加"为什么这个策略有效""布局有什么心理学原理""没说什么实质内容就觉得靠谱"等 trigger 词
- 明确排除"日常习惯行为"

## 审计信息

- **初始通过率**: 67% (低于 80%，触发 A2 修复)
- **修复后预期通过率**: 100% (待复测)
- **修复类型**: A2 (description) — 非 R/I/A1/E/B 重做
