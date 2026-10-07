# test-results — hiring-ops

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "经理一人说了算+CEO 插手"= ce22 层级招聘的镜像；判定动作：收权归委员会+否决权 |
| should-trigger-02 | 激活 | ✅ | "反馈全是感觉不错"= 信息包与事实支撑制度的直接命中（p102） |
| should-trigger-03 | 激活 | ✅ | "面了7轮没结论"= ce28 原型；5 位封顶/30 分钟/强制表态三参数齐上 |
| should-not-trigger-01 | 不激活 | ✅ | 面试合规是法律话题，description 明文不在范畴；"面试"字面信号不足以触发 |
| cross-decoy-01 | 转 hiring-quality-bar | ✅ | 流程无争议、争议在"要不要将就"= 标准取舍；"流程/标准"分界与 quality-bar 的 A2 区分段互相写明 |
| edge-01 | 边界处理 | ✅ | 小团队按 E5 最小实现降规模（2 人+信息包+独立结论），并标注推演性质，不硬推完整编制 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 hiring-quality-bar 的"流程/标准"分界、与 talent-portrait 的"流程/内容"分界、与 decision-timing-discipline 的"场景参数/通用机制"分界均验证通过。

## 自测发现的边界问题（记录供阶段 5）

1. "面了 N 轮定不下来"同时踩中本 skill（5 位封顶）与 decision-timing-discipline（响铃）：判定规则是招聘场景参数归本 skill、跨场景的通用拖延机制转响铃——若用户是"自研还是收购僵持 3 个月"类非招聘决策，则应转 decision-timing-discipline。
2. edge-01 揭示的重装备问题：完整委员会（4-5 人+信息包+面试官委员会）对 10 人以下公司不成立，最小实现是推演而非书中原文，已在 E5 与 B 段双重标注，部署时不要伪装成原书主张。
3. "全员出动"信号（内推 KPI）与 hiring-quality-bar 的"高管亲自抓"信号部分重叠：前者是组织机制（本 skill），后者是标准执行人问题（quality-bar E4）——两者在同一对话出现时按"改机制 vs 守标准"分流。
