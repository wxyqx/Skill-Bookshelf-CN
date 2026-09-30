# PIPELINE_STATE — 《精益创业 2.0》

- **书名**: 精益创业 2.0（The Startup Way）
- **作者**: [美] 埃里克·莱斯（Eric Ries）
- **类型**: 企业创新管理。方法论单元预期：创业式管理、内部创业/创新车间、成长引擎、连续超速增长、精益实验（假设-最小可行产品-验证学习）、创新会计、教练体系、共享资源、转型与阶段门径等，均有明确章节出处。注意与《精益创业》(The Lean Startup) 区分：本书是把精益方法推广到成熟企业的组织篇。
- **全文**: `fulltext.txt`（约 57.6 万字符，calibre 7.23 转换）
- **输出目录**: `e:\solo\books\lean-startup-2\`

## 用户决策（2026-09-29）

1. 5 本书一口气跑完，阶段 0 / 1.5 的确认材料写入产物文件供事后查看，**不实时停顿等确认**。
2. **跳过阶段 5 的安装步骤**：不复制到 `.trae/skills/`，不动 `e:\solo\skill-bookshelf\`。
3. 阶段 5 交付 = `DIGEST.md` 完成即止。

## 阶段状态

| 阶段 | 产出 | 状态 |
|---|---|---|
| 取全文 | fulltext.txt | ✅ 完成 |
| 阶段 0 整书理解 | BOOK_OVERVIEW.md | ✅ 完成（确认材料已写入文件，供事后审阅） |
| 阶段 1 并行提取 | candidates/ | ✅ 完成（串行降级执行，候选 130 条） |
| 阶段 1.5 三重验证 | verified.md + rejected/ | ✅ 完成（通过 120 / 淘汰 10；确认名单已写入 verified.md） |
| 阶段 2 RIA++ 构造 | 36 个 <skill-slug>/SKILL.md + test-prompts.json（四批完成，六段自查通过；verified.md 无 slug 字段，各单元 id→slug 映射待阶段 3 统一登记） | ✅ 完成 |
| 阶段 3 链接 | INDEX.md + GLOSSARY.md（含 id→slug 归一，INDEX.md 附映射表） | ✅ 完成 |
| 阶段 4 压力测试 | test-prompts.json + test-results.md | ✅ 完成（36 skill × 6 条 = 216 条盲测，216/216 通过；主流程降级自测） |
| 阶段 5 交付 | DIGEST.md（安装跳过） | ✅ 完成 |

## 执行日志

- 2026-09-29 全文提取完成（ebook-convert），57.6 万字符。
- 2026-09-29 阶段 0/1/1.5 完成：候选 130（框架 22 / 原则 24 / 案例 32 / 反例 22 / 术语 30）；通过 120（skill 单元 36 = 框架 20 + 原则 16；素材 54；词典 30）；淘汰 10（f06、f20、p01、p02、p03、p04、p07、p15、p18、p22，见 rejected/）。阶段 1 为串行降级执行（无子代理工具），产出格式与并行方案一致；确认材料写入 BOOK_OVERVIEW.md 与 verified.md 供事后审阅。
- 2026-09-29 阶段 3 完成：INDEX.md + GLOSSARY.md；id→slug 归一（SKILL.md 479 处、test-prompts.json 85 处），INDEX.md 附录登记权威映射表。
- 2026-09-29 收尾：9 个 test-prompts.json 残留 fXX 引用归一（32 处替换，覆盖 wield-the-sword / gatekeeper-to-enabler / accountability-method-culture / business-model-six-questions / one-page-preapproval / pivot-persevere-cadence / prfaq-working-backwards / startup-team-basic-unit / three-tier-support-structure）；阶段 4 压力测试完成，36 skill × 6 条 = 216 条盲测（主流程降级自测 fallback，无子代理工具），总通过率 **216/216（100%）**，回炉名单：**无**（全部 ≥ minimum_pass_rate 0.8，诱饵测试零失败）；36 份 test-results.md 生成、36 份 SKILL.md「测试通过率」回填 100% (6/6)；DIGEST.md 完成（约 1.15 万字，36/36 skill 覆盖）；**安装跳过**（未复制到 .trae/skills/ 或 skill-bookshelf，按用户要求）。

## 交付备注

- 书 1《当下的力量》已交付（19 skill，盲测 123/123）；书 2《高效能人士的七个习惯》已交付（29 skill，盲测 174/174）。均零安装。
- 2026-09-29 终检修复：8 个 skill 的 description 超出 ≤300 字红线（315–358 字），已精简至 264–300 字（保留触发场景/边界/中英 trigger，语义不变）；各 test-results.md 追加后置修复记录。
