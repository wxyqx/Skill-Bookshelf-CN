# test-results — coach-assume-they-are-right

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：一位固执的资深同事认为他的方案肯定行，完全不肯做任何验证，正面讲道理已经讲不通了，怎么让他试试实验？
- **判定理由**：固执资深同事+讲理失败是 description 首要场景，会激活并设计预测封存式自证实验。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们团队都是十年老兵，说'用户要什么我们最清楚'，拒绝一切用户调研，作为教练我该怎么介入？
- **判定理由**：'用户要什么我们最清楚'拒绝调研命中 A2 情境 2 原文与语言信号'我们比用户更懂'；会激活并设计让现实说话的自证实验。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：How do you coach a resistant senior team that refuses to validate its assumptions?
- **判定理由**：英文 prompt：coach a resistant senior team refusing to validate——描述核心 trigger 的直译。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：团队是新招的几个应届生，还没掌握实验方法，帮我设计一个两周的精益方法入门培训。
- **判定理由**：新手应届生要入门培训——B 段：自证实验是给自信老手的，新手直接教标准方法。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：团队挺配合的，愿意做假设盘点，帮我们把'用户会喜欢这个功能'背后的假设全部列出来排个序。
- **判定理由**：团队配合愿意盘点假设——应激活 leap-of-faith-assumption-audit（合作团队做全面盘点），相邻区分明示。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我嘴上说'假定你们是对的'，其实我打算让他们的实验失败后好接受我的方案，这样用有问题吗？
- **判定理由**：expected 明示“应激活本 skill 但立即触发其边界”：设局式使用被 B 段明令禁止（立场必须真诚，被识破永久关闭教练通道）——激活后应立即改为真诚立场或放弃教练角色。
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
