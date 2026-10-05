# test-results — expel-villains-protect-stars

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨/影响力中心）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | 抢功+打压异议=把私利置于集体之上，判据直接命中（u05 V2 novel question 的镜像）；"能人难搞正常"恰是要反驳的混淆 |
| should-trigger-02 | 激活 | ✅ | "立规矩怕误伤高产出怪才"= ce15/保护明星一侧的原型场景 |
| should-trigger-03 | 激活 | ✅ | "开始有人模仿坏做派"= ce16 临界点的标准预警信号（warning_signs 原文） |
| should-not-trigger-01 | 转 retention-playbook | ✅ | 能力强+成长停滞+被挖=留汰律的挽留场景；品行无亏，本 skill 不接手；两个 skill 的 A2 区分段互相写明 |
| should-not-trigger-02 | 转 talent-portrait | ✅ | 能力测评≠品行拦截；博兹沃茨法则管的是对无权势者的态度，不是技术深度 |
| edge-01 | 边界处理 | ✅ | 判据是利益指向不是相处舒适度（E1 判停条件）；说话冲无私利事实→不贴标签，给协作反馈 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 retention-playbook 的"品行 vs 绩效/挽留"分界、与 talent-portrait 的"品行 vs 能力"分界、与 hippo-resistance 的"品行 vs 话语权"分界均验证通过。
- **自测发现的边界问题**: ①"保护明星"与"挽留明星"（retention-playbook）在语言信号上极易撞车（都含"明星员工"），靠"品行有亏与否"切分——若用户同时问品行与去留，两 skill 应串联而非互斥；②"恶棍判定权在管理者"的程序正义缺口（B 段作者盲点）意味着 edge 场景若涉及"上司说他是恶棍但无事实"，skill 应先要事实再判——此约束写在 E1，但描述字段未强调，存在被绕过的风险。
