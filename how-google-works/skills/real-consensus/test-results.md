# test-results — real-consensus

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "点头同意+执行打折扣"= ce34 摇头娃娃原型；判定动作：追溯漏掉的异议+两条明路 |
| should-trigger-02 | 激活 | ✅ | "主持者已有倾向"= p130 负责人最后表态的直接场景 |
| should-trigger-03 | 激活 | ✅ | "共识=人人同意？"是定义级误读，I 段第一句即纠偏 |
| should-not-trigger-01 | 不激活 | ✅ | 紧急事故无共识流程空间（B 段反场景）；18 个 skill 中决策框架类也不该抢（指挥链止损优先） |
| cross-decoy-01 | 转 hippo-resistance | ✅ | "总监一开口大家都同意"= 权力污染而非流程缺失；两 skill A2 区分段互写（河马→权重，共识→流程） |
| edge-01 | 边界处理 | ✅ | 按决策量级开关：琐碎可逆不走流程，重大难逆才走；与人数无关 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 hippo-resistance 的"权重/流程"分界、与 decision-timing-discipline 的"质量/时限"分界、与 default-open-candor 的依赖关系（文化底座 vs 决策流程）均验证通过。
- **自测局限**: 用例与判卷出自同一主流程，存在自我合理化风险；最脆弱边界是 cross-decoy-01（"开会没人说真话"两类场景共用措辞），若盲测误触发应回炉 A2 区分段。
