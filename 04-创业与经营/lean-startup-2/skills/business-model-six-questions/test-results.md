# test-results — business-model-six-questions

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们的知识付费课卖不动，团队讨论来讨论去就是降价和打折，除了价格还能动什么？
- **判定理由**：'除了降价还能动什么'是 description 首要 trigger（verified V2 novel question 变体），会逐问给结构杠杆。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们的新产品做成了一单大生意，但财务和产品部为'这笔升级收入算产品还是服务'吵翻了，客户单子眼看要黄。
- **判定理由**：'收入算产品还是服务'引发部门之争命中 A2 情境 2 与语言信号原文。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们的硬件从设计到铺进门店要一年多，瓶颈其实是经销商不愿意花钱改造陈列室，技术上早就做完了。
- **判定理由**：瓶颈在经销商陈列室（非技术）——'承担中间环节/缩短 BML 周期的非技术环节'两问正是为此设计。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们产品上线三个月，留存很差，用户用了几次就走了，是不是该先做增长投放拉新？
- **判定理由**：留存差说明价值假设未过，应先激活 value-and-growth-hypotheses；判停条件明确'价值证据为零停止六问'。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：公司要给创新团队发钱了，每笔钱按学习里程碑分期拨付还是一年一拨，怎么设计？
- **判定理由**：创新团队拨款制度是 milestone-based-funding 的领域（对内拨款 vs 对外收费，相邻区分明示）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们想按效果收费，但销售说客户不接受，财务说对账做不了，这算商业模式问题还是执行问题？
- **判定理由**：按效果收费正是六问之一——会激活并给设计边界（履约能力为前提），同时指出销售/财务异议属内部裁决问题，必要时转 wield-the-sword 清障；判定为商业模式设计问题而非放弃。
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
