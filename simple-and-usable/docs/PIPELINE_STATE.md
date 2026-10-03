# PIPELINE_STATE — simple-and-usable

| 阶段 | 状态 | 产出 |
|---|---|---|
| 阶段 0 整书理解 | ✅ 完成 | BOOK_OVERVIEW.md（质量门通过：主旨/骨架/11 术语/10 条批判） |
| 阶段 1 并行提取 | ✅ 完成（串行降级：5 个 extractor 逐只执行） | candidates/{frameworks 36, principles 61, cases 43, counter-examples 32, glossary 16} |
| 阶段 1.5 三重验证 | ✅ 完成 | verified.md：97 条方法论候选 → 20 个 skill 单元（21% 通过率）；rejected/f19.md、f14.md（并入不独立） |
| 阶段 2 RIA++ 构造 | ✅ 完成 | 标杆 four-strategies 主流程自写（盲测 6/6）；其余 19 个由 4 批 builder 串行构造；主流程脚本统一终检通过 |
| 阶段 3 Zettelkasten | ✅ 完成 | INDEX.md（分组+mermaid 图+学习顺序）+ GLOSSARY.md（16 条）+ related_skills 回填 40 条边（依赖17/组合18/对比5） |
| 阶段 4 压力测试 | ✅ 完成 | 独立盲测 2 只评审员共 120 条 should/should-not 全部命中；1 条测试题修正（complexity-placement 缺终局语境）后单条重测通过；20 条 edge 全部一致（含 3 条协作路由）；test-results.md 已写入各 skill 目录 |
| 阶段 5 交付 | ✅ 完成 | DIGEST.md（约 5500 字）+ 书级 README.md + monorepo 五处同步 + 推送 wxyqx/skill-bookshelf-CN（第 23 本书）；按用户要求不安装本地 skills 目录，推送后清理本地构建产物 |

## Skill 清单（20 个，slug 定稿）

| # | slug | 来源 | 主题 |
|---|---|---|---|
| s01 | pseudo-simplicity-detection | f34,p03 | 貌似简单排查 |
| s02 | business-case-for-simplicity | f04,f05,p04 | 简化的商业论证 |
| s03 | simplicity-baseline | f06,p05,f14 | 简单基准描述 |
| s04 | field-observation | f09,p06,p07,p08 | 真实环境观察 |
| s05 | mainstream-user-lens | f07,f08,p09,p10,p11 | 主流用户立场 |
| s06 | control-and-emotion | f10,p12 | 掌控感与感情需求 |
| s07 | extreme-usability-goals | f11,p15 | 极端简单目标 |
| s08 | user-story-craft | f12,p13,p14 | 用户故事法 |
| s09 | share-the-insight | f15,p17 | 分享认识 |
| s10 | four-strategies | f03,p01,p18 | 四策略总纲 |
| s11 | remove-strategy | f16,f17,f18,f19,p19-p25,f22 | 删除策略 |
| s12 | declutter | f21,p26-p32 | 减速带清理 |
| s13 | organize-strategy | f36,f24,p34-p39,p43 | 组织策略 |
| s14 | visual-organization | f23,p40,p41,p42 | 视觉组织 |
| s15 | hide-strategy | f25,f26,f27,p44-p50 | 隐藏策略 |
| s16 | transfer-strategy | f28,f29,p52,p53,p56,p57 | 转移策略 |
| s17 | open-experience | f30,f31,p54,p55 | 开放式体验 |
| s18 | complexity-placement | f01,f02,p58,p59 | 复杂性放置 |
| s19 | details-carry-simplicity | f33,p60 | 细节支撑简单 |
| s20 | simplicity-boundaries | f35,f32,p02,p61 | 简单的边界 |

## 环境/约定

- 源文本：`_source/sections2/` 9 个章节文件（全书 4.7 万汉字，编码已验证干净）
- 交付形态：书架仓库 monorepo（第 23 本书），**不安装本地 skills 目录**（用户既定要求）
- 版权约定：R 段引用极短（≤60 字）、I 段完全自写、案例转述不抄录
