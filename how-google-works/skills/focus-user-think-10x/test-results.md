# test-results — focus-user-think-10x

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "竞品上了我们也要上"= 竞争注意力纪律的直接命中；判定动作：改写为用户侧语言+找未说出口的需求 |
| should-trigger-02 | 激活 | ✅ | "都很有把握完成"= OKR 全绿判据的原型场景；p187/p188 的镜像 |
| should-trigger-03 | 激活 | ✅ | 付费方（采购）与使用者（师生）分离 = c74/ce52 的镜像；站使用者的裁决有原文支撑 |
| should-not-trigger-01 | 不激活 | ✅ | 纯信息查询，description 明文排除；"竞品"字面信号不足以触发 |
| cross-decoy-01 | 转 technical-insight-first | ✅ | 痛点是"凭什么做成说不清"= 洞见之问；两个 skill 的 A2 区分段互相写明（depends-on 关系的前置位） |
| edge-01 | 边界处理 | ✅ | 赌注悖论前提是"输得起"；按 B 段先查生存约束与 70/20/10 桶位，不机械否决也不空谈 10 倍 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 technical-insight-first 的"根基/量级"分界、与 resource-70-20-10 的"目标/比例"分界均验证通过。

## 自测发现的边界问题（记录供阶段 5）

1. "聚焦用户"是通用口号，客服/公关类场景（"怎么回应用户投诉"）存在误触风险——description 已排除纯信息查询，但话术泛化风险需在真实部署中观察。
2. cross-decoy-01 依赖"说不清凭什么做成"这一信号与"方向"信号的权重区分：若用户同时问"为谁做"与"凭什么做成"，两 skill 应串联使用（先洞见后量级），而非二选一。
