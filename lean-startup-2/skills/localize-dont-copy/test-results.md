# test-results — localize-dont-copy

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：老板刚参加完硅谷研学回来，要求我们照搬 GE 的 FastWorks，连名字都要一样，明年年中就要见效。怎么落地？
- **判定理由**：“老板要求照搬 GE FastWorks、连名字都要一样”是 description 首要场景（copy/照搬、本地化）；会援引“复制不可能”把整套照搬降级为机制级本地实验并重起名字。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们买了咨询公司的 OKR 落地模板，员工培训完说“工具好是好，但回部门完全用不上，说的话大家都听不懂”。
- **判定理由**：“培训完格格不入、说的话听不懂”命中 A2 情境 4（ce18 标志症状）；会诊断语言与机制未本地化，而非继续加码培训。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：We want to replicate Google's 20% time exactly, including the name. Our COO says just copy-paste the policy. Thoughts?
- **判定理由**：英文 replicate / copy-paste / benchmark 为 trigger 直译；会给出挑机制本地实验+改语言的替代程序。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：我们部门把“周报”改名叫“成长复盘”，内容格式还是原来那套，员工说这是走形式，怎么让大家认可这个新名字？
- **判定理由**：改名不换机制是 B 段明示的反场景（重述对象必须是机制而非修辞）；本 skill 不为其背书，最多指出先改机制再谈名字。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：公司转型推了半年，现在没有专人负责，各部门各干各的，董事会问出了问题该找谁，我该推荐谁出来挑头？
- **判定理由**：变革责任归属与授权是 internal-change-owner 的判据（相邻区分明示“怎么学 vs 谁来管”）；本 skill 不替人选负责人。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们是一家 20 人的小公司，就 3 个部门，造不出“本公司语言”，是不是就没法用这套方法了？
- **判定理由**：“部分适用”型边界：会激活给出轻量路径——不造新词、用团队已有口语，核心仍是机制级本地实验；附带指出书中未讨论小组织属作者盲点。
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
