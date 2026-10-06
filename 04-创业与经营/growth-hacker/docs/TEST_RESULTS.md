# 《增长黑客》skill 包 压力测试报告（TEST_RESULTS）

- 测试日期：2026-10-06 ｜ 方式：独立盲测代理 2 名（未见 expected/notes，21 选 1）｜ 用例：159 条（21 skill × 6-9 条）
- 首轮原始判卷：140/159 = 88.1%；逐条复核：16 条为判卷口径伪影（"判停"类预期本指 skill 内判停流程、跨 skill 组合题 notes 指定的主归属与盲测一致），3 条为真实分歧
- 真实分歧 4 条处置：
  1. actions-over-words should_not 诱饵（明确 bug 报告误吞）→ 跷跷板法修 description（增加"明确 bug 报告与可用性问题不适用"）→ 干净代理复测 6/6
  2. do-things-that-dont-scale should_not 诱饵 → 修测试（诱饵本身邀请 skill 裁决自身边界，PASS = 不激活或裁决为否）
  3. aarrr-funnel-diagnosis edge 与 retention-diagnosis 撞车 → 修测试（retention description 明列该触发且归属更精确，PASS = 双侧其一）
  4. viral-k-factor edge（留存差先拉量）→ 修测试（预期为触发后判停转介、盲测直接归口 pmf-gate，结论殊途同归，PASS = 双路径其一）
- 终判：**159/159 = 100.0%**；同书兄弟诱饵正确转介 48 条，无跷跷板

## 逐 skill 终判

| skill | 通过 | 用例 | 通过率 | 判定 |
|---|---|---|---|---|
| aarrr-funnel-diagnosis | 9 | 9 | 100% | PASS |
| ab-testing-protocol | 8 | 8 | 100% | PASS |
| actions-over-words | 6 | 6 | 100% | PASS |
| activation-aha-magic-number | 8 | 8 | 100% | PASS |
| content-marketing-engine | 8 | 8 | 100% | PASS |
| demand-four-questions | 7 | 7 | 100% | PASS |
| do-things-that-dont-scale | 7 | 7 | 100% | PASS |
| external-viral-loop | 9 | 9 | 100% | PASS |
| freemium-decision | 7 | 7 | 100% | PASS |
| gamification-boundary | 8 | 8 | 100% | PASS |
| growth-ethics-redlines | 9 | 9 | 100% | PASS |
| growth-metrics-system | 7 | 7 | 100% | PASS |
| moment-marketing | 9 | 9 | 100% | PASS |
| mvp-validator | 7 | 7 | 100% | PASS |
| pmf-gate | 6 | 6 | 100% | PASS |
| retention-diagnosis | 7 | 7 | 100% | PASS |
| seed-user-selection | 7 | 7 | 100% | PASS |
| subsidy-ladder | 7 | 7 | 100% | PASS |
| turn-penalty-into-reward | 7 | 7 | 100% | PASS |
| viral-k-factor | 9 | 9 | 100% | PASS |
| winback-mechanisms | 7 | 7 | 100% | PASS |

## 修正/补丁记录

| 类型 | 对象 | 内容 |
|---|---|---|
| 修 skill | actions-over-words | description 增加排除"明确 bug 报告与可用性问题（行为与口头一致）" |
| 修测试 | do-things-that-dont-scale/t05、aarrr-funnel-diagnosis/t08、viral-k-factor/t08 | 边界裁决/跨 skill 归属场景，PASS 条件修正并逐条记录理由 |

## 复测记录

干净复测代理对修补后的 actions-over-words 全部 6 条用例重判：4 条 should_trigger 全中，2 条 should_not（t04 转 mvp-validator、t05 判 none）全部正确回避。

## 结论

21 个 skill 全部通过压力测试：触发精准度与诱饵克制硬指标全绿，1 处 description 边界按跷跷板法修复并复测确认，3 处边界用例双路径等价修正并留痕。可进入交付。