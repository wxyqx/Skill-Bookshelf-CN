# test-results — behavior-before-tools

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：公司花了 80 万买的知识库软件上线三个月，文档库基本是空的，行政要求每人每周至少写两篇，结果大家复制粘贴凑数。是软件不行吗？
- **判定理由**：'上系统没人用+行政命令维持使用率'是 description 原文场景，会激活并走行为假设→小群实验流程。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们准备给全公司 9000 人上一个新绩效 app，计划一次铺开，培训两周后统计完成率。这个方案有问题吗？
- **判定理由**：9000 人一次铺开+培训完成率验收命中 A2 情境 1/3（部署优先方案评审）。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：We rolled out a new collaboration tool company-wide. Adoption is at 12% and nobody volunteers feedback. Should we buy a better tool or change our approach?
- **判定理由**：英文 prompt：company-wide rollout 低采纳+零反馈，问买更好的工具还是改方法——正是工具遇冷归因诊断。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：线上接口平均响应时间涨到 4 秒，运维说要把数据库从 MySQL 换成分布式数据库，这个方案怎么评估？
- **判定理由**：数据库替换/性能修复是纯技术性能升级，没有行为变量，description 与 B 段均明确排除——不会强套行为实验流程。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：新流程已经小范围试点成功，现在要决定推广节奏：是强制所有部门下季度切换，还是保留旧流程双轨并行让大家自己选？
- **判定理由**：试点已成功后决定强制切换还是双轨并行，是推广验收方式问题，应激活 voluntary-adoption-indicator；本 skill 的'顺序'前提（行为证据先于工具）已满足，不激活。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：生产安全上报系统必须全员 100% 使用，这是合规硬要求，但一线工人确实不爱用，怎么按你们说的行为实验来做？
- **判定理由**：expected 明示“合规硬要求不适用自愿扩大，但行为设计仍然适用”：会激活并给出两分处理——全员强制是底线（不套自愿扩层），而“上报真实、低负担、不造假”的上报质量仍需小群行为实验与激励检查；与 dedicated-cross-functional-teams“可激活一半”同类，判为部分激活。
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
