# test-results — train-the-veto-holders

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：公司要推内部新工具和新工作法，培训预算只够一轮，先培训一线员工还是先培训各部门负责人？
- **判定理由**：“预算只够一轮先培训谁”是 description 核心命题；否决权持有者先于/同步实践者进同一间教室。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们的新流程试点效果很好，但每次提交审批都被财务打回来，理由永远是'没有先例'，怎么破？
- **判定理由**：“被财务以没有先例打回”是 A2 情境 2；画否决权地图、把财务纳入培训并对齐预批参数与风险语言。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：Who should we train first when rolling out the new methodology—practitioners or the gatekeepers who can veto it?
- **判定理由**：英文 gatekeepers / veto / stakeholder training 为 trigger 直译；输出否决者先行的名单纪律。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：员工年度合规培训完成率只有 70%，怎么把全员合规课的完课率提上去？
- **判定理由**：合规课完课率是以培训本身为目的的项目管理，B 段明确排除（本 skill 管变革传播中的对象排序）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：创新团队想请一位法务每周来团队坐班，随时解答合规问题，怎么说服法务部出这个人？
- **判定理由**：“法务进团队坐班”是 dedicated-cross-functional-teams 的 staffing 问题（相邻区分：进团队 vs 进教室）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：把法务总监请进培训教室，他当场表态'我反对整个这套东西'，这是不是失败了？
- **判定理由**：“当场反对≠失败”属本 skill 边界情形；会激活：否决依据从隐性变显性即达成一半目的，反对意见转成风险参数（one-page-preapproval），残余僵局升级支持者。
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
