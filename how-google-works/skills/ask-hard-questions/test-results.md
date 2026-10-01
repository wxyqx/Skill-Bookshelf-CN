# test-results — ask-hard-questions

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "战略会缺真问题+没人敢提被 AI 绕过"= c69/ce53 的合流场景；判定动作：可能语法改写+摆上台面+跟进机制 |
| should-trigger-02 | 激活 | ✅ | "怀疑中台被 Agent 绕过但证据不足、提过被'再看看'"= V2 novel_question 镜像；核心主张（不要求确凿证据+配反方与复查）直接命中 |
| should-trigger-03 | 激活 | ✅ | "组织体检+自检清单"= p212 清单的直接请求；输出含平台之辨与三问 |
| should-not-trigger-01 | 不激活 | ✅ | 投资人 PPT 要的是销量数字 = 预测请求；本 skill 恰恰拒绝"一定会怎样"，E1 判停条件覆盖 |
| cross-decoy-01 | 转 default-open-candor | ✅ | "不说真话/坏消息私下聊"缺的是安全环境与通道 → default-open-candor；本 skill 管难题的语法、公开化与跟进。A2 区分段（环境基建/提问内容）互相写明，两 skill composes-with 关系已声明 |
| edge-01 | 边界处理 | ✅ | 个人职业焦虑 ≠ 组织自检：答案为条件化——借用提问语法、注明层级差异，不照搬组织级步骤（B 段盲点外推的自检） |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 default-open-candor 的"环境/内容"分界、与 technical-insight-first 的"承认裂缝/选方向"分界、与预测式请求的边界均验证通过。
- **自测中发现的边界问题**: should-not-trigger-01 的诱饵"预测 2027 销量"与 should-trigger-02 的"怀疑被绕过"表面都是"谈未来"，区分基准是用户要"数字"还是要"不安"——已在 description 的不适用条款写明"市场预测/行业规模测算"。另注意 should-trigger-02 若用户接着问"那讨论会怎么开、怎么让所有人发言"，应联动 real-consensus。
