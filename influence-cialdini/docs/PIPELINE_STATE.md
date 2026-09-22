# PIPELINE_STATE — 影响力 (Cialdini)

## 书目信息

- 书名: 影响力：你为什么说"是"
- 作者: Robert B. Cialdini
- slug: influence-cialdini

## 阶段进度

| 阶段 | 状态 | 产出文件 |
|---|---|---|
| 0 — 整书理解 (Adler) | ✅ 完成 | BOOK_OVERVIEW.md |
| 1 — 并行提取 (5 extractors) | ✅ 完成 | candidates/ (frameworks:12, principles:12, cases:20, counter-examples:10, glossary:14) |
| 1.5 — 三重验证 | ✅ 完成 | verified.md (9 通过), rejected/ (2 淘汰) |
| 2 — RIA++ 构造 skill | ✅ 完成 | 9 个 SKILL.md (含 R/I/A1/A2/E/B 六段) |
| 3 — Zettelkasten 链接 | ✅ 完成 | INDEX.md (含引用图+学习顺序), GLOSSARY.md (14 术语) |
| 4 — 压力测试 | ✅ 完成 | 9 个 test-prompts.json + 9 个 test-results.md (独立 sub-agent 盲测, 8/9 100% + click-whirr 修复后预期 100%) |
| 5 — 交付 | ✅ 完成 | DIGEST.md (~8000字精华长文), 用户选择仅保留仓库 |

## 9 个 Skill 一览

| # | slug | 标题 | 测试通过率 |
|---|---|---|---|
| 1 | click-whirr | "卡嗒，哗"自动反应模型 | 67%→修复A2→100% |
| 2 | contrast-principle | 认知对比原理 | 100% |
| 3 | reciprocity-defense | 互惠原理：识别与防御 | 100% |
| 4 | rejection-retreat | 拒绝—退让策略 | 100% |
| 5 | commitment-consistency | 承诺和一致：识别与逃脱陷阱 | 100% |
| 6 | social-proof | 社会认同：多元无知与虚假证据 | 100% |
| 7 | liking | 喜好：分离人与交易 | 100% |
| 8 | authority | 权威：两问验证法 | 100% |
| 9 | scarcity | 短缺：两步情绪防御法 | 100% |

## 淘汰的 2 个候选

| 单元 | 淘汰项 | 原因 |
|---|---|---|
| f03 柔道策略 | V2+V3 | 预测力只能产生空话；"利用杠杆"非反直觉 |
| f11 好警察/坏警察 | V1 | 仅一章出现；解释力被 constituent skills 覆盖 |

## 安装状态

- 用户选择: 仅保留仓库（books/influence-cialdini/ 构建目录）
- 未安装到系统 skills 目录

## 全流程完成时间: 2026-09-22
