# test-results — foreshadow-payoff-homecoming

- **测试方式**: fallback（主流程自测）。

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ 通过 | "说不出哪里变了+结业设计"= 回到起点路径（B 路径）原题，V2 推演即此 |
| should-trigger-02 | 激活 | ✅ 通过 | "让人会后忍不住讨论"= 伏笔的转述冲动（喂养叙述本能） |
| should-trigger-03 | 激活 | ✅ 通过 | "开头放看不懂的、结尾有意义"= 伏笔路径（A 路径）逐字命中，E 段硬条件（当时必须看似另有用途）可用 |
| should-not-trigger-01 | 不激活 | ✅ 通过 | 安全须知=必须即时明确的信息，B 段明写不适用 |
| cross-decoy-01 | 转兄弟 skill | ✅ 通过 | "每天回来补全/集齐"= 过程粘性 → gap-collection-engine；"过程空缺 vs 终点揭示"分界在两个 A2 区分段双向写明 |
| edge-01 | 边界回答 | ✅ 通过 | 短视频无时间差，B 段明写"一次性短内容不适用"——判定为不值得，给出替代方向 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 gap-collection-engine 的"中途/终点"分界经正反用例验证。
