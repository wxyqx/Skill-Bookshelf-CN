# test-results.md — 阶段 4 压力测试报告

- 测试日期: 2026-10-01
- 测试对象: 18 个 skills（全部）
- 测试方式: **独立 sub-agent 盲测**（3 个干净的评审 agent，每人 42 条，互不知晓预期答案与测试类型）
- 用例总量: 126 条（should_trigger 72 / should_not_trigger 36 / edge_case 18），每 skill 7 条

## 判卷规则

- `should_trigger`: 盲测 matched == 本 skill → 通过
- `should_not_trigger`: 盲测 matched != 本 skill → 通过（诱饵容错为 0）
- `edge_case`: 对照 expected_behavior 的边界理由人工终审（不要求路由选择逐字一致，要求边界结论一致）

## 结果总览

| skill | should_trigger | should_not_trigger | edge_case | 结论 |
|---|---|---|---|---|
| opportunity-assessment-ten-questions | 4/4 | 2/2 | ✓（判 none，识别"事后补票"排除项正确） | 通过 |
| discovery-execution-two-modes | 4/4 | 2/2 | ✓（用框架判断"技术改造属执行性工作"） | 通过 |
| product-validation-trio | 4/4 | 2/2 | ✓（无 UI 产品的红线不豁免） | 通过 |
| minimal-product-definition | 4/4 | 2/2 | ✓（死线场景为已知盲区，不机械复读） | 通过 |
| hi-fi-prototype-as-spec | 4/4 | 2/2 | ✓（小团队载体可灵活，测试红线不豁免） | 通过 |
| prototype-testing-playbook | 4/4 | 2/2 | ✓（先解决"接触不到用户"前置障碍） | 通过 |
| charter-user-program | 4/4 | 2/2 | ✓（付费联合设计委员会≠特约用户计划） | 通过 |
| product-principles-priority | 4/4 | 2/2 | ✓（排期之争不归产品原则管） | 通过 |
| persona-driven-focus | 4/4 | 2/2 | ✓（人物角色≠广告定向包） | 通过 |
| emotion-based-demand | 4/4 | 2/2 | ✓（品牌情绪板属营销域，不激活） | 通过 |
| irrational-user-signals | 4/4 | 2/2 | ✓（活跃者优先恰恰该排除） | 通过 |
| special-product-defense | 4/4 | 2/2 | ✓（先定性"通用 vs 定制"再转出） | 通过 |
| metric-driven-improvement | 4/4 | 2/2 | ✓（发布次日掉转化→归 rapid-response-window） | 通过 |
| smooth-deployment | 4/4 | 2/2 | ✓（安全补丁不过渡仪式，排除项正确） | 通过 |
| rapid-response-window | 4/4 | 2/2 | ✓（窗口可压缩，发布不可无人值守） | 通过 |
| new-old-thing | 4/4 | 2/2 | ✓（照抄竞品不是"新瓶装老酒"背书） | 通过 |
| user-research-limits | 4/4 | 2/2 | ✓（A/B 测试属完善层，不触发定义警告） | 通过 |
| tech-headroom-20percent | 4/4 | 2/2 | ✓（第29章 20% 创新法则≠技术余量） | 通过 |

**总体: 126/126 = 100% 通过**（其中明确判分 108/108，edge_case 人工终审 18/18 边界结论一致）

## 跨 skill 混淆测试（硬性要求项）

36 条诱饵中含 18 条兄弟混淆场景（每 skill 至少 1 条"应触发同书另一个 skill"的 prompt），盲测在拿到全 18 skill 目录的选择题形式下**全部正确改判**，例如：

- "大客户要求定制一版才续签" → special-product-defense（而非 opportunity-assessment）
- "2000 份问卷说用户最想要高级筛选" → user-research-limits（而非 prototype-testing-playbook）
- "低月活功能按数据下线" → metric-driven-improvement（而非 minimal-product-definition）
- "发布次日转化掉 3 个点" → rapid-response-window（而非 metric-driven-improvement / smooth-deployment）
- "谷歌式 20% 创新时间申请" → none（tech-headroom-20percent 正确忍住）

## 局限声明（审计用）

1. 盲测为**路由层测试**（would_trigger + 第一动作），未盲测激活后的完整输出质量；执行层正确性由 E/B 段的判停条件约束。
2. 测试用例由独立于构造者的 agent 设计，但与 description 同源于 A2/B 段，存在设计同源偏置——诱饵与 description 的对齐可能高于真实分布。后续 darwin 进化（ratcheting）可用真实调用数据矫正。
3. 2 条 edge 的路由选择与 expected 存在分歧（opportunity-assessment::edge-01 判 none 而非"激活解释边界"；irrational-user-signals::edge-01 判 charter-user-program 而非本 skill），但两者的**边界结论**与 expected 一致，判为通过并在此留档。

## 结论

18/18 skill 通过压力测试（≥80% 线），无需回炉。进入阶段 5 交付。
