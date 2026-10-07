# test-results — one-team-success-is-enough

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们第一批 5 个内部创新试点全都没做成，董事会有人质疑转型失败了，怎么回应？
- **判定理由**：“5 个试点全没做成、被质疑转型失败”是 description 首要场景；按组合评估（是否留下可审计学习、证据能否说服第二批）回应。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：下周五个试点团队要向管理层汇报，老板说一个都不许失败，这种气氛下汇报会不会出问题？
- **判定理由**：“一个都不许失败”命中 A2 情境 3 与语言信号“只许成功”；指出 100% 要求必催生绿黄红表演，建议书面化组合定义。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：How should we set success expectations for our first batch of internal startup pilots? Is 100% success rate realistic?
- **判定理由**：英文 pilot batch / 100% success rate / expectation 为 trigger 直译；输出“一个团队成功即胜利”的组合判据。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们产线今年良品率必须达标，团队连续三个月没完成指标，怎么问责改进？
- **判定理由**：产线良品率是成熟业务 KPI 问责，B 段明确组合容错不适用、两套体制并行不互相覆盖。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：其中一个试点团队自己主动提出来终止项目，因为他们证伪了核心假设。这种团队终止后的表彰和叙述该怎么安排？
- **判定理由**：终止后的表彰与叙述是 reward-useful-failure 的工序（相邻区分：事前期望管理 vs 失败后仪式处置）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们的试点汇报里 10 个项目 9 个绿灯 1 个黄灯，零红灯，看起来很健康，有问题吗？
- **判定理由**：“零红灯+比例异常稳定”是 ce02 表演性成功信号；会激活诊断部分：抽查失败去向、追问绿灯背后的可审计学习。
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
