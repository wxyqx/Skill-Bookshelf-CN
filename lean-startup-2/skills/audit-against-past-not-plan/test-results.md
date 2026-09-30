# test-results — audit-against-past-not-plan

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们的探索项目做半年了还没有一分钱收入，下周要向董事会汇报，怎么写才能既诚实又站得住？
- **判定理由**：探索项目无收入怎么写汇报是 A2 情境 1 的标准场景，会以'对照过去'基线组织汇报。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：项目到期没完成责任制目标，团队说这半年收获特别大，想再要一年时间和 1000 万，我该批吗？
- **判定理由**：到期未达标+'收获特别大'续期申请是 A2 情境 2/语言信号原文，会用可审计学习标准自检。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：Our internal venture is being audited against the original business case and every quarter looks like a failure. Is that the right baseline?
- **判定理由**：英文 prompt 命中 trigger 词 innovation audit / baseline：对照原始商业案例审创新项目正是本 skill 要纠正的基线错误。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：财务部要审上一年度的费用报销合规性，帮我看看内控流程有没有漏洞。
- **判定理由**：费用报销合规审计是成熟业务内控问题，传统预算/合规对照成立，B 段排除。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们想把创新项目的进展画成一页仪表板，转化率、留存这些指标该怎么设计、按什么顺序搭？
- **判定理由**：问的是指标体系怎么搭（顺序与设计），应激活 innovation-accounting-three-levels；相邻区分明确'只问怎么建指标是对方'。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们创新项目连续三期环比都在进步，但三年下来离当初的目标越来越远，还要继续吗？
- **判定理由**：按本 skill 读数：连续三期环比进步=在进步（对照过去的基线结论）；但'还要继续吗'是转型/坚持决定，应交 pivot-persevere-cadence 的会议机制处理——本 skill 先给出基线读数再移交。
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
