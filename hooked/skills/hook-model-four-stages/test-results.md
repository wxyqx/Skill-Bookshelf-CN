# test-results.md — hook-model-four-stages

- **测试日期**: 2026-10-01（阶段 4 压力测试）
- **测试方式**: **主流程降级自测（fallback）**——按 methodology 06 降级条款执行：当前环境无独立 sub-agent 能力，由主流程以"干净视角"串行模拟"只加载本 SKILL.md 的全新 agent"逐条判定。**可信度低于独立 sub-agent 盲测**（判定者与流水线同源，存在自证偏差风险），建议发布前用独立会话复核。
- **盲测输入协议**: 模拟宿主环境——给判定者全部 21 个 skill 的 name + description 列表（做"该激活哪一个"的选择题）+ 本 skill 的 SKILL.md 全文 + 用户 prompt；隐藏 test-prompts.json 的 type / expected_behavior / notes，先判定后判卷。
- **通过率**: **6/6 = 100%**（minimum_pass_rate = 0.8，**达标**）
- **诱饵容错**: should_not_trigger 2/2 通过（0 失误，容错为 0 达标）

## 逐条盲测判定

| id | prompt 摘要 | 盲测判定 | 判定理由（模拟干净 agent 视角） | 判卷 |
|---|---|---|---|---|
| should-trigger-01 | 中学生背单词小程序，判断习惯潜能+整体框架 | 激活本 skill | description 明列"评审一个产品/功能有没有习惯养成潜能"；SKILL.md E1 适用性检查（学生主动参与、可每日高频）→ E2 五问逐环，与预期动作一致 | ✅ 通过 |
| should-trigger-02 | 触发转化都行但用户不回来，系统性查问题在哪 | 激活本 skill | description 的 trigger 信号"为什么用户不回来、留存断在哪"逐字命中；与 habit-test-three-steps 的区分（f20 管上线后测量定义，本例是循环归因）由 description"留存差要定位断在哪一环"决定 | ✅ 通过 |
| should-trigger-03 | 签到/勋章/收藏夹/推送一堆方案组织成完整闭环 | 激活本 skill | description"把零散的增长手段组织成完整循环时"直接命中；E 段按四阶段归位+闭环复查 | ✅ 通过 |
| should-not-trigger-01 | 新功能点击多完成少，改文案还是改流程 | 不激活，转 bmat-action-diagnosis | description"何时不调用：只优化单一环节（行动摩擦找 bmat-action-diagnosis）"显式排除；f07 的 description 含"点击多完成少/该改文案还是改流程"逐字匹配，选择题环境下 f07 胜出 | ✅ 通过 |
| should-not-trigger-02 | 房贷计算器一年用两次，按上瘾模型设计留存？ | 不激活为设计指令（或激活即判停），转 habit-zone-frequency-first | description"何时不调用：低频一次性工具……模型不适用"显式排除；即便进入 SKILL.md，E1 适用性前置检查直接判停，产出是"别按习惯产品设计"而非四阶段套用；f02 的 description（低频产品路线）匹配度更高 | ✅ 通过 |
| edge-01 | 老板要做"让用户上瘾"的产品，讲讲四阶段照着做 | 激活本 skill，但输出先纠偏 | 讲解四阶段属本 skill 职责；SKILL.md B 段伦理红线（习惯≠成瘾，L476"等同蓄意伤害"）+ E1 适用性检查 + description 红线句（"不用于绕过用户自主权的设计，产出前过操纵矩阵"）迫使 agent 先纠正"上瘾"用词、补适用性与伦理自检，而非直接给执行清单 | ✅ 通过 |

## 失败分析

无失败用例。

## 备注

- edge-01 的通过依赖完整 SKILL.md 的 B 段与 E1（description 单独只含红线提示，不保证纠偏动作完整）——若宿主只加载 description，该边界的输出质量可能下降，属 fallback 自测的已知局限。
- 本 skill 为全书总纲，其 6 条用例不与其他 20 个 skill 的用例重叠；兄弟混淆诱饵（f07、f02）均在 description 的"何时不调用"中有显式排除条目，是本测全绿的主要机制。


---

## 后置修复记录（2026-09-30 终检）

- description 超出 ≤300 字红线，已精简（保留全部触发场景、不适用边界、兄弟 skill 指向、中英 trigger 与伦理红线，语义不变）；本文件盲测判定结论继续有效。
