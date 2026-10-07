# test-results — habit-knowledge-skill-desire

- **被测对象**: [`SKILL.md`](./SKILL.md)（v0.1.0）
- **测试集**: `test-prompts.json`，共 6 条（3 条应触发 / 2 条诱饵（含同书兄弟 skill 混淆诱饵）/ 1 条边界）
- **minimum_pass_rate**: 0.8
- **通过率**: 6/6 = 100% → ✅ 达标，无需回炉
- **执行方式**: ⚠️ **主流程降级自测（fallback）**——当前环境无独立 sub-agent 能力，按 methodology 06 降级条款由主流程串行执行。判定方式：模拟"只加载本 SKILL.md 的全新 agent"（可见 description / A2 触发场景与语言信号 / E / B 边界），并对跨 skill 混淆诱饵附整包 29 个 skill 的 name+description 列表做"该激活哪一个"的选择题；判定时隐藏测试条目的 type / expected_behavior / notes。**可信度低于独立 sub-agent 盲测**，接入 darwin-skill 后可用真实独立盲测复核。

## 逐条判定

| # | 类型 | 用户 prompt | 判定 | 是否触发 | 模拟 agent 判定理由 |
|---|---|---|---|---|---|
| 1 | should_trigger | 理财课学完了三套，记账 App 换了四个，还是月光，问题到底出在哪？ | ✅ 通过 | 是 | desc+V2 场景匹配（理财课三套仍月光）；三栏定位缺口在意愿侧（钱在其使命中无位置），预测补课与换 App 均无效。 |
| 2 | should_trigger | 我知道锻炼重要也知道怎么练，就是不想动，这算懒吗？ | ✅ 通过 | 是 | desc 匹配（知道重要也知道怎么练就是不想动）；定位意愿栏并做 why-bother 追问，不归因于懒。 |
| 3 | should_trigger | 公司组织了新系统培训，大家考试都过了，回去还是用老办法，为什么？ | ✅ 通过 | 是 | desc 匹配（培训考试都过、回去仍用老办法）；区分技巧转化缺失与意愿缺失，分别给不同栏位的干预。 |
| 4 | should_not_trigger | 有没有好用的番茄钟 App 推荐？想要界面干净的。 | ✅ 通过 | 否 | 番茄钟 App 推荐=纯工具选择问题，非习惯成分缺口诊断。 |
| 5 | should_not_trigger | 我的每周计划总是周一就作废，是不是我的计划排法有问题？ | ✅ 通过 | 否 | '日计划承载要务'的层次错误是日程结构问题，应激活 fourth-gen-time-management；三要素模型不管排程。 |
| 6 | edge_case | 我女儿知道玩游戏不好，也承认影响成绩，但她还是天天玩。 | ✅ 通过 | 有限度 | 可调用定位意愿栏（她'知道'与'会'俱足，缺意愿），但必须拦下'讲道理'式说教——结合亲子关系产能（情感账户）与双赢协议设计意愿环境。 |

## 回炉记录

无需回炉：通过率 ≥ minimum_pass_rate（0.8），且全部诱饵测试（should_not_trigger）零失误、边界判定与 B 段规则一致。未对 SKILL.md / test-prompts.json 做任何修改。

---

*本文件为阶段 4 审计产物，生成于 2026-09-29。*