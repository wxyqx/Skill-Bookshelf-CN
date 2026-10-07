# test-results — decision-timing-discipline

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "拖四个月+再调研一下"= ce36 原型；判定动作：两轮无增量→PIA→响铃 |
| should-trigger-02 | 激活 | ✅ | "琐事淹没+核心业务没时间"= 少做决策与 80/80 的双重命中 |
| should-trigger-03 | 激活 | ✅ | "法务拖三周"= ce39/c59 直接对应；判定动作：嵌入团队+马背上路，并保留强合规例外 |
| should-not-trigger-01 | 不激活 | ✅ | 紧急事故无决策空间（B 段反场景第一项），指挥链优先 |
| cross-decoy-01 | 转 real-consensus | ✅ | "决策已做、反对者怠工"= 共识后效问题；两 skill A2 区分段互写（讨论充分了但不拍板→本 skill；拍板了不挺身→real-consensus） |
| edge-01 | 边界处理 | ✅ | "期限 vs 新信息"的张力按 p134 处理：实质增量调期限，无增量按期拍板；E 段步骤 4 有对应判据 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 real-consensus 的"时限/质量"分界、与 hippo-resistance 的"结构/权力"分界、与 ship-iterate-fail-well 的"上马/迭代"衔接均验证通过。
- **自测局限**: 用例与判卷出自同一主流程，存在自我合理化风险；最脆弱边界是 edge-01（期限刚性的反向场景），若盲测发现 agent 一律"按期拍板"或一律"顺延"，应回炉 E 段步骤 4 的判据表述。
