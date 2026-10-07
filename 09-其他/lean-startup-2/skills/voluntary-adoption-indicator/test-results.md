# test-results — voluntary-adoption-indicator

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：新审批流程在两个部门试点很成功，CIO 现在要求下季度强制全员切换，我觉得不对但拿不出理由，双轨并行又怕永远切换不了。
- **判定理由**：“强制全员切换还是双轨并行”是 A2 情境 1；给出双轨+观察自愿迁移率的裁决依据与退出机制。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：我们在推新的项目管理方法，现在部署率 85%，但只有 3 个团队是真在用的。汇报里该拿什么数字证明推广效果？
- **判定理由**：“部署率 85%、只有 3 个团队真在用”是 A2 情境 2 与 ce15 噪声测量；验收指标换成自愿迁移率并访谈未加入者。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：We're launching an internal design system. Should usage be mandatory, or should we keep the old components around and watch which one teams pick?
- **判定理由**：英文 mandatory vs opt-in 为 trigger 直译；建议保留旧轨、跟踪自愿迁移率作制度质量领先指标。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：生产车间的安全上报新系统 9 月 1 日必须全员上线使用，这是安监要求，宣传物料怎么写让大家接受度高一点？
- **判定理由**：安监强制上线属 B 段排除（强制是义务、自愿率无意义）；问题实为宣传与培训物料。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：公司要上新绩效系统，9000 人一次铺开，我先培训两周再统计使用率——这个推广顺序对吗？
- **判定理由**：“先铺开再统计使用率”问的是部署顺序，归 behavior-before-tools（相邻区分：顺序 vs 度量）；此处行为证据尚未建立。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：开放自愿报名三个月，报名的团队越来越多，但用得最好的反而是被强制接入的财务部。自愿率还能当指标吗？
- **判定理由**：“自愿率能否与强制样本并读”的边界；会激活：自愿流入证明价值主张成立，财务部高使用率须查退出后持续性（防强制幻觉），自愿率不替代后端测量。
- **对照预期**：一致 —— 边界判断符合 `expected_behavior` 中定义的边界理由。

---

## 通过率

- 通过 **6/6**，通过率 **100%**（minimum_pass_rate = 80%）✅
- 其中 `should_not_trigger`（诱饵，容错为 0）：2/2 全部正确拒绝。
- 硬边界场景核验（医疗/安全强制/质量事故/权力不对称等）：`should-not-trigger-01` 逐条核对，判定均按 SKILL.md 的 B 段边界执行，未放宽、未误触。

## 结论

- **全部通过，接受**。trigger 描述与边界条款在本轮降级自测中无歧义；兄弟 skill 混淆场景全部被正确拒绝。
- 提示：本轮为 fallback 自测；若后续获得子代理能力，建议对 `should_not_trigger` 与 `edge_case` 优先复测。

## 回炉记录

- 本轮**无需回炉**：通过率 100%（≥ 0.8），且诱饵测试零失败、跨 skill 混淆场景全部正确拒绝。
- 回炉权限备忘（methodology 06）：如未来复测失败，只改 SKILL.md 的 `description` / A2 / E / B；不得修改 test-prompts.json 的测试条目。
