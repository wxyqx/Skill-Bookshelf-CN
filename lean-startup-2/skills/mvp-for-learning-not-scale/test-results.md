# test-results — mvp-for-learning-not-scale

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：老板说我们这个验证用的 MVP 也要过高可用评审，不然不让上线测，我该照办吗？
- **判定理由**：“MVP 也要过高可用评审”是 description 首要场景；先问加码增加什么学习，无增量则用风险控制替代工程加码。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：架构师说虽然只有 50 个试点用户，但现在就得按 100 万用户设计，不然以后重构代价太大，怎么看？
- **判定理由**：“50 个用户就按 100 万设计”即 A2 情境 3/ce21 提前投资可扩展基础设施的标准话术。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：Our MVP looks too rough for demos. Should we polish it for scale or keep it ugly for learning?
- **判定理由**：英文 for learning not for scale / MVP quality bar 为 trigger 直译；输出“多糙才够”的裁决规则。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：产品已经验证成功了，下季度正式发布给全部客户，帮我定 SLA 和高可用架构方案。
- **判定理由**：已验证成功、进入执行期发布，B 段明确“质量就是价值本身”，为学习而优化的标准不再适用。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们要验证学生愿不愿意为时间管理 app 付费，帮我头脑风暴几种最省钱的测试载体，分别要花多少钱。
- **判定理由**：头脑风暴最省钱测试载体是 mvp-trio-and-scorecard 的开工前选型工序（相邻区分：选载体 vs 选定后的打磨标准之争）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们的 MVP 涉及患者数据，法务说必须先过数据安全评估才能找用户测，这算不算无谓的工程加码？
- **判定理由**：“合规与高可用要切开”的边界：会激活本 skill 的裁决框架——合规底线不可绕（B 段），但合规成本可经 one-page-preapproval 参数化压到与实验规模匹配。
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
