# PIPELINE_STATE — 创业投资法律手册

- 书 slug: startup-legal-handbook
- 来源: E:\download\122510\122510\创业投资法律手册:那些你在创业时应该知道的公司法知识.epub(EPUB,251 文档,文本层完整)
- 开始: 2026-10-05,跨日完成于 2026-10-06

| 阶段 | 状态 | 产出 |
|---|---|---|
| 提取 | ✅ | _source/ch00-front + ch01-ch10(235 问,21 万字;EPUB spine 顺序,章标题页切分,base64 水印清洗) |
| 阶段 0 | ✅ | BOOK_OVERVIEW.md(9 骨架论点,10 术语,时效性为第一批判)——2026-10-06 因并行会话清理重建一次 |
| 阶段 1 | ✅ | 11 单元扫描 → 原始候选约 400 条 → 合并五池(58/125/49/61/55)。注:合并池被并行清理,以验证产出+源文恢复;glossary 由源文重扫 55 条 |
| 阶段 1.5 | ✅ | verified_A(61/183)+ verified_B(16,重建池已逐条原文复核,定位/引文全修正)→ verified.md(77 单元→16 skill)+ rejected/ |
| 阶段 2 | 🔄 | 标杆: charter-governance-design;其余 15 个 builder 分批 |
| 阶段 3 | ⬜ | INDEX.md + GLOSSARY.md(素材: candidates/glossary.md 55 条) |
| 阶段 4 | ⬜ | test-prompts.json 随各 skill 产出;集中盲测+终检待做 |
| 阶段 5 | ⬜ | DIGEST.md;书架 wxyqx/skill-bookshelf-CN 同步(04-创业与经营);push;清理本地 |

## skill 清单(16)
entity-choice-incorporation, capital-contribution-compliance, equity-rights-design, veil-piercing-liability, charter-governance-design, resolution-validity-procedure, shareholder-qualification-registration, minority-shareholder-remedies, nominee-shareholding-risk, equity-transfer-pricing, capital-change-restructuring, employee-equity-incentive, exit-dissolution-liquidation, legal-rep-compliance-contracts, cross-border-foreign-investment, paper-validity-traps

## 注意事项
- **并行会话风险**:本工作区有另一会话在拆 chuanyue-handong,曾清掉本流水线中间产物;关键文件已备份 %TEMP%\legal-handbook-backup;清理时只删自己的书目录
- **法律时效性**:本书 2014 年版(2013 公司法),每个 skill 的 B 段必须带时效性警示(2023《公司法》/民法典/外商投资法/九民纪要差异)
- 版权:R 段引用 ≤60 字(比红线 150 字更严)
- 子代理并发上限 3-4,失败等 30 秒补发
- skill 输出为方法论蒸馏,非法律意见;各 SKILL.md 应声明不构成法律建议
