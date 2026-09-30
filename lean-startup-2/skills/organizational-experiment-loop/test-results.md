# test-results — organizational-experiment-loop

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我想做副业，朋友劝我先花两个月把网站建完整再推广，我觉得太重了——到底该先做完整产品还是先测有没有人要？
- **判定理由**：“先建完整网站还是先测有没有人要”命中 description 首要场景与 A2 情境 1；按五步循环重构为最便宜 MVP+行为进展单位。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：公司让我牵头一个内部创新项目，快半年了没产出，领导问我们到底有没有进展、怎么证明——我该拿什么汇报？
- **判定理由**：内部项目半年无产出、领导问怎么证明进展——A2 情境 3；以验证式学习组织汇报并接领导者两问。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们的新项目数据一直不好，团队吵了两周要不要换方向，有人说再坚持坚持，有人说要 pivot，怎么决定？
- **判定理由**：“要不要换方向”是五步循环第 5 步转型/坚持的标准入口；用假设证据状态与转型的结构化定义输出决定。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们准备立项一个新内部工具，想先把所有假设一条条列出来排个序，看哪个最该先测——有没有系统的方法？
- **判定理由**：只要假设清单与排序=第 1 步专用工具，description 明确“只排假设用 leap-of-faith-assumption-audit”，不得抢调全循环。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：顺便问一下，MVP 和原型机有什么区别？给我讲讲概念就行。
- **判定理由**：MVP 与原型机概念查询是纯信息查询，description 与 B 段明确排除——简要回答概念即可，不展开五步循环构造。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：老板要求每个团队每季度至少跑一个实验，怎么把这句话变成制度？
- **判定理由**：“把每季一实验变制度”主诉含“实验怎么跑”；会激活定循环，并指出制度层需配 growth-board-design/milestone-based-funding（组合而非二选一）。
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

---

## 后置修复记录（2026-09-29 终检）

- **修复内容**：description 超出 ≤300 字红线（终检发现），已做**精简**（删除冗余修饰语，保留全部触发场景、不适用边界、兄弟 skill 指向与中英双写 trigger 词）。
- **语义影响评估**：触发条件、反场景、边界与 trigger 词集合未变（逐条核对），本质为同一描述的压缩表达；本文件所列盲测判定结论继续有效。
- **复测**：抽样复核 should_not_trigger 诱饵与边界场景（各 description 仍含对应排除语），无回归。
