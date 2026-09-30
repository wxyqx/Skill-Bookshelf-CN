# test-results — leap-of-faith-assumption-audit

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我想做宠物上门殡葬服务，感觉肯定有市场，动手前该先确认哪些东西？
- **判定理由**：新事业'感觉肯定有市场'动手前先确认什么——description 首要场景（V2 novel question 原型）。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：下周立项评审会，方案被挑刺最多的就是'你们有什么证据'，我们现在只有技术参数，怎么补？
- **判定理由**：评审被问'有什么证据'只有技术参数——A2 情境 3 原文（该不该造优先于能不能造）。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：Before we build this out, help us run an assumption audit. Which leap-of-faith assumptions should we test first?
- **判定理由**：英文 prompt：assumption audit / leap-of-faith assumptions test first——trigger 词直译。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：这个功能的转化率我们已经有三个月的真实数据了，下一步怎么优化？
- **判定理由**：已有三个月真实用户行为数据——B 段明确此时直接看数据、不再重走假设审计；审计价值已由数据替代。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们已经决定了先测'用户愿不愿意付费'这条假设，现在要想用什么产品形态去测最省钱，大家提几个方案？
- **判定理由**：假设已选定，问用什么形态测最省钱——mvp-trio-and-scorecard 的载体选型（相邻区分明示：测什么归本 skill，用什么测归对方）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们是内部 IT 团队，系统必须用某指定技术栈，商业上领导已经拍板了，写假设还有意义吗？
- **判定理由**：会激活并给边界：'商业上领导已拍板'不等于商业风险已排除——拍板本身可能是未测假设；若确无商业假设，则按 B 段只审技术假设（指定技术栈下的可靠性/迁移成本等）。
- **对照预期**：一致 —— 边界判断符合 `expected_behavior` 中定义的边界理由。

---

## 通过率

- 通过 **6/6**，通过率 **100%**（minimum_pass_rate = 80%）✅
- 其中 `should_not_trigger`（诱饵，容错为 0）：2/2 全部正确拒绝。

## 结论

- **全部通过，接受**。trigger 描述与边界条款在本轮降级自测中无歧义；兄弟 skill 混淆场景全部被正确拒绝。
- 提示：本轮为 fallback 自测；若后续获得子代理能力，建议对 `should_not_trigger` 与 `edge_case` 优先复测。

## 回炉记录

- 本轮**无需回炉**：通过率 100%（≥ 0.8），且诱饵测试零失败、跨 skill 混淆场景全部正确拒绝。
- 回炉权限备忘（methodology 06）：如未来复测失败，只改 SKILL.md 的 `description` / A2 / E / B；不得修改 test-prompts.json 的测试条目。
