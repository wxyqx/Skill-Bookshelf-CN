# test-results — hippo-resistance

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "CTO 一开口就定了"= 河马场景原型；判定动作：数据开场+质疑义务 |
| should-trigger-02 | 激活 | ✅ | "大老板在场+年轻同事有数据"= c55 案例的镜像 |
| should-trigger-03 | 激活 | ✅ | "一线知道但没人说"= 质疑义务缺失的直接命中 |
| should-not-trigger-01 | 不激活 | ✅ | 紧急事故指挥链清晰，B 段反场景直接覆盖 |
| cross-decoy-01 | 转 real-consensus | ✅ | 数据已共享、问题在"没有结论/没人支持"= 共识流程问题；两 skill A2 区分段互相写明 |
| edge-01 | 边界处理 | ✅ | 愿景/审美允许主观（B 段），但需区分决策类型回答，不是机械拒绝 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 real-consensus 的"权重/流程"分界、与紧急场景的边界均验证通过。
