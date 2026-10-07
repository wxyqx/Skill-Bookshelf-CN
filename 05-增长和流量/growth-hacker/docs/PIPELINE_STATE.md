# 增长黑客 — 流水线状态

- 书名: 《增长黑客：创业公司的用户与收入增长秘籍》 范冰 著（电子工业出版社 2015）
- 源: git@github.com:xdash/zengzhangheike-the-book.git 内 增长黑客-范冰.epub（正文约 20.9 万字，8 章 + 序 + 后记附录）
- slug: growth-hacker
- 分类: 04-创业与经营（booklist"流量的战略级理解"组，与 traffic-pool 同类）
- 节奏: 全自动；交付推 GitHub 后临时目录零残留

## 状态
- [x] 阶段 0 完成：4 组精读 116KB + BOOK_OVERVIEW 19KB
- [x] 阶段 1 完成：candidates/ 5 文件共 148KB（frameworks 34 + principles 36 + cases 23 + counter-examples 19 + glossary 28）
- [x] 阶段 1.5 完成：三重验证 → verified.md（29KB 级）
  - 输入 70 条 → 去重合并 21 个单元（8 个聚类域：PMF 验证 4 / 获客 3 / 激活 4 / 留存 3 / 收入 2 / 传播 3 / AARRR 元层 1 / 职业道德 1）
  - 淘汰 5 条（rejected/f18、f31、f32、p13、p32，均注明挂载项与素材去向）
  - 独立成 skill 率 21/70 = 30%（合并为主要压缩因子，正常区间下沿）
  - verified.md 含聚类总表（挂接 A1 案例/反例/术语 id）+ 降级素材注 + 全集群 2015 时效警示（9 条，元方法/参数层分离）
- [x] 阶段 2 完成：21 个 SKILL.md + test-prompts.json（进行中：按 verified.md 的 21 个 proposed_slug 构造，候选池中 cases/counter-examples/glossary 作 A1 素材挂接）
- [x] 阶段 3+4 完成：INDEX/GLOSSARY（21/21 链接）；盲测 159 用例终判 100%（首轮 88.1%，16 伪影+1 处 description 修复+复测 6/6+3 处边界留痕修正）
- [ ] 阶段 5 交付 → DIGEST（18KB）已写；待打包入库 04-创业与经营 + 推送

## 备注
- 阶段 1.5 的"用户轻确认 ★"按流水线"节奏: 全自动"配置跳过；淘汰名单与聚类已在 verified.md 供回溯。
- 阶段 2 硬约束：每个 skill 须通过 verified.md 末尾的时效警示校验——只保留判断逻辑层，2015 参数层（开放平台/补贴/SEO-ASO/微信规则/邮件生态/重定向 cookie）按当期重查或显式降权。
