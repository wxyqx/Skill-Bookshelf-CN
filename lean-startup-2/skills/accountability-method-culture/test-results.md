# test-results — accountability-method-culture

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们公司墙上贴满了'拥抱变化''不断革新'的价值观海报，团建也没少搞，但大家该保守还是保守，为什么没人当真？
- **判定理由**：价值观海报没人当真是 description 首要场景（口号与考核两张皮），会激活并按责任制→方法→文化诊断。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们送了两批骨干去学创新方法，回来都说好，但三个月了没有一个实验落地，说是老板还是按老一套问进度。
- **判定理由**：'培训完没变化、老板按老一套问进度'命中 A2 情境 2 与语言信号'培训完没变化'。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：团队明明知道有更好的开发方案，但那个方案会增加返工量，影响他们的绩效评级，所以全员拒绝，怎么办？
- **判定理由**：考核矩阵直接惩罚目标行为（返工量影响评级）即 A2 情境 3 的 EMS 型症状。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们买了新的绩效管理软件，想全公司推广，怎么让员工尽快用起来？
- **判定理由**：新绩效软件的推广是工具采纳问题（应激活 behavior-before-tools），不是文化因果诊断；description 排除纯推广诉求。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：法务部审批太慢拖累所有项目，想请你们帮我们把法务流程改造成服务内部用户的赋能部门。
- **判定理由**：法务部门整体改造应激活 gatekeeper-to-enabler，本 skill 只在其责任制层出问题时回诊。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们是个刚成立三个月的新团队，老板说想从一开始就建立好文化，需要做文化诊断吗？
- **判定理由**：B 段明确：新组建团队无历史残留，直接设计责任制即可，不需要文化改造叙事——不做诊断。
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
