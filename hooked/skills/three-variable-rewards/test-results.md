# test-results.md — three-variable-rewards

- **测试日期**: 2026-10-01（阶段 4 压力测试）
- **测试方式**: **主流程降级自测（fallback）**——按 methodology 06 降级条款执行：当前环境无独立 sub-agent 能力，由主流程以"干净视角"串行模拟"只加载本 SKILL.md 的全新 agent"逐条判定。**可信度低于独立 sub-agent 盲测**（判定者与流水线同源，存在自证偏差风险），建议发布前用独立会话复核。
- **盲测输入协议**: 模拟宿主环境——给判定者全部 21 个 skill 的 name + description 列表（做"该激活哪一个"的选择题）+ 本 skill 的 SKILL.md 全文 + 用户 prompt；隐藏 test-prompts.json 的 type / expected_behavior / notes，先判定后判卷。
- **通过率**: **6/6 = 100%**（minimum_pass_rate = 0.8，**达标**）
- **诱饵容错**: should_not_trigger 2/2 通过（0 失误，容错为 0 达标）

## 逐条盲测判定

| id | prompt 摘要 | 盲测判定 | 判定理由（模拟干净 agent 视角） | 判卷 |
|---|---|---|---|---|
| should-trigger-01 | 内部知识库没人贡献，加积分商城有用吗 | 激活本 skill | description"社区贡献量不足/评审激励体系"逐字命中（verified.md V2 标准外推）；E1 对齐动机+E3 社交替代性检查（Mahalo 教训：积分可能挤出社交动机）与预期一致 | ✅ 通过 |
| should-trigger-02 | 社区老用户不发言，怎么设计贡献者的回报机制 | 激活本 skill | description"怎么让人持续贡献"trigger 命中；E2 三通道盘点+对齐检查+变量方案，产出链完整 | ✅ 通过 |
| should-trigger-03 | 游戏化方案评审：签到积分、等级勋章、周排行榜三件套上不上 | 激活本 skill | description"评审激励体系/游戏化方案（积分徽章排行该不该做）"逐字命中；E1 先问"用户为什么来"+载体≠酬赏的判断链与预期一致 | ✅ 通过 |
| should-not-trigger-01 | 课程页转化率低，宣传语强调"升职加薪"还是"别被同龄人落下" | 不激活，转 three-core-motivations | description"何时不调用：行动前的文案动机（那是 f08）"显式排除；f08 的"落地页文案选打动点/趋希望 vs 避恐惧"语义逐字匹配（来之前 vs 来之后的环节分工） | ✅ 通过 |
| should-not-trigger-02 | 短视频留存挺好，但担心用户三个月后看腻，新鲜感怎么维持 | 不激活，转 finite-infinite-variability | prompt 问变量的来源与存续（会不会腻），非酬赏通道选择；f13 的 description（"用户会不会腻/novelty、新鲜感耗尽"）逐字匹配；f12 的"酬赏单一可预测"语义不符 | ✅ 通过 |
| edge-01 | 运营想学拼多多做"开宝箱随机返现"，随机红包符合多变酬赏原理吧 | 激活本 skill，承认机制有效但显式给出红线评估 | prompt 点名"多变酬赏原理"，激活无疑；E5 伦理红线复核（"确认没有用赌博式变量机制针对易感人群制造强迫性使用"）+description 红线句强制 agent 在背书机制有效性的同时给出 f18 复核与易感人群评估，不直接背书 | ✅ 通过 |

## 失败分析

无失败用例。

## 备注

- edge-01 是伦理红线执行类的代表用例：本 skill 的 E5 为具名步骤（非附注），红线执行不依赖 agent 自觉，这是设计上最强的一条。
- f08（环节：来之前/来之后）与 f13（类型 vs 存续）两条兄弟混淆诱饵均由 description"何时不调用"显式指名化解。
