# test-results — twenty-percent-time

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "想搞谷歌那套 20% 时间+要不要规定周五下午"= 制度设计原型场景；判定动作：自由>时长，纠正打卡化（E1） |
| should-trigger-02 | 激活 | ✅ | "宣布了但没人真用/经理排满"= 名存实亡的直接命中（B 段+E5 存活自检） |
| should-trigger-03 | 激活 | ✅ | "采纳发 5% 奖金+排行榜"= p207 外部奖励挤出内在动机的反方向提案，核心主张（与钱无关）直接命中 |
| should-not-trigger-01 | 不激活 | ✅ | 下班后副业合规 ≠ 公司时间内的自主权制度；B 段反场景明确排除 |
| cross-decoy-01 | 转 innovation-chaos | ✅ | 创新委员会+创新指标是"给创新建官僚机构"（ce46/雅虎乌迪案例），属于环境哲学层 → innovation-chaos；本 skill 只管自由时间的制度细则。两 skill 的 A2 区分段（总纲 vs 制度）互相写明 |
| edge-01 | 边界处理 | ✅ | 律所计费制是跨行业迁移：答案为条件化激活——翻译成自选目标权+先检余量，而非照搬工时（B 段工程师中心盲点） |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 innovation-chaos 的"环境哲学/制度细则"分界、与 resource-70-20-10 的"时间档/资源档"分界、与副业管理的边界均验证通过。
- **自测中发现的边界问题**: should-trigger-01 中用户同时问了"怎么落地"与"要不要规定工时"，若 agent 只答后者会与 E 段脱节——已在 E1 加判停条件（要求先审批内容即回到 innovation-chaos）。另注意"内部黑客松规则"同时可能被 innovation-chaos 抢答：判定基准是用户问的是活动细则（本 skill）还是该不该办创新活动（innovation-chaos）。
