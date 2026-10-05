# test-results — retention-playbook

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "明星提离职+不想只靠加薪"= 留汰律原型场景；判定动作：诊断动因→发展对冲→1 小时窗口→alumni |
| should-trigger-02 | 激活 | ✅ | "骨干被扣、流动的全是边缘人"= ce31 巧克力囤积的直接命中 |
| should-trigger-03 | 激活 | ✅ | "继任者盯谁"= 接班人计划分支（f34）；与 talent-portrait 的区分：画像是招聘画像，接班是留汰侧，无冲突 |
| should-not-trigger-01 | 不激活 | ✅ | 绩效垫底者不属明星/高潜，B 段反场景直接覆盖；18 个 skill 中无招聘/留汰之外的匹配项 |
| cross-decoy-01 | 转 expel-villains-protect-stars | ✅ | "抢功+贬低同事"触发的是私利判别与清除问题；两 skill 的 A2 区分段互相写明（品行走驱逐、发展走留汰） |
| edge-01 | 边界处理 | ✅ | 应走电梯演讲分支而非"加薪或放行"二选一；E 段步骤 3 的分支条件可机械执行 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 expel-villains-protect-stars 的"品行/发展"出口分界、与 hiring-* 三 skill 的"进门/进门后"分界、与"反报价挽留"主流方法的区分均验证通过。
- **自测局限**: 用例与判卷出自同一主流程，存在自我合理化风险；cross-decoy-01 同时压到"明星"字面词，是本 skill 最脆弱的边界，若盲测发现误触发应回炉 A2 区分段。
