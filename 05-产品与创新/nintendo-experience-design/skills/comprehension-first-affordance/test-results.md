# test-results — comprehension-first-affordance

- **测试方式**: fallback（主流程自测，方法同 intuition-design-loop/test-results.md）。

## 逐条判定

| id | 预期 | 判定 | 理由 |
|---|---|---|---|
| should-trigger-01 | 激活 | ✅ 通过 | "首屏堆卖点+转化低"是 A2 场景 1 原型；判定动作：语言素描逐项裁决 |
| should-trigger-02 | 激活 | ✅ 通过 | "演示第一页放什么"命中场景 1/4 |
| should-trigger-03 | 激活 | ✅ 通过 | "不知道第一步干嘛+信息全"命中场景 2，且正是 ce04 反例的镜像 |
| should-not-trigger-01 | 不激活 | ✅ 通过 | 校对任务无关 |
| cross-decoy-01 | 转兄弟 skill | ✅ 通过 | 文案没问题但学完即流失=排序/编排问题；判定：转 primacy-frontload-first-timers，教学方式配 intuition-design-loop。本 skill description 的不适用清单未明写此例，但 A2 区分段已覆盖——通过，记录一条改进备注：description 可补"教学顺序问题不适用" |
| cross-decoy-02 | 转兄弟 skill | ✅ 通过 | "改了三轮文案仍无效"=该诊断脉络（ psychological-context-redesign 的 A1 案例 3 正是此题）；判定：转 psychological-context-redesign |
| edge-01 | 边界外 | ✅ 通过 | B 段明写"纯品牌/审美场景"不适用；判定：美术馆展陈合法，但导视/说明牌仍属"了解优先"管辖——边界回答而非机械套用 |

## 结果

- **通过率: 7/7 = 100%**（fallback 自测）
- **改进备注（不影响通过）**: cross-decoy-01 的分界依赖 SKILL.md 的 A2 区分段而非 description 本身——宿主只读 name+description，若实机误触发，优先在 description 末尾补一句"不适用于教学顺序与节奏问题（见 primacy-frontload / fatigue-timing）"。
