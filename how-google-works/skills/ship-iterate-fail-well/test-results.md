# test-results — ship-iterate-fail-well

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "修一个月完美再发 vs 先发收集反馈"= 交付-迭代的上线路径之争；判定动作：E1 卓越自检 → E2 低调上市 |
| should-trigger-02 | 激活 | ✅ | "迭代七轮日活仍平+要不要认输"= ce48 奇迹判据的直接命中；输出含止损 + 败得漂亮善后 |
| should-trigger-03 | 激活 | ✅ | "关停+团队情绪+传做创新会被优化"= c87 Wave 善后样板与观察者效应（p202）的直接命中 |
| should-not-trigger-01 | 不激活 | ✅ | 预算已批、只要执行排期 = 纯营销执行请求；本 skill 是发布策略的决策纪律，不接管已定方案的执行 |
| cross-decoy-01 | 转 resource-70-20-10 | ✅ | "预算怎么分/新方向要人"是项目群配比问题 → resource-70-20-10；本 skill 管单项目的发布节奏与止损。A2 区分段（配比 vs 节奏）互相写明 |
| edge-01 | 边界处理 | ✅ | 医疗场景触发 B 段合规反场景：答案为分层（交互层可迭代、诊疗与数据底线前置验证），非一刀切 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 resource-70-20-10 的"配比/节奏"分界、与 innovation-chaos 的"生/养葬"分界、与 decision-timing-discipline 的"决策时点/产品循环"分界均验证通过。
- **自测中发现的边界问题**: should-not-trigger-01 是本组最险的诱饵——"低调上市"原则容易让 agent 冲上去劝用户取消发布会；判定基准修正为：用户若问"该不该造势"则激活本 skill，若只要执行排期则不激活。另注意 should-trigger-02 若用户追问"砍掉后省下的人投给谁"，应联动 resource-70-20-10。
