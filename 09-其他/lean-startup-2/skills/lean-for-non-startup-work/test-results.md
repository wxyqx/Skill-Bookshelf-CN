# test-results — lean-for-non-startup-work

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我是个行政，公司马上开年会，领导让我负责排议程。都说精益创业好，可我又不做产品，这套方法跟我有什么关系？
- **判定理由**：行政排年会+'这方法跟我有什么关系'是 A2 情境 1/2 与语言信号原文。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：老板让我发个招聘广告招数字能源团队的工程师，我就是个 HR 专员，有什么办法能让这个招聘做得比以前聪明点？
- **判定理由**：HR 发招聘广告想做得更聪明——A2 情境 2 与书中招聘广告实验（日常 FastWorks）对应。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：I'm not a PM, just an office admin. Is lean startup stuff even relevant for someone like me, or is it only for building products?
- **判定理由**：英文 prompt：office admin 问 lean 是否与我相关——description 直译。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：财务月结每个月都要按时完成，报表格式的口径最近总出错，怎么把这套流程做得更稳不出错？
- **判定理由**：财务月结口径稳定化是有成熟 SOP 的确定性执行——B 段明确不做实验。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：公司推了半年精益工作法，现在没有专人负责，各部门各干各的，培训回来的同事都说“格格不入”。该派谁出来挑头？
- **判定理由**：'该派谁挑头'是变革责任归属——internal-change-owner 的领域（相邻区分明示）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我给老板做 PPT 前想先找三个同事测试一下哪些图表看得懂，结果被老板说“就十几页片子搞这么复杂，先干正事”。我还要坚持实验吗？
- **判定理由**：会激活：按 B 段'方法的价值在轻'回答——PPT 前测三同事是便利贴级轻实验，不需立项排场；同时按判停提示组织无容忍时先积累个人信用，不必硬顶。
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
