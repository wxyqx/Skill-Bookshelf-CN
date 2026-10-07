# test-results — innovate-in-the-open

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我的方案被老板否了，但我还是觉得方向对，要不要拉着两个同事下班后偷偷继续做？
- **判定理由**：方案被否要不要私下继续做是 description 首要场景（影子项目），激活并给'地下是过渡态'规则。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们团队用个人网盘和微信群跑业务流程快半年了，一直没敢让 IT 部门知道，这样下去行吗？
- **判定理由**：个人网盘/微信群跑业务瞒着 IT——A2 情境 2 影子 IT 原文。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：Should we run this initiative as a skunkworks project in stealth, or innovate in the open inside the company?
- **判定理由**：英文 prompt：skunkworks stealth vs innovate in the open——description trigger 词直译。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们下一代芯片设计在流片前必须严格保密，防止竞争对手窃取，该怎么管访客和文档？
- **判定理由**：芯片流片前防竞争窃取是知识产权/商业机密管理，B 段明确排除（本 skill 只管对母体隐瞒的组织政治问题）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：项目已经决定公开试点了，接下来要跟高管谈条件：我们承诺交付什么，换他们帮我们清哪些障碍，这场谈判怎么设计？
- **判定理由**：已决定公开后的谈判设计（承诺交付换清障）是 wield-the-sword 的领域（相邻区分明示：公开之后怎么谈）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：领导说'先低调做，别声张，做出成绩我给你报上去'——这算公开创新吗？
- **判定理由**：命中 A2 情境 3（领导建议先低调做的边界）：会激活并回答——低调可作为过渡态，但必须设公开日期与汇报对象；无日期的地下即'永久地下'，按判停处理。
- **对照预期**：一致 —— 边界判断符合 `expected_behavior` 中定义的边界理由。

---

## 通过率

- 通过 **6/6**，通过率 **100%**（minimum_pass_rate = 80%）✅
- 其中 `should_not_trigger`（诱饵，容错为 0）：2/2 全部正确拒绝。
- 硬边界场景核验（医疗/安全强制/质量事故/权力不对称等）：`should-not-trigger-01` 逐条核对，判定均按 SKILL.md 的 B 段边界执行，未放宽、未误触。

## 结论

- **全部通过，接受**。trigger 描述与边界条款在本轮降级自测中无歧义；兄弟 skill 混淆场景全部被正确拒绝。
- 提示：本轮为 fallback 自测；若后续获得子代理能力，建议对 `should_not_trigger` 与 `edge_case` 优先复测。

## 回炉记录

- 本轮**无需回炉**：通过率 100%（≥ 0.8），且诱饵测试零失败、跨 skill 混淆场景全部正确拒绝。
- 回炉权限备忘（methodology 06）：如未来复测失败，只改 SKILL.md 的 `description` / A2 / E / B；不得修改 test-prompts.json 的测试条目。
