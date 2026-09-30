# test-results — gap-collection-engine

- **测试方式**: fallback（主流程自测）。

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ 通过 | "知识库没人贡献"是 V2 推演原题（先整体图鉴再露空缺）；description 关键信号"图鉴/空缺"命中 |
| should-trigger-02 | 激活 | ✅ 通过 | "'规定写三页'越来越抗拒"= 命令式重复的反例（广播体操原理），改空缺+节奏 |
| should-trigger-03 | 激活 | ✅ 通过 | "积分徽章总觉得不对"= 先整体后空缺 vs PBL 的核心分界，V3 与 I 段直接覆盖 |
| should-not-trigger-01 | 不激活 | ✅ 通过 | 单次表单填写=一次性任务，无重复无收集——description 明写"无重复需求的一次性任务不适用" |
| cross-decoy-01 | 转兄弟 skill | ✅ 通过 | "两种计划自己挑+反馈设计"= 选择和斟酌 → risk-reward-choice-feedback；成长两主题的分界清晰 |
| edge-01 | 激活+红线 | ✅ 通过 | "电商停不下来"命中 B 段"把'停不下来'用在有害行为上"红线——判定为拒绝该用法并说明前提；此红线应转 stop-design-graceful-endings 的立场审计 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 三个成长主题间的分界（收集/选项/共鸣）经正反用例验证；成瘾红线用例验证 B 段有效。
