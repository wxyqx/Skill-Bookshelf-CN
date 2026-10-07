# test-results — open-as-strategy

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨/影响力中心）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "先发制人开源 vs 命根子封闭"= u09 V2 novel question 的近题；判定动作：去道德化一问+两个封闭前提检验 |
| should-trigger-02 | 激活 | ✅ | "什么条件下才配选封闭"直接命中封闭两前提（p59/c39），并预置了"我们不是苹果"的正确直觉 |
| should-trigger-03 | 激活 | ✅ | "锁定用户/不许导出"撞反锁定条款（p60/退订自由）；预期动作：E5 反锁定自检 |
| should-not-trigger-01 | 转 default-open-candor | ✅ | 坏消息传不上来=讲真话的安全环境问题；"开放"同词不同层的头号混淆场景，两个 skill 的 A2 区分段互相写明 |
| should-not-trigger-02 | 不激活 | ✅ | 协议知识查询无战略判断；description 已写入"纯开源协议知识查询"的排除项 |
| edge-01 | 边界处理 | ✅ | 被动的合规交付不是战略选择；预期先分类再决定是否进入判定流程，不机械套框架 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 default-open-candor 的"信息开放 vs 战略开放"同词分界、与 technical-insight-first 的串联关系（封闭前提①由洞见之问回答）均验证通过。
- **自测发现的边界问题**: ①中文"开放"一词在两个 skill 间撞车是全书最大的同词混淆源——本 skill description 已写"不适用于组织内部信息透明"，但若用户 prompt 同时含内外两层（如"开放公司文化并开源产品"），应两 skill 串联激活而非互斥，判卷时需允许复合答案；②"护城河/锁定"字样也可能吸引 focus-user-think-10x（用户立场相近），区分靠"分发与生态策略 vs 方向与量级"，本次测试未覆盖该交叉，列为盲测时的补充诱饵候选。
