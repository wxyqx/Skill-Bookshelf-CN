# PIPELINE_STATE — positioning-ries-trout（定位：有史以来对美国营销影响最大的观念）

- 书：《定位：有史以来对美国营销影响最大的观念》里斯 & 特劳特，机械工业出版社"定位经典丛书"
- 构建目录：C:\Users\Verify\.zcode\workspace\default\books\positioning-ries-trout\（用完即清）
- 去向：wxyqx/skill-bookshelf-CN（登记为第 40 本，7 处同步），本地不保留

| 阶段 | 状态 | 产出 |
|---|---|---|
| 提取 | ✅ 2026-10-05 | _source/book_full.txt 15 万字，front+引言+22 章+附录共 24 个切分文件 |
| 阶段 0+1 扫描 | ✅ 4 扫描器 | candidates/scannerA-D.md，原始候选 324 条 |
| 阶段 1 合并 | ✅ 5 合并器 | 框架 51 / 原则 67 / 案例 105 / 反例 45 / 术语 51 = 319 单元 |
| 阶段 1.5 验证 | ✅ 2 验证官 | verified.md（118→90 单元，打包 15 skill）+ verified-cases.md（反例 44 通过按 9 家族归组，案例 105 全保留并标注 A1 主题） |
| 打包定案 | ✅ | **15 个 skill**（验证官1 的 15 个；V2 建议的命名/延伸与 V1 重叠故合并，空位→skill5、组织采纳→skill15；反例家族作 B 段素材分配：A自弃→1、D正面进攻→6、B命名→8、C延伸→9、F空位→5、G组织采纳→15、E/H/J→1/15/4） |
| 阶段 2 构造 | ✅ 15/15（标杆盲测 7/7，菜单修 game-rules 后全过） | 各 skill SKILL.md+test-prompts.json |
| 阶段 4 测试 | ✅ 终检 ALL PASS；集中盲测硬性题 90/90（34 诱饵 0 失误），15 edge 全部合理流转 | 各 skill test-results.md |
| 阶段 3 链接 | ✅ | INDEX.md / GLOSSARY.md(51术语) / DIGEST.md(约3240字) |
| 上传书架 | 进行中 | |
| 清理本地 | 未开始 | |

## 15 skill 清单（slug ← 覆盖单元 ← 反例家族）
1. outside-in-perception-first ← f03,p03,p06,p11,p21 + 家族A(自弃)
2. own-one-word-in-mind ← f02,p04,p05,p20,p23
3. first-in-mind-beats-better ← f04,p07,p16,p33,p39
4. mental-ladder-diagnosis ← f06,f10,f45,p48,p49 + 家族J(诊断验证)
5. challenger-follower-positioning ← f07,f08,f11,f17,f18,p18,p22,p63 + 家族F(空位误判)
6. reposition-the-competitor ← f20,p25,p26,p28,p46 + 家族D(正面进攻)
7. leader-defense-playbook ← f12,f13,f14,f15,f16,p13,p17
8. naming-that-hooks ← f22,f23,f24,f27,f34,p08,p27,p30 + 家族B(命名陷阱)
9. brand-extension-rules ← f29,f30,f32,f33,f35,f37,p40,p41 + 家族C(延伸死法)
10. company-institution-positioning ← f02公司面,f38,f39,f46,p02,p43
11. country-place-positioning ← f40,f41,p45
12. personal-career-positioning ← f31,f47,f48,p50,p51,p52 + e44
13. positioning-six-question-process ← f01,f49,f50,p09,p55,p56,p64
14. mind-runs-by-ear-media-rules ← f25,f43,f44,p36,p37
15. positioning-game-rules ← f51,p58,p59,p60,p62,p65,p66,p67 + 家族G(组织采纳) + 家族H(心态错觉)
