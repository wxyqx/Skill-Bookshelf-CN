# test-results — intuition-design-loop

- **测试方式**: fallback（主流程自测）。子代理配额受限，无法独立盲测；每条用例由主流程对照全部 13 个 skill 的 frontmatter description 做"该激活哪一个"的选择题判定，重点检查跨 skill 混淆。可信度低于独立盲测，建议接入 darwin-skill 后重跑。

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ 通过 | "教程完成率低+要不要强制"命中核心反场景；description 明确含"教程没人看/强制观看"。判定动作：反问"强制解决的是看到还是学会"，给出三步微循环改法 |
| should-trigger-02 | 激活 | ✅ 通过 | "告诉他步骤转头就忘/让他自己学会"是"怎么让他们自己发现"的典型措辞 |
| should-trigger-03 | 激活 | ✅ 通过 | "边看边动手、有成就感"命中 A2 场景 1/5 |
| should-not-trigger-01 | 不激活 | ✅ 通过 | 纯信息查询，无设计诉求 |
| should-not-trigger-02 | 不激活 | ✅ 通过 | 文采润色与行动设计无关 |
| cross-decoy-01 | 不激活本 skill，应激活 fatigue-timing-management | ✅ 通过 | "前面不错+第6章断崖=中途弃坑"是疲劳节奏信号；本 skill description 的不适用清单虽未明写此例，但 A2 区分段明确写了"教程没人看→本 skill；看了一半弃坑→那个"。判定：转 fatigue-timing-management |
| edge-01 | 激活但声明边界 | ✅ 通过 | description 明确"不适用于需要严格执行的合规指令"；E 段仍可用于教学环节，考核标准必须明示——与 B 段反场景一致 |

## 结果

- **通过率: 7/7 = 100%**（fallback 自测）
- **混淆检查**: 与 fatigue-timing-management 的分界（行动设计 vs 节奏管理）在 7 组用例下无歧义。
- **建议**: 上线后用真实会话抽检 cross-decoy-01 类场景；接入 darwin-skill 独立盲测。
