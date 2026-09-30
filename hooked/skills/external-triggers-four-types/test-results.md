# test-results.md — external-triggers-four-types

- **测试日期**: 2026-10-01（阶段 4 压力测试）
- **测试方式**: **主流程降级自测（fallback）**——按 methodology 06 降级条款执行：当前环境无独立 sub-agent 能力，由主流程以"干净视角"串行模拟"只加载本 SKILL.md 的全新 agent"逐条判定。**可信度低于独立 sub-agent 盲测**（判定者与流水线同源，存在自证偏差风险），建议发布前用独立会话复核。
- **盲测输入协议**: 模拟宿主环境——给判定者全部 21 个 skill 的 name + description 列表（做"该激活哪一个"的选择题）+ 本 skill 的 SKILL.md 全文 + 用户 prompt；隐藏 test-prompts.json 的 type / expected_behavior / notes，先判定后判卷。
- **通过率**: **6/6 = 100%**（minimum_pass_rate = 0.8，**达标**）
- **诱饵容错**: should_not_trigger 2/2 通过（0 失误，容错为 0 达标）

## 逐条盲测判定

| id | prompt 摘要 | 盲测判定 | 判定理由（模拟干净 agent 视角） | 判卷 |
|---|---|---|---|---|
| should-trigger-01 | 冷启动二选一：投信息流还是做内容搏推荐 | 激活本 skill | description"冷启动预算分配"逐字命中；E3 把两选项落位为付费型/回馈型并引出自主型许可的关键第三选项，与预期动作一致 | ✅ 通过 |
| should-trigger-02 | 一停投放次日留存腰斩，财务不加预算了怎么办 | 激活本 skill | description"增长复盘（停投即流失）"逐字命中；E4 判停（问题不在投放而在内部触发未建立，停止加码、转 f05/f07）正是预期动作 | ✅ 通过 |
| should-trigger-03 | 老带新担心用户觉得被套路，怎么设计不透支朋友关系 | 激活本 skill | description"审查获客渠道"+人际型触发语义命中；E5 黑暗模式三问自检 + PayPal"实际价值驱动自发传播"正例与预期一致 | ✅ 通过 |
| should-not-trigger-01 | 用户不用推送也自动打开，一到情绪点就想起我们，条件反射怎么形成 | 不激活，转 internal-trigger-anchoring | description"何时不调用：情绪绑定（internal-trigger-anchoring）"显式排除；prompt 的"情绪点/条件反射"指向 f05 的情绪锚点语义 | ✅ 通过 |
| should-not-trigger-02 | 上一次的投入自动变成下一次回来的提醒（不是群发） | 不激活，转 load-next-trigger | description"何时不调用：投入内生召回"显式排除；f16 的"触发闭环/用户投入生成"语义匹配；本 skill 与 f16 的 contrasts 关系（外铺 vs 内生）在两边 description 均有区分句 | ✅ 通过 |
| edge-01 | 被大 V 转发日活一周涨五倍，老板要按峰值招人排期怎么劝 | 激活本 skill，给结构化回答 | prompt 属增长复盘场景；SKILL.md I 段四类体检指标（回馈幻觉）+ B 段 ce02（"盲目乐观，认为这就算大功告成，实则不然"、按峰值扩张）直接支撑"先查自主型转化、反对按峰值配置"的判断，非仅贴类型标签 | ✅ 通过 |

## 失败分析

无失败用例。

## 备注

- 本 skill 承载两条硬性跨 skill 诱饵（f05 内部触发、f16 内生召回），均为触发类/投入类兄弟混淆的高危对；化解机制是 description"何时不调用"的显式指名 + contrasts 关系在两侧 SKILL.md 的对称记录。
- "停投即流失"（ce03）与"回馈昙花一现"（ce02）两条书内反例分别对应 should-trigger-02 与 edge-01，反例绑定的 warning_signs 可被 E 段直接引用，是正面判定的主要依据。
