# test-results — org-design-rules

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨/影响力中心）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "12 个直接汇报+建议加 COO 层"= V2 novel question 原题：7 是下限，12 在安全区，是否加层只看有无影响力中心（u03 V2 推演） |
| should-trigger-02 | 激活 | ✅ | "重组拖两个月"= 重组纪律的直接命中（速战速决+敲定前实施，c20/p25） |
| should-trigger-03 | 激活 | ✅ | "每个部门都要自己的入口"= 产品痕迹检验（ce14/c21 的正面翻版） |
| should-not-trigger-01 | 转 expel-villains-protect-stars | ✅ | 抢功+打压异议=把私利置于集体之上，是品行判别问题；结构 skill 不应接手，A2/B 段分界写明 |
| should-not-trigger-02 | 不激活 | ✅ | 纯排版执行，无设计判断；"组织架构"字样不构成触发信号 |
| edge-01 | 边界处理 | ✅ | B 段明确"3–5 人初创是伪问题"（8 人同理），但两个比萨/影响力中心可作轻量参考——预期回答是边界澄清而非整段激活 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 expel-villains-protect-stars 的"结构 vs 品行"分界、与 hippo-resistance 的"结构 vs 话语权"分界、与纯执行任务的边界均验证通过。
- **自测发现的边界问题**: "7 的法则"数字极易被反向套用（按传统上限理解）——E1 已显式写"下限不是上限"，edge-01 进一步检验最小适用规模；对 8 人团队应回答"不需要"，skill 不应机械套参数。
