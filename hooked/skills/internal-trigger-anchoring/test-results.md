# test-results.md — internal-trigger-anchoring

- **测试日期**: 2026-10-01（阶段 4 压力测试）
- **测试方式**: **主流程降级自测（fallback）**——按 methodology 06 降级条款执行：当前环境无独立 sub-agent 能力，由主流程以"干净视角"串行模拟"只加载本 SKILL.md 的全新 agent"逐条判定。**可信度低于独立 sub-agent 盲测**（判定者与流水线同源，存在自证偏差风险），建议发布前用独立会话复核。
- **盲测输入协议**: 模拟宿主环境——给判定者全部 21 个 skill 的 name + description 列表（做"该激活哪一个"的选择题）+ 本 skill 的 SKILL.md 全文 + 用户 prompt；隐藏 test-prompts.json 的 type / expected_behavior / notes，先判定后判卷。
- **通过率**: **6/6 = 100%**（minimum_pass_rate = 0.8，**达标**）
- **诱饵容错**: should_not_trigger 2/2 通过（0 失误，容错为 0 达标）

## 逐条盲测判定

| id | prompt 摘要 | 盲测判定 | 判定理由（模拟干净 agent 视角） | 判卷 |
|---|---|---|---|---|
| should-trigger-01 | 番茄钟 App 只在 deadline 前用，怎么进入日常 | 激活本 skill | description"工具只在 deadline 前被想起"逐字命中（verified.md V2 标准外推）；E1–E3（找高频情绪锚点→即时药方验证→喂养期）与预期动作一致，E4 判停兜底 | ✅ 通过 |
| should-trigger-02 | 访谈说不错但回家不想起、除非发推送，问题出在哪 | 激活本 skill | description"功能没问题但用户不惦记"逐字命中；E 段三步走+"每当用户感到 X 就会 Y"绑定句式是硬产出 | ✅ 通过 |
| should-trigger-03 | 一觉得无聊就下意识刷短视频，机制是怎么回事（自查） | 激活本 skill（反向用法） | description"自查'一无聊就刷手机'"逐字命中；A2 情境 4 明确保留反向用法（识别反射弧、重获控制），与 BOOK_OVERVIEW 批判节的两种用法口径一致 | ✅ 通过 |
| should-not-trigger-01 | 用户要"更快的报表"，怎么从访谈里挖出真正想解决的情绪问题 | 不激活，转 five-whys-emotional-root | description"何时不调用：挖情绪根源（five-whys-emotional-root）"显式排除；prompt 的动词是"挖"（发现阶段），f06 管挖、本 skill 管绑，A2 区分条目两侧对称 | ✅ 通过 |
| should-not-trigger-02 | 获客讨论：投广告还是老带新，预算怎么分配 | 不激活，转 external-triggers-four-types | description"何时不调用：外部触达分工"排除；f04 的"冷启动预算分配"逐字匹配 | ✅ 通过 |
| edge-01 | 企业财务系统每天必须用，频率这么高还需要情绪锚定吗 | 激活本 skill，给克制回答 | prompt 直接询问"情绪锚定"必要性，激活无疑；克制回答的依据链：频率来自外部要求而非内部触发（I 段机制定义）→ 强制场景做情绪操纵既不合适也无必要（B 段红线"不把让用户离不开当目标"+设计者本位批判）→ E4 判停精神（不硬装反射）→ 建议预算转向降低摩擦与酬赏对齐（f07/f09/f12 的领地）。**注意**："建议放摩擦/酬赏对齐"的具体去向需 agent 综合 E4 与全书结构推导，description 单独不保证完整，属 fallback 自测已知局限 | ✅ 通过（带边界备注） |

## 失败分析

无失败用例。

## 备注

- edge-01 是本 skill 最脆弱的一条：考验"不机械套用机制"的克制力，通过依赖 I 段机制定义与 B 段红线的组合推理，建议独立复核时重点重测此条。
- f06（挖/绑分工）与 f04（外部/内部分工）两条兄弟混淆诱饵均由"何时不调用"显式指名化解。
