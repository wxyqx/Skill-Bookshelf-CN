# PIPELINE_STATE — cong-baobiao-kan-qiye（从报表看企业：数字背后的秘密（第5版））

- 书：《从报表看企业：数字背后的秘密（第5版）》张新民，人大社 2024-01
- 构建目录：C:\Users\Verify\.zcode\workspace\default\books\cong-baobiao-kan-qiye\（用完即清）
- 去向：wxyqx/skill-bookshelf-CN（登记后 7 处同步），本地不保留

| 阶段 | 状态 | 产出 |
|---|---|---|
| 提取 | ✅ 2026-10-05 | _source/book_full.txt 21.3万字，13 章切分 |
| 阶段 0+1 扫描 | ✅ 4 扫描器 | candidates/scannerA-D.md，原始候选 334 条 |
| 阶段 1 合并 | ✅ 5 合并器 | 框架 54 / 原则 57 / 案例 80 / 反例 35 / 术语 65 = 291 单元 |
| 阶段 1.5 验证 | ✅ 2 验证官 | verified.md（框架+原则：76 通过，打包 16 skill）+ verified-cases.md（反例 31 通过，案例索引，4 打包建议） |
| 打包定案 | ✅ | **17 个 skill**：16（验证官1）+ 比率避坑独立；商誉→估值、占款→治理、审计+造假合并、e06/e09/e24/e26/e30/e35/e08 按主题随包 |
| 阶段 2 构造 | ✅ 17/17（标杆盲测 7/7；7 个超长 description 已修剪） | 各 skill SKILL.md+test-prompts.json |
| 阶段 4 测试 | ✅ 终检 ALL PASS；集中盲测硬性题 101/102（唯一失分=标杆 T3 表述歧义），34 诱饵 0 失误 | 各 skill test-results.md |
| 阶段 3 链接 | ✅ | INDEX.md / GLOSSARY.md(65术语) / DIGEST.md(3448字) / BOOK_OVERVIEW.md |
| 上传书架 | 进行中 | |
| 清理本地 | 未开始 | |

## 17 skill 清单（slug ← 覆盖单元）
1. eight-lens-statement-analysis ← f01,f51,f54,p45
2. strategy-from-asset-structure ← f02,f03,f11,f12
3. capital-source-four-drives ← f14,p16,p52,e06
4. governance-stance-analysis ← f13,f16,p30,p38,e07,e10,e29,e33
5. parent-vs-consolidated-statements ← f08,f17,f18,f31,p18,p46
6. two-end-eating-working-capital ← f19,p23,p21,p51,p31,e09
7. asset-quality-triage ← f39,f30,f20,f23,p42,p54,p55,e35
8. income-statement-structure-analysis ← f26,f27,f28,f29
9. core-profit-cash-conversion ← f21,f22,p19,p20,p44,p57
10. valuation-ma-equity-pricing ← f25,p26,f32,f33,f34,p43,e13,e34,e24,e26
11. cost-determinants-impairment-attribution ← f37,f38,p29,p32,p33,p34
12. financial-risk-debt-quality ← f45,p47,p48,p49,p50
13. overexpansion-risk-signals ← f40,f47,f48,e08
14. prospect-forecast-growth-options ← f52,f53,f41,f44,e30
15. financial-fraud-detection ← f49,p05,p06,e01,e14,e17,e19,e25,e28
16. business-to-statements-deduction ← f05,f07,p03
17. ratio-analysis-pitfalls ← e03,e04,e05,e12,e16,e18,e23
