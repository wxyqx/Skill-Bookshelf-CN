# PIPELINE_STATE — 《上瘾》

- **书名**: 上瘾：让用户养成使用习惯的四大产品逻辑（Hooked: How to Build Habit-Forming Products）
- **作者**: [美] 尼尔·埃亚尔（Nir Eyal）、瑞安·胡佛（Ryan Hoover）著，钟莉婷、杨晓红 译
- **出版**: 中信出版社
- **全文**: `fulltext.txt`（约 28.3 万字符，calibre 7.23 转换）
- **输出目录**: `e:\solo\books\hooked\`

## 全文结构

| 部分 | 行号 | 说明 |
|---|---|---|
| 正文 | L1–L2365 | 序言 + 前言 + 第1–8章 + 附录（蒸馏主体） |
| 注释和参考资料 | L2366–末尾 | 尾注，不作为候选来源 |

## 用户决策（沿用既定约定，2026-09-30）

1. 一口气跑完，阶段 0 / 1.5 的确认材料写入产物文件供事后查看，**不实时停顿等确认**。
2. **跳过阶段 5 的安装步骤**：不复制到 `.trae/skills/`，不动 `e:\solo\skill-bookshelf\` 本地目录。
3. 阶段 5 交付 = `DIGEST.md` 完成即止；**完成后按用户要求打包上传 GitHub（skill-bookshelf-CN 仓库）**，打包时排除 fulltext.txt 与 _work（版权红线）。

## 阶段状态

| 阶段 | 产出 | 状态 |
|---|---|---|
| 取全文 | fulltext.txt | ✅ 完成 |
| 阶段 0 整书理解 | BOOK_OVERVIEW.md | ✅ 完成（含事后确认材料节） |
| 阶段 1 并行提取 | candidates/（串行降级执行 5 个提取器） | ✅ 完成 |
| 阶段 1.5 三重验证 | verified.md + rejected/（9 个） | ✅ 完成（含事后确认名单节） |
| 阶段 2 RIA++ 构造 | <skill-slug>/SKILL.md × 21 + test-prompts.json × 21 | ✅ 完成（2026-09-30 至 10-01） |
| 阶段 3 链接 | INDEX.md + GLOSSARY.md + 21 个 SKILL.md 链接回填 | ✅ 完成（2026-10-01） |
| 阶段 4 压力测试 | test-prompts.json + test-results.md × 21 | ✅ 完成（2026-10-01，fallback 自测，126/126 通过） |
| 阶段 5 交付 | DIGEST.md（安装按用户决策跳过） | ✅ 完成（2026-10-01） |
| 打包上传 GitHub | skill-bookshelf-CN | ⬜ 待终检后进行 |

## 执行日志

- 2026-09-30 全文提取完成（ebook-convert），28.3 万字符；正文/尾注边界定位完毕。
- 2026-09-30 阶段 0/1/1.5 完成：候选 134 条（框架 24 / 原则 24 / 案例 37 / 反例 22 / 术语 27）；skill 单元通过 21 个（skill 池通过率 21/48≈44%），素材/词典单元通过 86 条（案例 37 + 反例 22 + 术语 27，含少量改绑）；淘汰 9 条（全部 V3 不过，其中 p05 兼 V1）；合并去重 18 条。详见 verified.md 与 rejected/。
- 2026-10-01 阶段 3 完成：21 个 SKILL.md 的 frontmatter `related_skills` 与文末"相关 skills"节回填完毕（占位清理）。链接统计——frontmatter 记录 83 条（composes-with 75 / depends-on 4 / contrasts-with 4）；唯一边 49 条（对称 34 对 + 单向 15 条），单向条目集中于机制单元 E 段伦理复核指向 manipulation-matrix 的守门星型（5 条）与 upgrade-not-replace 的反场景路由（3 条）；4 条 depends-on 均来自 SKILL.md 内显式"使用前提"声明（f09 依赖 f07 归因、f12 依赖 f05 内部触发、f13 依赖 f12 通道、f16 依赖 f05 情绪锚点）。INDEX.md（7 组分类表 + mermaid 引用图 + 推荐学习顺序 + 典型路径）与 GLOSSARY.md（27 条共享词典，含习惯/成瘾、三个"触发"、两种"多变"三组红线词辨析）产出。
- 2026-10-01 阶段 4 完成：126 条用例（21×6，含 40 条 should_not_trigger 诱饵与 21 条 edge_case）按 methodology 06 降级条款做**主流程降级自测（fallback）**——模拟"只加载该 SKILL.md 的全新 agent"，隐藏 type/expected/notes 先判定后判卷，各 test-results.md 均标注"可信度低于独立 sub-agent 盲测"。总通过率 **126/126 = 100%**（无 skill 低于 0.8 门槛，无回炉重做）。重点核对两类诱饵：①兄弟 skill 混淆（触发类 f04/f05/f06 之间、投入类四件套之间、f02/f03/f20 的"频率"词面、f18/p09/p16 的伦理线粒度）——40 条跨 skill 诱饵全部通过；②伦理红线（"打卡焦虑拉 DAU""伪装内生触发""取消导出""注销加摩擦""弱化使用报告"等 21 条 edge 用例）全部执行红线或转介伦理守门单元。边界用例暴露 3 处移交链缺口，按 methodology 06"只准改 description/A2/E/B"微修：five-stored-values（E4 补 f18 转介）、investment-timing-granularity（B 段补 f18 转介）、habit-test-three-steps（B 段补 p16 移交），修后复测通过，记录见各自 test-results.md"回炉与微修记录"。各 skill 通过率（6/6）已回填 SKILL.md 审计信息。
- 2026-10-01 阶段 5 完成：DIGEST.md 精华长文产出（约 9800 字，按书骨架组织——立论与机会评估/触发/行动/酬赏/投入/道德闸门/测量，含 4 条典型使用路径、6 条陷阱反例、6 条作者局限、术语速查与产物地图；每个方法论小节附 skill 链接）。**安装按用户既定决策跳过（零安装）**：未复制到 `.trae/skills/`，未动 `e:\solo\skill-bookshelf\` 本地目录；DIGEST.md 与 INDEX.md 均已注明"本批 skill 未安装到本地技能目录，如需启用请手动复制"。
- 待办：GitHub（skill-bookshelf-CN）打包上传待终检后进行，打包时排除 fulltext.txt 与 _work（版权红线）。

## 交付备注

- 本仓库此前已交付 12 本（145 skills）；2026-09-29 批次 5 本（168 skills）已上传 GitHub（17 本 · 313 skills）。本本完成后将同步上传。
