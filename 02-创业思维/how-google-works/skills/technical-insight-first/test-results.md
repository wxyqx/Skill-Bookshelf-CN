# test-results — technical-insight-first

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨/影响力中心）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "BP 写多细"= 计划姿态问题的原型；判定动作：原则文替代路线图+洞见之问（c01/c30） |
| should-trigger-02 | 激活 | ✅ | "调研说需求大 vs 工程说做不出"= 市场调查与洞见之争（ce05/p47）；评审第一问应是洞见之问 |
| should-trigger-03 | 激活 | ✅ | "计划还要不要守"= "计划可变，基础岿然不动"的直接命中（p45） |
| should-not-trigger-01 | 转 open-as-strategy | ✅ | 开源/封闭是分发与生态战略选择；本 skill 只负责其中的"技术洞见优势"前提检验，A2 区分段已写明串联关系 |
| should-not-trigger-02 | 不激活 | ✅ | 执行层排期在 B 段反场景内明确退出；'排期计划'与'战略计划'分界有效 |
| edge-01 | 边界处理 | ✅ | 稳定行业降级为自检而非一票否决（B 段"不否定一切计划"的延伸）；预期是分场景回答而非机械强制 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 open-as-strategy 的"过滤器 vs 战略选择"串联分界、与 ship-iterate-fail-well 的"根基 vs 节奏"分界、与运营排期的边界均验证通过。
- **自测发现的边界问题**: ①"计划必错"的口号容易被泛化为反一切规划——B 段与 E1 判停已设退出条件，但 description 里"不适用于成熟业务运营排期"的措辞在英文提问（operational planning）下可能不够醒目，是后续 A2 微调的候选点；②edge-01 类"稳定行业要不要问洞见"的答案有一定自由度（自检 or 一票否决），盲测环境下不同 agent 可能给出都合理但不同的判断，判卷时应接受"降级使用"与"仍强制提问"两种自洽回答。
