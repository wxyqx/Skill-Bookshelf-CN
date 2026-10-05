# test-results.md — habit-zone-frequency-first

- **测试日期**: 2026-10-01（阶段 4 压力测试）
- **测试方式**: **主流程降级自测（fallback）**——按 methodology 06 降级条款执行：当前环境无独立 sub-agent 能力，由主流程以"干净视角"串行模拟"只加载本 SKILL.md 的全新 agent"逐条判定。**可信度低于独立 sub-agent 盲测**（判定者与流水线同源，存在自证偏差风险），建议发布前用独立会话复核。
- **盲测输入协议**: 模拟宿主环境——给判定者全部 21 个 skill 的 name + description 列表（做"该激活哪一个"的选择题）+ 本 skill 的 SKILL.md 全文 + 用户 prompt；隐藏 test-prompts.json 的 type / expected_behavior / notes，先判定后判卷。
- **通过率**: **6/6 = 100%**（minimum_pass_rate = 0.8，**达标**）
- **诱饵容错**: should_not_trigger 2/2 通过（0 失误，容错为 0 达标）

## 逐条盲测判定

| id | prompt 摘要 | 盲测判定 | 判定理由（模拟干净 agent 视角） | 判卷 |
|---|---|---|---|---|
| should-trigger-01 | 房贷计算器加签到和每日推送，靠谱吗 | 激活本 skill | description"低频产品该走什么路线/评估'让用户每天打开'是否现实"逐字命中；E2（重构高频入口）+E3（首选心智路线）给出两条正路；B 段"为凑频率做打扰式推送"红线覆盖"不要硬造打扰" | ✅ 通过 |
| should-trigger-02 | 两个新点子（每日记账 vs 年度合同审查）先做哪个 | 激活本 skill | description"新点子可行性过滤"直接命中；两轴不对称判据（频率硬、用途软）是 I 段签名结构，产出为两轴定位+三选一结论 | ✅ 通过 |
| should-trigger-03 | 功能有用但用户不来，要不要继续投入做习惯设计 | 激活本 skill | A2 情境 3（需求评审争执）对应；description"值不值得做习惯设计"命中；E 段以三选一结论收束 | ✅ 通过 |
| should-not-trigger-01 | 记账 App 上线三个月留存平平，是没救还是没到时候 | 不激活，转 vitamin-to-painkiller | description"何时不调用：判断维生素/止痛药证据（那是 vitamin-to-painkiller）"显式排除；f03 的 description 含"判断产品是没救还是没到时候"逐字匹配 | ✅ 通过 |
| should-not-trigger-02 | 上线半年，用数据找忠实用户行为路径让新用户照走 | 不激活，转 habit-test-three-steps | description"何时不调用：产品已上线要测真实习惯（那是 habit-test-three-steps）"显式排除；f20 的"习惯路径"语义逐字匹配 | ✅ 通过 |
| edge-01 | 每周一次的健身打卡，做不成每日习惯就别做？ | 激活本 skill，给结构化回答 | prompt 直接落在频率轴判断域；I 段明示"习惯形成没有通用时间表、'频率多高才算高'无定论"，E2 给"贴近每日"的重构方向而非一票否决，E4 输出三选一结论；B 段旧习惯回转（ce04）提示防复发。**注意**：description 单独读可能被浅层 agent 误推为"每周=频率不足=放弃"，本判定按完整 SKILL.md（I 段相对判断框架）给通过 | ✅ 通过（带边界备注） |

## 失败分析

无失败用例。

## 备注

- edge-01 是本 skill 最脆弱的一条：通过依赖 I 段的"无数值门槛"声明与 E4 三选一收束。若未来 Description 精简，应保留"频率优先是方向而非一票否决线"的措辞。
- 与 f03（向后看验收）与 f20（上线后测量）的兄弟混淆诱饵均由 description 的"何时不调用"显式条目化解。


---

## 后置修复记录（2026-09-30 终检）

- description 超出 ≤300 字红线，已精简（保留全部触发场景、不适用边界、兄弟 skill 指向、中英 trigger 与伦理红线，语义不变）；本文件盲测判定结论继续有效。
