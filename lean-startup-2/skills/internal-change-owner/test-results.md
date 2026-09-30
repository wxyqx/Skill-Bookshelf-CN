# test-results — internal-change-owner

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：董事会刚批准了数字化转型，CIO 问是不是把项目整体外包给某大咨询公司主导，内部只需要配合。这样行得通吗？
- **判定理由**：外包咨询公司主导转型行不行是 A2 情境 1 原文——激活并给内部人主导判据。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们推新工作法推了半年，没有专人负责，各部门各干各的，上周开总结会老板问“出了问题到底该找谁”，全场没人接话。
- **判定理由**：推半年无人负责、'出了问题找谁'无人应答——A2 情境 2 权力真空。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：Our transformation office head has the title but no budget, reports through three layers, and just executes HQ directives. Is that a real owner?
- **判定理由**：英文 prompt：有头衔无预算无授权——A2 情境 3'实职还是封号'直译。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：报销流程从 5 天压到 1 天的小改进定了方案，部门里几个人认领一下执行就行，需要专门设个“变革负责人”吗？
- **判定理由**：报销流程小改进票决/指派即可——B 段明确排除（设专人专责是杀鸡用牛刀）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：公司请了咨询公司做转型教练，方法模板都是现成的。现在要把 GE 那套东西翻译成我们自己的说法、换个名字落地，该注意什么？
- **判定理由**：把外部方法翻译成本公司语言换名字落地是 localize-dont-copy 的领域（相邻区分明示分工）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：一位中层骨干主动请缨负责转型，但 CEO 只肯口头支持：不给预算、不调整他的汇报线、也不发正式任命。他该接受这个角色吗？
- **判定理由**：会激活：B 段与判停明确——只给口头支持不给预算/汇报线/任命时，正确动作是先完成授权谈判，无授权的专人只是替罪羊预备役，不应贸然接受。
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
