# test-results.md — vitamin-to-painkiller

- **测试日期**: 2026-10-01（阶段 4 压力测试）
- **测试方式**: **主流程降级自测（fallback）**——按 methodology 06 降级条款执行：当前环境无独立 sub-agent 能力，由主流程以"干净视角"串行模拟"只加载本 SKILL.md 的全新 agent"逐条判定。**可信度低于独立 sub-agent 盲测**（判定者与流水线同源，存在自证偏差风险），建议发布前用独立会话复核。
- **盲测输入协议**: 模拟宿主环境——给判定者全部 21 个 skill 的 name + description 列表（做"该激活哪一个"的选择题）+ 本 skill 的 SKILL.md 全文 + 用户 prompt；隐藏 test-prompts.json 的 type / expected_behavior / notes，先判定后判卷。
- **通过率**: **6/6 = 100%**（minimum_pass_rate = 0.8，**达标**）
- **诱饵容错**: should_not_trigger 2/2 通过（0 失误，容错为 0 达标）

## 逐条盲测判定

| id | prompt 摘要 | 盲测判定 | 判定理由（模拟干净 agent 视角） | 判卷 |
|---|---|---|---|---|
| should-trigger-01 | 记账 App 三个月，用户说好但离不开的迹象没有，没救还是没到时候 | 激活本 skill | description"判断产品是没救还是没到时候"逐字命中（verified.md V2 标准外推）；E2 痒判据三问只收行为证据，E3 分支（维生素期=设计窗口/止痛药期=保护动作）与预期一致 | ✅ 通过 |
| should-trigger-02 | 投资人问维生素还是止痛药，怎么回答 | 激活本 skill | description"被问 vitamin or painkiller"逐字命中；I 段阶段论回答（先维生素后止痛药是正当路径）+ 判据，非硬编故事 | ✅ 通过 |
| should-trigger-03 | 不愿卸载+NPS 高，但怀疑不是真依赖，怎么验证 | 激活本 skill | description"验证依赖是真习惯还是口头喜欢"命中；E2 硬约束"不接受态度数据"正是预期的"判据只认行为" | ✅ 通过 |
| should-not-trigger-01 | 新点子一年只发生一两次，该不该按习惯产品设计 | 不激活，转 habit-zone-frequency-first | description"何时不调用：入场前判断能否成习惯（habit-zone-frequency-first）"显式排除；且 E4 判停条件"行为本身频率不足→先回 f02，本 skill 判停"提供第二道防线 | ✅ 通过 |
| should-not-trigger-02 | 不发推送也自动打开，这种自动回访机制怎么形成、想复制 | 不激活，转 internal-trigger-anchoring | description"何时不调用：……做情绪绑定设计"指向 f05；prompt 问的是机制形成（施工方）而非验收判据，f05 的"自查'一无聊就刷手机'/条件反射"语义匹配 | ✅ 通过 |
| edge-01 | "挺好的但我不用"，留存低但没人卸载，还有救吗 | 激活本 skill，坚持判据流程 | description 的"没救还是没到时候"命中；E2 拒绝态度数据（不愿卸载不算证据）、走判据三问收行为证据；E4/B 段"阶段论不豁免频率判据"覆盖"警惕频率轴问题（先回 f02）"；不直接站队"有救/没戏" | ✅ 通过 |

## 失败分析

无失败用例。

## 备注

- 与 f02 的"向前看/向后看"分工和与 f05 的"验收方/施工方"分工是本 skill 两条诱饵的化解机制，均写入 description 的"何时不调用"。
- edge-01 中"频率轴提示"的产出依赖 B 段"低频行为频率不足，永远不会变止痛药"条目；description 单独不保证该提示出现，属 fallback 自测已知局限。
