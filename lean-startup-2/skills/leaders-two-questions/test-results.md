# test-results — leaders-two-questions

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：孩子的月考成绩掉了十几名，我不想一开口就骂，第一句话该问什么？
- **判定理由**：孩子考砸了第一句问什么——A2 情境 2 原文，激活并给两问话术与理由。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：下属负责的新产品上市遇挫，下午要来汇报坏消息，我怕自己忍不住先骂人，怎么准备这场谈话？
- **判定理由**：下属汇报坏消息前的谈话准备是 A2 情境 1；会给出把追责开场换成两问的具体话术与顺序纪律。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：In our review meeting, what should a leader ask first when a project misses its targets?
- **判定理由**：英文 prompt：leader ask first when project misses targets——description 核心直译。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：仓库昨晚丢了一批货，监控查清楚了是老张没按流程锁门，这种情况怎么处理他？
- **判定理由**：丢货查清责任人是纯执行力/事故问责问题，B 段明确排除（直接谈执行问责，套两问是纵容绕圈子）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们转型会开得太少，项目总是拖到最后一刻才讨论要不要转向，怎么把这种会制度化地排进日程？
- **判定理由**：转型会怎么制度化排期是 pivot-persevere-cadence 的领域（相邻区分明示：什么时候谈归对方）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：下属汇报'项目虽然没达标，但我们收获特别大'，然后讲了一堆感悟，没有任何数字，我该用两问吗？
- **判定理由**：'收获特别大'无数字正是 A2 情境 4/ce19 场景——激活：第一问照问，第二问'你是怎么知道的'专防假学习；答不出证据则按判停共同设计最小实验。
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
