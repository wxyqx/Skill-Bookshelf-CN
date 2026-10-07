# test-results — talent-portrait

- **测试方式**: fallback（主流程自测）。子代理盲测因配额/基础设施限制不可用；每条用例由主流程对照全部 18 个 skill 的 slug+positioning 做"该激活哪一个"判定。可信度低于独立盲测。

## 全部 18 个 skill 的判定基准（供混淆检查）

hippo-resistance（防高薪者意见）· org-design-rules（7法则/两个比萨）· expel-villains-protect-stars（恶棍与明星）· technical-insight-first（技术洞见替代计划）· open-as-strategy（开放战略）· focus-user-think-10x（聚焦用户往大处想）· hiring-quality-bar（招聘质量律）· talent-portrait（人才画像）· hiring-ops（招聘组织化）· retention-playbook（留汰律）· real-consensus（共识≠一致）· decision-timing-discipline（响铃/80-80/马背）· default-open-candor（默认开放/路由器）· resource-70-20-10 · twenty-percent-time · ship-iterate-fail-well · innovation-chaos · ask-hard-questions

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ | "两年前不存在的岗位+要求几年经验"= 画像/光圈场景原型（V2 novel_question 的直接镜像） |
| should-trigger-02 | 激活 | ✅ | "真的爱学习 vs 证书话术"= 学习型动物探测器+ce24 反信号，双重命中 |
| should-trigger-03 | 激活 | ✅ | "简历不对口但惊艳"= 加大光圈的定义场景（c47/ce26 镜像） |
| should-not-trigger-01 | 不激活 | ✅ | 背调核实是事务性话题，description 明文不在范畴 |
| cross-decoy-01 | 转 hiring-quality-bar | ✅ | "水准线上+先用着+不合适再换"= 标准取舍与兜底策略；画像方法已走完，非测量问题 |
| edge-01 | 边界处理 | ✅ | "投缘≠谷歌范儿"是 B 段明文的张力；用操作化评分纠偏，不机械否定老板观察 |

## 结果

- **通过率: 6/6 = 100%**（fallback 自测）
- **混淆检查**: 与 hiring-quality-bar 的"画像/律法"分界、与 hiring-ops 的"内容/流程"分界均验证通过。

## 自测发现的边界问题（记录供阶段 5）

1. "谷歌范儿/文化契合"是 18 个 skill 中最容易被泛化的信号：与 expel-villains-protect-stars（品行拦截）共用博兹沃茨法则，与 culture fit 面试只有"操作定义+四维之一"的差异——部署时若用户只说"看合不合得来"，应先区分是测量设计（本 skill）还是标准取舍（hiring-quality-bar）。
2. should-trigger-01 类新岗位画像与 hiring-ops 的最小流程设计常在同一对话出现（既要画像又要流程），串联使用为常态，单一激活判定会低估双 skill 场景。
3. "错失机遇之问"在面试题库类网站已有流传（原书 2014 年出版），题面需要随行业换血（ce27 的教训同样适用于本 skill 自己的工具）。
