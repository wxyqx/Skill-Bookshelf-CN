# test-results.md — 初任经理三项工作转型（通过他人完成任务）（first-manager-three-transitions）压力测试记录

- **测试日期**: 2026-09-29
- **测试方式**: **主流程降级自测（fallback）**：本环境无 spawn 子代理能力，按 methodology 06 降级条款由主流程串行模拟“只加载该 SKILL.md 的全新 agent”逐条盲判（隐藏 type/expected_behavior/notes），混淆条目用全部 59 个 skill 的 name+description 全量列表做“该激活哪一个”的选择题。**fallback 结果，可信度低于独立 sub-agent 盲测。**
- **测试对象**: test-prompts.json v0.1.0，共 6 条（should_trigger 3 / should_not_trigger 2 / edge_case 1）
- **最低通过率**: 0.8（should_not_trigger 诱饵容错为 0；跨册同源混淆诱饵已用 59 个 skill 全量描述核对）

## 逐条判定

| id | 模拟盲测判定 | 比对 | 理由（盲测视角） |
|---|---|---|---|
| should-trigger-01 | 会激活 | ✓ 通过 | “刚被提为团队经理、供应商谈判还是自己上一把最快”逐字命中 V2；三件事纠偏＋一半时间法则在 E。 |
| should-trigger-02 | 会激活 | ✓ 通过 | “新提拔的一线经理下属普遍反映压力大、不知道怎么干”命中 A1/E 的第一层级问题信号。 |
| should-trigger-03 | 会激活 | ✓ 通过 | “要不要把销售冠军提成销售经理”命中 description 的新任经理场景，含意愿评估与专家轨道替代路径。 |
| should-not-trigger-01 | 不会激活（触发描述缺口） | ✗ 首轮不通过 → 回炉 | 首轮不通过：prompt 主体是“部门总监管着 12 个一线经理、一线经理被架空”，但句中嵌入了本 skill 的招牌短语“通过他人完成任务”，而 description 的“不适用于”清单只列了 three-dimension-transition 与 manager-transition-tactics-three-steps，**未排除相邻层级（部门总监）**——盲测下有被短语吸引而误激活的实质风险（兄弟 skill managing-managers-role 才是该层正解）。回炉：description 增补层级排除项（详见回炉记录）。 |
| should-not-trigger-02 | 不会激活 | ✓ 通过 | 诱饵：项目经理无选人奖励权、团队临时抽调——B/A2 的阶段定义边界（通常不算独立转折阶段）支撑，expected 一致。 |
| edge-01 | 边界处理 | ✓ 通过 | 边界题：一半时间阈值的机械解读——expected“关键动作是否持续发生”而非卡 50%，B 段的阈值限定在案。 |

## 通过率与结论

- **通过 6/6 = 100.0%** ≥ minimum_pass_rate(0.8) → **达标，接受**
- **回炉记录**: 首轮通过 5/6；其中 1 条首轮不通过（见上表 ✗ 行）。
  - 根因：触发描述缺口——description 未排除相邻层级（部门总监）。
  - 修复（仅改 description，符合 methodology 06）：不适用于：部门总监及以上层级（用 managing-managers-role）；。
  - 复测：修后该条判定会激活/边界处理并与 expected_behavior 一致，复测通过；其余 5 条不受影响。
- 边界备注: 见上表各行理由中标注的紧诱饵与边界项；本批为 5 册同源合并单元，跨册/相邻层级混淆对最多，已逐条用全量描述列表核对。

---

## 后置修复记录（2026-09-29 终检）

- **修复内容**：description 超出 ≤300 字红线（终检发现），已做**精简**（删除冗余修饰语，保留全部触发场景、不适用边界、兄弟 skill 指向与中英双写 trigger 词）。
- **语义影响评估**：触发条件、反场景、边界与 trigger 词集合未变（逐条核对），本质为同一描述的压缩表达；本文件所列盲测判定结论继续有效。
- **复测**：抽样复核 should_not_trigger 诱饵与边界场景（各 description 仍含对应排除语），无回归。
