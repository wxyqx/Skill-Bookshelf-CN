# TEST_RESULTS — 阶段 4 压力测试结果

> 测试方式：独立 sub-agent 盲测——盲测员未参与蒸馏，仅见全部 16 个 skill 的 name + description 与测试用例的 prompt 字面，做"16 选 1（含都不激活）"的判断；不参考 type / expected_behavior / expectation / notes。主流程再对照 test-prompts.json 判卷；每条用例的逐条判定见各 skill 的 test-results.md（盲测原始记录存档于流水线 stage4/blind-A|B|C.md 及复测记录）。

## 总体结果

- **16 / 16 skill 通过**（minimum_pass_rate = 0.8，最终全部 100%）
- 96 条用例：should_trigger 48/48，should_not_trigger 32/32，edge_case 16/16
- **诱饵容错为 0**：should_not_trigger 无一误激活，全部正确拒答或正确指向兄弟 skill
- **同书兄弟混淆诱饵 27 条**，全部正确指向兄弟 skill

## 触发修补记录（1 轮发现 → 2 轮修补 → 复测通过）

首轮盲测 95/96：property-rights-timing 的 1 条正面用例（改制方案遭媒体"贱卖国资"质疑、要不要开发布会回应）被盲测员判给 business-government-distance——两个 skill 对"被媒体质疑怎么回应"存在触发重叠。按"修 skill 而非修测试"原则：

1. 第一轮修补：给 property-rights-timing 增加"见光死"传播纪律触发、给 business-government-distance 增加让渡排除——复测发现跷跷板效应（政商 skill 的"旧改制历史被扒"正面用例被抢走）。
2. 第二轮精化：按场景本质切分边界——"产权改革推进中方案见光"的传播纪律归 property-rights-timing；"旧改制历史多年后被翻出的公开对峙姿态"归 business-government-distance，两侧互斥声明写进各自 description。
3. 干净盲测代理复测：两 skill 各 6/6 通过。

## 兄弟混淆诱饵一览（节选，全部通过）

| 本 skill | 混淆诱饵场景 | 正确指向 |
|---|---|---|
| policy-signal-capture | 观察官方表态温度而非听传言 | policy-thermometer-reading |
| policy-cycle-positioning | 只盯单一文件的条款含义 | dormant-clause-interpretation |
| red-hat-structure-decision | 产权清晰化的时机选择 | property-rights-timing |
| property-rights-timing | 恐慌期要不要戴红帽子 | red-hat-structure-decision |
| initial-identity-pricing | 已有存量企业的产权改革 | property-rights-timing |
| media-deification-cycle | 扩张目标是否脱离能力 | delusional-expansion-detection |
| delusional-expansion-detection | 泡沫期的退出时机 | bubble-exit-discipline |
| bubble-exit-discipline | 政策周期定位 | policy-cycle-positioning |
| business-government-distance | 改制方案"贱卖国资"攻击应对 | property-rights-timing |
| rent-based-model-audit | 政商姿态光谱设计 | business-government-distance |

## 边界用例要点（16 条，全部符合预期）

边界用例专门检验 skill 不被机械套用，包括：仿冒"边区效应"的线下零售选址不激活（marginal-zone-entry）、大企业套用后发者借力需判停（latecomer-resource-borrowing）、舆论危机中"树典型"与姿态设计的竞合（media-deification-cycle 与 business-government-distance 的边界）、产权自救与政商姿态的让渡（property-rights-timing ↔ business-government-distance 互斥声明生效）。
