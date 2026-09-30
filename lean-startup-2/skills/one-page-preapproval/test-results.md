# test-results — one-page-preapproval

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：学校怕担安全责任，干脆禁止学生做任何自主实验项目。有没有比一刀切禁止更好的办法？
- **判定理由**：“一刀切禁令有没有更好办法”是 description 首要场景与 A2 情境 1；用三档参数化预批把禁令改成显性边界。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们法务审批一个内部实验要三周，法务自己也抱怨制度僵化，但那份审批文件已经二十多页了，怎么改？
- **判定理由**：“法务三周+文件二十多页怎么改”直接对应 c26 一页纸法务文件；诊断真触发参数并把文件当 MVP 迭代压缩。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：怎么设计合规规则才能让团队自愿把实验做小，而不是个个都报大数字？
- **判定理由**：“怎么让团队自愿把实验做小”=预批参数的反向激励（V3 独有机制）；会输出参数三档设计意图。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们整个采购部都想转型：把采购从审批者变成服务内部客户赋能者，系统、人员、考核全要重设计。
- **判定理由**：采购部整体转型（定位/人员/考核全重设计）是 gatekeeper-to-enabler 的部门路径（相邻区分：单件规则 vs 整部门路径）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们这个实验就这一次，涉及某项政策红线，领导已经口头同意了，怎么把这次豁免落实下来？
- **判定理由**：一次性政策红线豁免是 wield-the-sword 的交易谈判（description 明确排除“单次个案豁免”）；预批解决“每一批”。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们起草了预批参数，但把关部门一位主管说：出事他要个人担责，所以宁可全审。
- **判定理由**：主管“担责所以宁可全审”是预批已知失效前提；会激活判停：不硬压参数，先转 accountability-method-culture 调问责对称性或由高层为参数区间背书。
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
