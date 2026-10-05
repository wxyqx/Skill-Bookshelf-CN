# test-results — hiring-quality-bar

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "空了4个月+一般但能到岗"= 宁缺毋滥的压力测试原型；判定动作：成本并列+换路径不换标准 |
| should-trigger-02 | 激活 | ✅ | "还行但说不上哪里特别好"= 拿不准的直接命中；不对称法则裁决 |
| should-trigger-03 | 激活 | ✅ | 连续误聘复盘；两个自检问题直接可用（composes 串联见下方边界问题 2） |
| should-not-trigger-01 | 不激活 | ✅ | 谈薪话题，description 明文不在范畴；招聘语境不足以触发 |
| cross-decoy-01 | 转 hiring-ops | ✅ | "第8轮定不下来+没人担责"= 决策权与流程问题；"标准/流程"分界在两个 skill 的 A2 区分段互相写明 |
| edge-01 | 边界处理 | ✅ | 不硬扛不降标，换路径不换标准；已标注此为推演而非书中原文（B 段盲点） |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 hiring-ops 的"标准/流程"分界、与 talent-portrait 的"律法/画像"分界均验证通过。

## 自测发现的边界问题（记录供阶段 5）

1. "标准太高招不到人"与"流程太慢招不到人"在用户话术里常混在一起（如 should-trigger-03 的"标准还是流程"）：本 skill 应作为首选入口（先校准律法），再按判停条件转 ops；两者串联而非互斥。
2. "宁缺毋滥"对劳动密集型岗位不适用（B 段已排除），但用户若不说明岗位类型，需先反问岗位性质再套律法——description 已含"何时不调用"，实际部署建议先追问。
3. "宁漏聘不误聘"与 ce26（Instagram 漏聘之痛）存在内在张力：律法说漏聘代价小，案例说漏掉十亿美元创始人——正确读法是"拿不准时不录"针对**平均情形**，光圈与破例机制（talent-portrait）是它的对冲，两个 skill 需一起读。
