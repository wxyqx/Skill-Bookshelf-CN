# test-results — innovation-chaos

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "创新实验室+首席创新官+按创意数考核"= ce46 雅虎创新委员会的同构提案；判定动作：判自相矛盾、CEO 兼任、拆审批 |
| should-trigger-02 | 激活 | ✅ | "全靠老板立项+一线点子石沉大海+没人再提"= 指派制扼杀物竞天择的直接命中（f41/p179） |
| should-trigger-03 | 激活 | ✅ | "疯原型没人敢跟进"= 第一追随者缺失（f42）的原型场景；输出含低摩擦加入机制与部门分布检查 |
| should-not-trigger-01 | 不激活 | ✅ | 单点子可行性评审 ≠ 环境设计；B 段反场景明确排除，不会拿"混沌"哲学回答市场大小问题 |
| cross-decoy-01 | 转 twenty-percent-time | ✅ | 方向已定（给自由时间），问的是细则（可攒/绩效/报备）→ twenty-percent-time；本 skill 只在"该不该管创新/怎么营造环境"层接手。两 skill 的 A2 区分段（环境总纲 vs 制度细则）互相写明 |
| edge-01 | 边界处理 | ✅ | "拿混沌当流程豁免"触发 B 段拒绝项：混沌=创意生产方式，非质量与责任豁免；并给出过滤器/检验标准的补位转介 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 twenty-percent-time 的"环境/制度"分界、与 focus-user-think-10x 的"来源/量级"分界、与单点子评审的边界均验证通过。
- **自测中发现的边界问题**: innovation-chaos 的 related_skills 按任务要求留空，但其 A2 实际承担了给 twenty-percent-time / focus-user-think-10x 派流的入口职责——若未来加链接，composes-with twenty-percent-time（作为其环境前提）是最自然的一条。另注意 should-trigger-01 若用户追问"那实验室里的人干什么"，会滑向 org-design-rules 的组织设计问题，自测按主诉"要不要设创新官"判定。
