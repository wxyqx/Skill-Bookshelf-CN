# inspired-skills

由《启示录：打造用户喜爱的产品》（*INSPIRED: How to Create Tech Products Customers Love*）蒸馏出的一组**可被 AI Agent 调用的技能**（Skills）。

> 九成产品失败的根本原因，是没有人专职做"探索产品"这件事——
> 产品经理的本职是探索出**有价值的、可用的、可行的**产品，
> 在写第一行代码之前，用高保真原型和真实用户验证这三点；
> 因为"如果产品没有市场价值，无论开发团队多么优秀也无济于事"。
> 本项目把这套方法提炼成 18 个原子化技能。

---

## 来源

| | |
|---|---|
| **书名** | 启示录：打造用户喜爱的产品（*INSPIRED*） |
| **作者** | Marty Cagan（曾任惠普程序员、网景平台及工具部门副总裁、eBay 产品管理及设计高级副总裁） |
| **出版** | 英文原版 2008 / 中文版 2011（华中科技大学出版社，七印部落 译） |
| **蒸馏工具** | cangjie-skill（仓颉：把长内容蒸馏成可调用技能的流水线） |
| **蒸馏方法** | RIA-TV++（整书理解 → 并行提取 → 三重验证 → RIA++ 构造 → 链接 → 压力测试 → 交付） |

---

## 如何选用（场景导航）

- **要不要做这个想法** → 先跑 `opportunity-assessment-ten-questions`（十问只问问题不谈方案）
- **想法通过、要动手了** → `discovery-execution-two-modes` 切换重心 → `hi-fi-prototype-as-spec` 造原型 → `product-validation-trio` 做三验证 → `prototype-testing-playbook` 学会测试操作
- **范围失控、要砍功能** → `minimal-product-definition`（通过测试后不可削减，超支只延工期）
- **想找人帮你打磨** → `charter-user-program`（特约用户 ≠ 尝鲜者）+ `persona-driven-focus`（每版聚焦一类人）
- **团队吵不出结果** → `product-principles-priority`（分歧的本质是优先级没对齐）
- **大客户/大单提特殊要求** → `special-product-defense`（接特例 = 改行做定制软件商）
- **搞不清用户要什么** → `user-research-limits`（调研能完善产品，定义不出产品）+ `irrational-user-signals`（警惕技术爱好者，研究愤怒的用户）
- **产品卖不动** → `emotion-based-demand`（企业买恐惧贪婪，大众买孤独自豪）+ `new-old-thing`（老需求+新技术）
- **改老产品、发布与善后** → `metric-driven-improvement` → `smooth-deployment` → `rapid-response-window`
- **开发喊"要重写代码"** → `tech-headroom-20percent`（20% 余量是产品生存保险）

---

## 18 个技能

### 立项与探索

- [`opportunity-assessment-ten-questions`](skills/opportunity-assessment-ten-questions/SKILL.md) — **机会评估十问**：只问问题不谈方案的十连问，淘汰馊主意，防"把洗澡水和孩子一起泼掉"
- [`discovery-execution-two-modes`](skills/discovery-execution-two-modes/SKILL.md) — **探索与执行两阶段**：定义产品是艺术不可设期限，用流水线并行收纳中途新需求
- [`product-validation-trio`](skills/product-validation-trio/SKILL.md) — **三验证**：价值/可用性/可行性在写代码前用同一个原型同时验证，缺一即败
- [`minimal-product-definition`](skills/minimal-product-definition/SKILL.md) — **基本产品**：通过用户测试后不可再削减，超支只延工期（断腿的狗打不了猎）
- [`hi-fi-prototype-as-spec`](skills/hi-fi-prototype-as-spec/SKILL.md) — **高保真原型即文档**：原型取代纸质 PRD，可测试才合格，原型代码全部废弃

### 用户与验证

- [`charter-user-program`](skills/charter-user-program/SKILL.md) — **特约用户计划**：≤10 个免费开发伙伴，招不到特约用户 = 需求不成立
- [`prototype-testing-playbook`](skills/prototype-testing-playbook/SKILL.md) — **原型测试操作法**：鹦鹉技巧代替引导，连续六位理解价值即收工
- [`user-research-limits`](skills/user-research-limits/SKILL.md) — **市场调研的边界**：调研能回答"谁在用"，回答不了"该打造什么"
- [`persona-driven-focus`](skills/persona-driven-focus/SKILL.md) — **人物角色聚焦**：决定谁不是目标用户同样重要，宣称老少皆宜是自欺欺人
- [`irrational-user-signals`](skills/irrational-user-signals/SKILL.md) — **非理性消费者信号**：技术爱好者最没参考价值，研究愤怒的用户（新生测试）

### 决策与方向

- [`product-principles-priority`](skills/product-principles-priority/SKILL.md) — **产品原则与优先级共识**：方案之争的病根是目标优先级没排序
- [`special-product-defense`](skills/special-product-defense/SKILL.md) — **特例产品防御**：混淆客户需求与产品需求，接了就被合同绑死
- [`emotion-based-demand`](skills/emotion-based-demand/SKILL.md) — **情感需求分析**：企业级买恐惧与贪婪，大众买孤独、爱与自豪
- [`new-old-thing`](skills/new-old-thing/SKILL.md) — **新瓶装老酒**：成功产品多是老需求+更好的新瓶，不必寻找全新市场

### 增长与运维

- [`metric-driven-improvement`](skills/metric-driven-improvement/SKILL.md) — **指标驱动改进**：别当功能加工厂，注册转化 9%→18% 收益就能翻倍
- [`smooth-deployment`](skills/smooth-deployment/SKILL.md) — **平滑部署**：新旧版本并行过渡，不要轻易试探用户的耐心
- [`rapid-response-window`](skills/rapid-response-window/SKILL.md) — **快速响应阶段**：发布后一周是黄金窗口，关键不是会不会出问题而是多快解决
- [`tech-headroom-20percent`](skills/tech-headroom-20percent/SKILL.md) — **20% 技术余量**：预留自主时间防"重写代码危机"，eBay 三次重写的教训

---

## 相关文档

- [docs/BOOK_OVERVIEW.md](docs/BOOK_OVERVIEW.md) — 整书理解（骨架/术语/批判）
- [docs/DIGEST.md](docs/DIGEST.md) — 精华长文（不读全书看这篇，约 8800 字）
- [docs/INDEX.md](docs/INDEX.md) — 技能总览 + 引用图 + 推荐学习顺序
- [docs/GLOSSARY.md](docs/GLOSSARY.md) — 25 条共享术语词典
- [docs/verified.md](docs/verified.md) — 三重验证通过记录（18 通过 / 23 淘汰）
- [docs/test-results.md](docs/test-results.md) — 压力测试报告（126/126 盲测通过）
- [docs/candidates/](docs/candidates/) · [docs/rejected/](docs/rejected/) — 提取候选池与淘汰审计
