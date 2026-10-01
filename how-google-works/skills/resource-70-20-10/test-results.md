# test-results — resource-70-20-10

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | 核心/新兴/前沿三路抢 headcount = c77 三分类的原型场景；判定动作：70/20/10 配比+给 10% 设上限 |
| should-trigger-02 | 激活 | ✅ | 独立开发者 2000 小时 = V2 novel_question 镜像；有收入线（70）、有信号方向（20）、纯兴趣实验（10），且需提醒 10% 刻意给小 |
| should-trigger-03 | 激活 | ✅ | "砸了两千多万+只报好消息"= 牛顿过度投资偏见的直接命中（ce47）；输出含止损转介 ship-iterate-fail-well |
| should-not-trigger-01 | 不激活 | ✅ | 8 个功能的排期是单项目内优先级，B 段反场景明确排除；不与组合配置混淆 |
| cross-decoy-01 | 转 twenty-percent-time | ✅ | "每人一部分工作时间做自选项目"是自由时间制度细则 → twenty-percent-time；本 skill 管的是组织资源在项目群间的配比。两 skill 的 A2 区分段互相写明（时间档 vs 资源档） |
| edge-01 | 边界处理 | ✅ | E 段判停条件（无养家的 70% 不机械套比例）直接覆盖；回答应为条件化：保留克制精神、放弃比例形式 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 twenty-percent-time 的"资源档/时间档"分界、与 ship-iterate-fail-well 的"配比/止损"分界、与单项目排期的边界均验证通过。
- **自测中发现的边界问题**: edge-01（生存期）暴露出 SKILL.md 的 description 未把"核心业务未跑通"写进不适用清单——已在 description 与 E 段判停条件中补齐；另注意 cross-decoy-01 若用户同时追问"这个制度要占多少人力预算"，则两 skill 应先后激活（先 resource 后 twenty-percent-time 的细则），自测按"主诉是制度细则"判给 twenty-percent-time。
