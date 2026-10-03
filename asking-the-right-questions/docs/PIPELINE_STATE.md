# PIPELINE_STATE — asking-the-right-questions

| 阶段 | 状态 | 产出 |
|---|---|---|
| 阶段 0 整书理解 | ✅ 完成 | BOOK_OVERVIEW.md（质量门通过：主旨/骨架/11 术语/12 条批判） |
| 阶段 1 并行提取 | ✅ 完成（串行降级：5 个 extractor 逐只执行） | candidates/{frameworks 30, principles 39, cases 35, counter-examples 46, glossary 22} |
| 阶段 1.5 三重验证 | ✅ 完成 | verified.md：69 条方法论候选 → 22 个 skill 单元（32% 通过率）；rejected/f12.md（反串法降级为共用技巧） |
| 阶段 2 RIA++ 构造 | 🔄 进行中 | 标杆：skills/locate-issue-conclusion/；其余 21 个由 builder 分批构造 |
| 阶段 3 Zettelkasten | ⏳ | INDEX.md + GLOSSARY.md（glossary.md 提升）+ related_skills 回填 |
| 阶段 4 压力测试 | 🔄 与阶段 2 交错 | 每 skill test-prompts.json；独立盲测集中执行 |
| 阶段 5 交付 | ⏳ | DIGEST.md + 上传书架仓库 wxyqx/skill-bookshelf-CN（第 22 本书） |

## Skill 清单（22 个，slug 定稿）

| # | slug | 来源 | 主题 |
|---|---|---|---|
| s01 | pan-for-gold-reading | f01 | 淘金式阅读姿态 |
| s02 | strong-sense-self-audit | f02,p03,p01,p05 | 强势批判自审 |
| s03 | critical-thinker-values | p04,p09 | 批判性思考者价值观 |
| s04 | keep-dialogue-alive | f05,p06,p39 | 批判性对话维持 |
| s05 | scrutiny-worthiness-filter | f03,p08 | 审查价值过滤 |
| s06 | wishful-feeling-check | p02,f04,p07 | 感情先行与一厢情愿自检 |
| s07 | critical-question-master-list | f06 | 关键问题清单总纲 |
| s08 | locate-issue-conclusion | f07,p10,p11 | 论题与结论定位 |
| s09 | identify-reasons | f08,f10,p15 | 理由识别 |
| s10 | charity-before-judgment | f09,p16 | 施惠原则 |
| s11 | ambiguity-loaded-words | f11,p12,p13,p14 | 歧义与感情色彩词排查 |
| s12 | value-assumption-mining | f13,p18,p19 | 价值观假设挖掘 |
| s13 | descriptive-assumption-mining | f14,p17,p20 | 描述性假设挖掘 |
| s14 | fallacy-three-questions | f15,p21,p22,p23 | 谬误三问判别 |
| s15 | evidence-grade-triage | f16,f17,p24,p25,p27 | 证据效力分级 |
| s16 | expert-opinion-audit | f18,p26 | 专家意见四查 |
| s17 | research-survey-audit | f19,f20,p28,p29,p30 | 研究报告与调查审查 |
| s18 | analogy-evaluation | f21 | 类比评价与自造 |
| s19 | rival-causes-audit | f22,f23,p31,p32,p33 | 替代原因审查 |
| s20 | deceptive-data-check | f24,f25,f26,p34 | 数据欺骗性检查 |
| s21 | omitted-info-probe | f27,f28,p35,p36 | 省略信息排查 |
| s22 | alternative-conclusions | f29,f30,p37,p38 | 备选结论生成 |

## 环境/约定

- 源文本：`_source/sections2/` 13 个章节文件（全书 12.4 万汉字，编码已验证干净）
- 交付形态：书架仓库 monorepo（第 22 本书），**不安装本地 skills 目录**（用户 2026-10-02 指示）
- 版权约定：R 段引用极短（≤60 字）、I 段完全自写、案例转述不抄录
