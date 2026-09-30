# test-results — reward-useful-failure

> 测试轮次：阶段 4 压力测试（2026-09-29）。
> 测试方式：**主流程降级自测（fallback）** —— 本环境无子代理工具，无法执行独立 sub-agent 盲测；由主流程模拟“只加载本 SKILL.md 的全新 agent”逐条判断 prompt 是否会激活本 skill。**可信度低于独立 sub-agent 盲测**。
> 判卷标准：`should_trigger` 须明确激活且动作方向符合预期；`should_not_trigger` 不得激活（容错为 0，诱饵含跨 skill 混淆）；`edge_case` 判断须符合预期中定义的边界理由。
> 本书 36 个 skill 的兄弟对照清单（description/相邻区分）已在判卷时逐条核对；本 skill 的诱饵构成：跨 skill 混淆诱饵 1 条 + 同域/反场景诱饵 1 条。

---

## 逐测试结果

### 1. `should-trigger-01` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：下属负责的创新项目上周黄了，及时止损只花了很少的钱。下周全员大会，这个项目黄了的事我该怎么讲？
- **判定理由**：“全员会怎么讲下属失败”是 A2 情境 1 与 description 首要场景；叙述权还给负责人、领导只补三件事、对比数字量化赞美。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 2. `should-trigger-02` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：公司年会刚宣布“拥抱失败”，结果季度考核里项目失败一票否决，现在没人敢提前砍项目，全在硬撑。怎么改？
- **判定理由**：口号拥抱失败、考核一票否决=ce02 式信号不一致（A2 情境 3）；逐条对照奖励/晋升/考核并设计终止表彰机制。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 3. `should-trigger-03` ｜ `should_trigger` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：Our team killed their own project early and saved us millions. Leadership wants to punish the 'failure'. How do organizations handle celebrating a well-executed shutdown?
- **判定理由**：英文 killed their own project / celebrate shutdown 为 trigger 直译；按“谁来讲、讲什么、奖给谁”给出处置。
- **对照预期**：一致 —— 明确激活，执行方向符合 `expected_behavior`。

### 4. `should-not-trigger-01` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：产线上这个月出了 3 起质量事故，客诉率翻倍，质量管理部问要不要对事故责任人宽容处理，毕竟公司提倡宽容失败。
- **判定理由**：产线质量事故是确定性缺陷，B 段明确六西格玛纪律照常、拒绝以容错名义豁免质量责任。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 5. `should-not-trigger-02` ｜ `should_not_trigger` ｜ 判定：不触发 ｜ ✅ 通过

- **prompt**：第一批 5 个内部试点项目全都没做成，高层开始怀疑转型失败了。这种组合层面的预期该怎么管理？
- **判定理由**：组合层预期管理是 one-team-success-is-enough（相邻区分：事前期望 vs 单次终止的叙事与激励处置）。
- **对照预期**：一致 —— 正确拒绝；诱饵指向的兄弟 skill 不在本次判定范围（本题只测本 skill 不抢调）。

### 6. `edge-01` ｜ `edge_case` ｜ 判定：触发 ｜ ✅ 通过

- **prompt**：有位同事连续三个项目都黄了，每次都说“学到了很多”，但说不出测过什么假设、指标变化是什么。公司要不要继续给他机会？
- **判定理由**：讲不出假设的连续失败触发 E 判停的不予表彰分支（ce13 冒牌创业者信号）；会激活本流程，转增长委员会重审并要求下个项目先交假设清单。
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
