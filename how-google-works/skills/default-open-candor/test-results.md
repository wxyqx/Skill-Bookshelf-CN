# test-results — default-open-candor

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "要不要公开坏消息"= 举证倒置的判定场景；"担心军心不稳"正是 p148 明确排除的理由 |
| should-trigger-02 | 激活 | ✅ | "中层美化汇报"= ce43 双向过滤原型；判定动作：snippets 直连+10 秒规则 |
| should-trigger-03 | 激活 | ✅ | "全员会只有软球"= ce44/c65 直接对应；判定动作：多莉+红牌+领导者示范 |
| cross-decoy-01 | 转 open-as-strategy | ✅ | "开源换生态"是对外战略账；两 skill A2/B 段互写"同名不同层"（对外算收入，对内只谈真相） |
| should-not-trigger-02 | 不激活 | ✅ | 无差别群发=B 段反场景（ce45）；skill 若被激活也应以纠偏响应而非放大轰炸 |
| edge-01 | 边界处理 | ✅ | 区分"讲真话安全环境"与"转发未核实截图"：开正门（导入多莉/复盘通道）+管噪声，只堵不疏会坐实杀信使效应 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 open-as-strategy 的"对内/对外"分界、与 real-consensus 的"底座/流程"依赖关系、与信息轰炸的反向边界均验证通过。
- **自测局限**: 用例与判卷出自同一主流程，存在自我合理化风险；最脆弱边界有二——cross-decoy-01（"开放"一词共用）、should-not-trigger-02（"共享一切"的字面误用），若盲测发现误触发应回炉 A2 与 description 中"不调用"措辞。
