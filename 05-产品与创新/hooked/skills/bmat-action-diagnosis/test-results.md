# test-results.md — bmat-action-diagnosis

- **测试日期**: 2026-10-01（阶段 4 压力测试）
- **测试方式**: **主流程降级自测（fallback）**——按 methodology 06 降级条款执行：当前环境无独立 sub-agent 能力，由主流程以"干净视角"串行模拟"只加载本 SKILL.md 的全新 agent"逐条判定。**可信度低于独立 sub-agent 盲测**（判定者与流水线同源，存在自证偏差风险），建议发布前用独立会话复核。
- **盲测输入协议**: 模拟宿主环境——给判定者全部 21 个 skill 的 name + description 列表（做"该激活哪一个"的选择题）+ 本 skill 的 SKILL.md 全文 + 用户 prompt；隐藏 test-prompts.json 的 type / expected_behavior / notes，先判定后判卷。
- **通过率**: **6/6 = 100%**（minimum_pass_rate = 0.8，**达标**）
- **诱饵容错**: should_not_trigger 2/2 通过（0 失误，容错为 0 达标）

## 逐条盲测判定

| id | prompt 摘要 | 盲测判定 | 判定理由（模拟干净 agent 视角） | 判卷 |
|---|---|---|---|---|
| should-trigger-01 | 点击率高但注册完成率不到 20%，改文案还是砍字段 | 激活本 skill | description"转化漏斗点击多完成少/争论'该改文案还是改流程'"逐字命中（verified.md V2 标准外推）；E2 按"触发→能力→动机"归因+E3"先补能力"排序与预期一致 | ✅ 通过 |
| should-trigger-02 | 调研都说想要报表导出，上线三个月没人用，为什么说的和做的不一样 | 激活本 skill | description"用户调研说想要但上线不用"逐字命中；E1–E2 拆三要素逐项排查，拒绝直接归因"其实没需求"或马上加激励 | ✅ 通过 |
| should-trigger-03 | 用福格行为模型分析为什么一半学生从不打开在线练习 | 激活本 skill | description trigger 信号"福格模型/Fogg behavior model"被用户点名；E 段给出诊断顺序与"先补能力"建议，跨域（教育）适用 | ✅ 通过 |
| should-not-trigger-01 | 健身打卡社群怎么设计才能让用户每天打开，核心情绪锚点选哪个 | 不激活，转 internal-trigger-anchoring | prompt 不是"行为为什么不发生"的归因，而是从零设计情绪-产品绑定；f05 的 description（"把情绪-使用设计成默认"、情绪锚点）匹配度更高；本 skill 的"何时不调用"未显式指名 f05，判定依赖选择题环境下的语义对比（SKILL.md A2 区分条目有显式说明兜底） | ✅ 通过 |
| should-not-trigger-02 | 想加积分勋章排行榜，用户会买账吗 | 不激活，转 three-variable-rewards | prompt 是游戏化评审；f12 的 description"评审激励体系/游戏化方案（积分徽章排行该不该做）"逐字匹配；本 skill 描述聚焦行为归因，无酬赏设计语义 | ✅ 通过 |
| edge-01 | App 根本没人下载，也是行动公式的问题吗 | 审慎部分调用或拒绝，主体转触发端 | B 段显式反场景："用户根本没有需求（0→1 阶段）……先验证需求存在"与"纯触达量问题：曝光不足时归因于能力/动机是浪费，先回到触发端"；E2 判停条件（触发未出现先修触发、转 f04）支撑"下载为 0 更可能是触达/触发端问题"的回答，与预期"审慎的部分调用或拒绝"一致 | ✅ 通过 |

## 失败分析

无失败用例。

## 备注

- should-not-trigger-01 是本 skill 相对脆弱的一条：description 的"何时不调用"未指名 f05（只写了 0→1 验证/纯触达/已发生），化解靠选择题环境下与 f05 description 的语义对比 + SKILL.md A2 区分条目（"'习惯设计'场景先走触发端"）。若独立复核时该条失败，修法是给 description 的"何时不调用"补"从零设计情绪绑定（f05）"。
- edge-01 考验 B 段反场景（0→1 与纯触达）的执行，两条显式条目足够支撑拒绝式回答。
