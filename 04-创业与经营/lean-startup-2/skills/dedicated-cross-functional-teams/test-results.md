# test-results — dedicated-cross-functional-teams

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：内部产品团队想配个法务，但法务 headcount 根本借不到，这个项目还能上吗？
- **判定理由**：借不到法务 headcount 是 description 首要场景——激活并给'借义工'解法与判停。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们创新项目挂着跨职能的名头，实际是五个部门各派一个代表，每次开会都凑不齐人，决策一等就是一周。
- **判定理由**：跨职能名头下实际是各部门兼职代表凑不齐——A2 情境 2 的专职性纪律问题；会给出借义工而非借编制的解法。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：Should team members on our internal venture be dedicated full-time, or is it fine if they join part-time from their departments?
- **判定理由**：英文 prompt：专职还是各部门兼职参与——description 核心规则的直译。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们想请一位外部行业专家每周来顾问两小时，帮忙把把关方向，怎么设计这个顾问协议？
- **判定理由**：外部专家每周两小时顾问是 B 段明确排除的场景（本就不在场，不适用专职纪律）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：公司要全面推广新工作法了，培训名单该怎么定？法务和财务的负责人要不要也拉进教室？
- **判定理由**：全公司推广的培训名单（法务财务负责人进不进教室）是 train-the-veto-holders 的组织传播层问题，不是团队层 staffing。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：有位设计师特别认同我们的愿景，愿意用下班时间帮我们，但他不能搬桌子过来坐班，这算义工吗？
- **判定理由**：命中'义工模式'：会激活并给边界判断——义工的关键在'物理在场与响应速度'，不能坐班只能算名义义工，需约定关键节点到场/固定响应时段，并接受关键时刻无人在场的代价。
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
