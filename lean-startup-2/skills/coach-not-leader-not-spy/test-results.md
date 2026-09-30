# test-results — coach-not-leader-not-spy

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我最近在给两个创新团队当内部教练，老板昨天跟我说：你反正每周都见他们，顺便帮我盯着点他们的进度，有什么情况直接告诉我。
- **判定理由**：'顺便帮我盯进度'是 A2 情境 2 原文——激活并拒绝情报职能、保留方法职能。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：公司想建内部教练队伍，HR 问教练算什么岗位、要不要考核、向谁汇报，现在全是热心员工在兼职，干半年就累跑了。
- **判定理由**：建教练队伍的岗位/考核/汇报设计与兼职流失（三病症状）命中 A2 情境 1/4。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：We hired an external lean coach and the team now complains she reports everything to our VP. Should coaches sit in performance reviews?
- **判定理由**：英文 prompt：外部教练向 VP 汇报一切、该不该进绩效评审会——正是'非间谍'边界与 A2 情境 5 的咨询距离问题。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们创新团队总卡在财务审批和预算上，是不是也该找个厉害的教练帮我们搞定？
- **判定理由**：瓶颈是预算与审批——B 段：那是发起人/支持者的职责，找教练解决不了（应激活 three-tier-support-structure）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：团队特别固执，谁的话都不听，觉得自己肯定能成。有没有什么招能让他们接受现实、愿意出去见用户？
- **判定理由**：团队固执需要说服技术——那是 coach-assume-they-are-right 的领域（自证实验），本 skill 管角色边界。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：教练发现团队在实验里伪造用户数据，要不要悄悄告诉他们的老板？
- **判定理由**：会激活（教练角色边界纠纷）：'不间谍'指不做常规进度情报，但伪造数据触及诚实与伦理底线——不应'悄悄'告诉老板，而应把问题带回团队要求其自行披露/当面共同处理，教练不作地下情报员也不包庇。
- **对照预期**：一致 —— 边界判断符合 `expected_behavior` 中定义的边界理由。

---

## 通过率

- 通过 **6/6**，通过率 **100%**（minimum_pass_rate = 80%）✅
- 其中 `should_not_trigger`（诱饵，容错为 0）：2/2 全部正确拒绝。
- 硬边界场景核验（医疗/安全强制/质量事故/权力不对称等）：`edge-01` 逐条核对，判定均按 SKILL.md 的 B 段边界执行，未放宽、未误触。

## 结论

- **全部通过，接受**。trigger 描述与边界条款在本轮降级自测中无歧义；兄弟 skill 混淆场景全部被正确拒绝。
- 提示：本轮为 fallback 自测；若后续获得子代理能力，建议对 `should_not_trigger` 与 `edge_case` 优先复测。

## 回炉记录

- 本轮**无需回炉**：通过率 100%（≥ 0.8），且诱饵测试零失败、跨 skill 混淆场景全部正确拒绝。
- 回炉权限备忘（methodology 06）：如未来复测失败，只改 SKILL.md 的 `description` / A2 / E / B；不得修改 test-prompts.json 的测试条目。
