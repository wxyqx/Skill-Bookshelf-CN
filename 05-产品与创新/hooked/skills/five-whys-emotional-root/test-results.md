# test-results.md — five-whys-emotional-root

- **测试日期**: 2026-10-01（阶段 4 压力测试）
- **测试方式**: **主流程降级自测（fallback）**——按 methodology 06 降级条款执行：当前环境无独立 sub-agent 能力，由主流程以"干净视角"串行模拟"只加载本 SKILL.md 的全新 agent"逐条判定。**可信度低于独立 sub-agent 盲测**（判定者与流水线同源，存在自证偏差风险），建议发布前用独立会话复核。
- **盲测输入协议**: 模拟宿主环境——给判定者全部 21 个 skill 的 name + description 列表（做"该激活哪一个"的选择题）+ 本 skill 的 SKILL.md 全文 + 用户 prompt；隐藏 test-prompts.json 的 type / expected_behavior / notes，先判定后判卷。
- **通过率**: **6/6 = 100%**（minimum_pass_rate = 0.8，**达标**）
- **诱饵容错**: should_not_trigger 2/2 通过（0 失误，容错为 0 达标）

## 逐条盲测判定

| id | prompt 摘要 | 盲测判定 | 判定理由（模拟干净 agent 视角） | 判卷 |
|---|---|---|---|---|
| should-trigger-01 | 用户要"更快的报表"，提速 30% 使用率没涨，怎么找到真正要的 | 激活本 skill | description"用户只要功能不要情绪（要更快的报表提速了没人用）"逐字命中（verified.md V2 标准外推）；E1 校验起点+E2 连问+E3 情绪词停问+绑定句式产出，与预期一致 | ✅ 通过 |
| should-trigger-02 | 写落地页文案，只知道功能愿望清单，不知道用户在什么情绪下需要我们 | 激活本 skill | description"文案不知对准什么情绪"逐字命中；A2 情境 3 对应 | ✅ 通过 |
| should-trigger-03 | 访谈对象说一套做一套（重视数据却从不看周报），怎么问下去 | 激活本 skill | description"口是心非/double talk"命中；B 段"言语不一定能反映出最真实的想法"（L684）+起点纪律（实际行为，L686）支撑"从行为起连问"的回答 | ✅ 通过 |
| should-not-trigger-01 | 五连问挖出来了（怕被老板问住），接下来怎么绑成条件反射、安排推送喂养 | 不激活，转 internal-trigger-anchoring | description"何时不调用：绑定与喂养设计（internal-trigger-anchoring）"显式排除；发现已完成，问句是安装施工——f06 挖、f05 绑的分工在两侧 description 与 A2 均对称记录 | ✅ 通过 |
| should-not-trigger-02 | 产线设备反复停机，主管要求连问五个为什么找流程根因 | 不激活 | description"何时不调用：流水线故障根因分析（丰田原版 5 Whys）"显式排除；B 段"机械/流程故障的根因分析是丰田原版领地，终点是流程改进而非情绪"双重防线 | ✅ 通过 |
| edge-01 | 问到第四个为什么用户不耐烦、答案像在编，第五问还要继续吗 | 激活本 skill，给克制回答 | prompt 是本 skill 执行中的过程问题，激活无疑；E3"情绪词即停，不必机械凑满五问"+B 段"审问式访谈易触发防御、得到编造的合理化答案"（改用情境推演/移情图）+E4 交叉验证，覆盖预期的两种合法收束 | ✅ 通过 |

## 失败分析

无失败用例。

## 备注

- 本 skill 的两条诱饵分布均衡：一条同书兄弟混淆（f05），一条同源方法论混淆（丰田原版 5 Whys）；后者是全部 21 个 skill 中唯一的"邻近方法论诱饵"，化解依赖 description 与 B 段对"终点判据不同"（根因 vs 情绪词）的显式声明。
- edge-01 的"访谈伦理"维度（停止追问、改用推演工具）由 B 段显式覆盖，不依赖 agent 自行发挥。
