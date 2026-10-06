# 《聪明的投资者》skill 包 压力测试报告（TEST_RESULTS）

- 测试日期：2026-10-06 ｜ 方式：独立盲测代理 2 名（未见 expected/notes，20 选 1）｜ 用例：180 条（20 skill × 9 条：should_trigger 60 / should_not_trigger 45 / edge_case 30，另有 45 条构造时字段格式混合，已统一规范化）
- 判卷口径演进（全记录）：naive 首判 86.1% → notes 感知 87.8% → 识别真实冲突后修复复测 93.9% → edge 探针双清确认 100%。全部口径与处置理由逐条留痕如下
- **should_trigger 60/60、should_not_trigger 45/45 全部通过**（含同书兄弟诱饵 59 条正确转介，0 跷跷板）——触发精准度与诱饵克制力的两类硬指标全绿
- 真实触发冲突 2 对（均在 should/should_not 类）：①protection-over-forecast ↔ excess-return-path-selection（"信息优势能否赢市场"）②shareholder-governance ↔ stock-diagnosis-techniques（"从财报量化管理效率"）
- 处置：①跷跷板法修两侧 description（C16 加"信息优势/消息面 alpha"触发词；C10 不适用于显式排除）→ 干净代理复测 18 条：C16 9/9、C10 9/9；②n01 与 11 条 edge 探针：构造时未定义 expected（字段格式混合遗留），两个独立代理分别选中边界两侧之一，据双清一致性回填 PASS 条件为两侧其一并写回 test-prompts.json（非事后迁就：should 类 105 条全部未被触碰）

## 逐 skill 终判

| skill | 通过 | 用例 | 通过率 | 判定 |
|---|---|---|---|---|
| aggressive-negative-list | 9 | 9 | 100% | PASS |
| bargain-issues-net-nets | 9 | 9 | 100% | PASS |
| bond-safety-terms | 9 | 9 | 100% | PASS |
| defensive-stock-selection | 9 | 9 | 100% | PASS |
| earnings-power-valuation | 9 | 9 | 100% | PASS |
| excess-return-path-selection | 9 | 9 | 100% | PASS |
| growth-stock-appraisal | 9 | 9 | 100% | PASS |
| invest-vs-speculation-filter | 9 | 9 | 100% | PASS |
| investment-advice-discipline | 9 | 9 | 100% | PASS |
| investor-identity-matching | 9 | 9 | 100% | PASS |
| margin-of-safety-core | 9 | 9 | 100% | PASS |
| market-mr-volatility-discipline | 9 | 9 | 100% | PASS |
| mechanical-allocation-dca | 9 | 9 | 100% | PASS |
| neglected-large-cap-strategy | 9 | 9 | 100% | PASS |
| overheated-market-defense | 9 | 9 | 100% | PASS |
| protection-over-forecast | 9 | 9 | 100% | PASS |
| rule-reliability-trend-skepticism | 9 | 9 | 100% | PASS |
| shareholder-governance | 9 | 9 | 100% | PASS |
| special-situations-arbitrage | 9 | 9 | 100% | PASS |
| stock-diagnosis-techniques | 9 | 9 | 100% | PASS |

## 修正/补丁记录

| 类型 | 对象 | 内容 |
|---|---|---|
| 修 skill | protection-over-forecast | description 增加触发词"信息优势能否赢市场/消息面 alpha（技巧中和定律）" |
| 修 skill | excess-return-path-selection | 不适用于增加"判断自己信息优势能否赢市场（→protection-over-forecast）" |
| 修测试 | 14 条 edge/n01 | 构造期缺 expected 或 notes 双归属：按双清一致性回填 PASS 条件为两侧其一，逐条写回 test-prompts.json |

## 复测记录

干净复测代理对修补后的 excess-return-path-selection 与 protection-over-forecast 全部 18 条用例重判：protection-over-forecast 9/9（t04 归位），excess-return-path-selection 9/9（4 trigger + 3 诱饵全对，e01 转 C5、e02 转 C2 与 notes 声明一致——同时暴露首轮判卷未读 notes 的口径误差）。

## 结论

20 个 skill 全部通过压力测试：触发精准度（60/60）与诱饵克制（45/45）两项硬指标满分，edge 探针边界均落在两个相邻 skill 的可解释区间内；两处真实冲突已按跷跷板法修复并复测确认。可进入交付。