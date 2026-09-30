# test-results — fatigue-timing-management

- **测试方式**: fallback（主流程自测）。

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ 通过 | "'挺好的但坚持不下来'+中途断崖"= "想玩但很困"原话场景；description 关键信号直接命中 |
| should-trigger-02 | 激活 | ✅ 通过 | "第 4 个汇报开始冷场+提神环节放哪"= 时机问题（E2 定位饱和点），而非内容制作 |
| should-trigger-03 | 激活 | ✅ 通过 | "'腻了但还想看'"是书中矛盾状态的逐字复现 |
| should-not-trigger-01 | 不激活 | ✅ 通过 | 第一章流失=开头问题（onboarding/内容价值分诊），非中途疲劳；description 明写"中途下滑" |
| cross-decoy-01 | 转兄弟 skill | ✅ 通过 | 用户已定位时机、问"怎么设计反转"=施工问题 → surprise-design-two-beliefs。分界"诊断用我、施工用它"在两 skill 的 A2 区分段互相写明 |
| edge-01 | 激活+红线 | ✅ 通过 | B 段明写"把疲劳当变现工具"是反场景；金融语境需先分诊价值问题——边界处理符合预期 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 surprise-design-two-beliefs 的"诊断/施工"分工双向清晰（两边 A2 都写了区分段）。
