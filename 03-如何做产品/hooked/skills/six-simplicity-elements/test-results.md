# test-results.md — six-simplicity-elements

- **测试日期**: 2026-10-01（阶段 4 压力测试）
- **测试方式**: **主流程降级自测（fallback）**——按 methodology 06 降级条款执行：当前环境无独立 sub-agent 能力，由主流程以"干净视角"串行模拟"只加载本 SKILL.md 的全新 agent"逐条判定。**可信度低于独立 sub-agent 盲测**（判定者与流水线同源，存在自证偏差风险），建议发布前用独立会话复核。
- **盲测输入协议**: 模拟宿主环境——给判定者全部 21 个 skill 的 name + description 列表（做"该激活哪一个"的选择题）+ 本 skill 的 SKILL.md 全文 + 用户 prompt；隐藏 test-prompts.json 的 type / expected_behavior / notes，先判定后判卷。
- **通过率**: **6/6 = 100%**（minimum_pass_rate = 0.8，**达标**）
- **诱饵容错**: should_not_trigger 2/2 通过（0 失误，容错为 0 达标）

## 逐条盲测判定

| id | prompt 摘要 | 盲测判定 | 判定理由（模拟干净 agent 视角） | 判卷 |
|---|---|---|---|---|
| should-trigger-01 | 政务 App 老年用户注册率低，大字版也没用，问题出在哪 | 激活本 skill | description"特定人群（如老年人）不用产品"逐字命中（verified.md V2 标准外推）；E2 逐项排查六要素，指出大字版只覆盖部分脑力维度、卡点可能在脑力/社会偏差/非常规性，与预期一致 | ✅ 通过 |
| should-trigger-02 | 结账 11 个字段放弃率 75%，哪一步最该砍 | 激活本 skill | description"注册/下单/办事流程完成率低"命中；E1 列全步骤→E2 逐项标注摩擦→E3 锁最短板→E4 对应减法，产出链完整 | ✅ 通过 |
| should-trigger-03 | 报销系统没人用：嫌麻烦+怕填错被审计盯上，怎么分析 | 激活本 skill | "嫌麻烦"对应脑力/时间、"怕被审计盯上"对应社会偏差（他人接受度）——正是本 skill 相对常见易用性清单的两个签名维度；description trigger"怕丢人/社会偏差"语义覆盖 | ✅ 通过 |
| should-not-trigger-01 | 注册后想让用户多填资料、导通讯录，该什么时候提、怎么提 | 不激活，转 investment-timing-granularity | description"何时不调用：投入阶段的设计（投入端允许加摩擦，规则方向相反）"显式排除；f17 的"注册后要不要立刻收资料"逐字匹配；contrasts 关系两侧对称记录 | ✅ 通过 |
| should-not-trigger-02 | 推送打开率只有 2%，怎么提高曝光 | 不激活，转 external-triggers-four-types | description"何时不调用：纯触达问题"显式排除；行为根本没被唤起，未到能力摩擦排查；f04 的触达/触发语义匹配 | ✅ 通过 |
| edge-01 | 专业工具"上手有点难但学会了效率高"，学习成本高价值高的产品需要简化吗 | 可调用但克制，部分调用 | prompt 直接问"需要简化吗"，激活无疑；克制回答的依据链：首次上手属行动环节（E 段减摩擦适用，定位 time-to-first-value 的最短板做定向减法）vs 精通后的效率属技能沉淀（B 段"把一切环节都简化到零会同时消灭投入"、与 f17 的分段判据）→ 反对整体儿童化。**注意**："技能习得=储存价值（f15）"的显式指认需 agent 综合分段判据推导，description 单独不保证完整，属 fallback 自测已知局限 | ✅ 通过（带边界备注） |

## 失败分析

无失败用例。

## 备注

- edge-01 是本 skill 最脆弱的一条（"学习成本即护城河"的张力），通过依赖 B 段投入反场景 + contrasts-with f17 的分段判据组合；建议独立复核时重点重测。
- 两条诱饵（f17 投入端、f04 触达端）均有 description 显式排除条目，是本测全绿的主要机制。
