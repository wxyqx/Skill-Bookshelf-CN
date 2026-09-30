# test-results — unified-entrepreneurial-theory

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：公司想让 CIO 兼管创新，我担心这又是个荣誉头衔，怎么判断给他的是不是实职？
- **判定理由**：“CIO 兼管是不是荣誉头衔”是 description 首要场景；用七项职责逐项审计，重点核对真实经营职责（支票本）。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们公司的新产品、IT 政策、并购和数字化转型各归各的部门管，各有一套考核，要不要统一设一个部门？
- **判定理由**：四类活动各归各部门要不要统一设部是 A2 情境 3；盘点现状并按七项职责设计归口方案。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：Should we set up a dedicated innovation function and appoint a chief innovation officer? What would make it real rather than ceremonial?
- **判定理由**：英文 innovation function / chief innovation officer 为 trigger 直译；给出七项职责审计框架。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们的内部 ERP 项目部署太慢了，18 个月才上一套，怎么用实验方法把这个流程做快？
- **判定理由**：ERP 部署提速是项目层实验问题（归实验循环/MVP 类），B 段明确单个项目执行不属本 skill。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：部门里两个探索项目都在烧钱，下个季度预算只够留一个，该怎么裁？
- **判定理由**：两个探索项目裁一是组合裁决归 growth-board-design（相邻区分：裁决 vs 归口与职责审计）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们要新设一个'创业部'，第一任负责人应该从内部提拔懂文化的，还是从外面请做过风投的？
- **判定理由**：会激活一部分：借七项职责中心智模式条目回答“重要的是心智模式不是履历”，并明示选拔评估超出本 skill 执行步骤属边界。
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
