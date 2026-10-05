# verified.md — 三重验证总记录(阶段 1.5 产出)

> 《财务报表分析(简明版·立体化数字教材版)》张新民、钱爱民
> 候选池 224 条(frameworks 59 / principles 60 / cases 33 / counter-examples 25 / glossary 47)
> 验证范围:framework + principle + counter-example 共 144 条 → **通过 81 条(56%)**,淘汰 36 条(含跨文件并入),glossary 不做独立 skill(进 GLOSSARY.md),cases 不做独立 skill(进 A1 段与 DIGEST)。
> 详细 V1/V2/V3 判定:framework+principle 见 `_verify/verified_A.md`(58 条),counter-example 见 `_verify/verified_B.md`(23 条);淘汰原因见 `rejected/rejected_A.md`、`rejected/rejected_B.md`。
> 本文件记录合并去向:81 个通过单元 → **18 个 skill**。

## 最终 skill 方案(18 个)

| # | slug | 名称 | 包含单元 (orig_ids) |
|---|---|---|---|
| 1 | strategic-analysis-path | 战略视角综合分析路径 | v-A01(f03), v-A02(f56), v-A03(f57) |
| 2 | project-quality-entry | 项目质量分析总纲与审计意见入口 | v-A04(f04), v-A05(f09), v-A06(f06,pr40) |
| 3 | cash-quality-funding-risk | 货币资金质量与获现率诊断 | v-A07(f11), v-A08(f32,pr42), v-A09(pr43), v-B21(ce23), v-B10(ce12) |
| 4 | receivables-and-funneling | 商业债权质量与资金占用识别 | v-A10(f12,pr17), v-A11(f13,pr34), v-A12(pr22), v-A13(pr23) |
| 5 | inventory-and-margin | 存货与毛利率质量分析 | v-A14(f14), v-A15(f38,pr19) |
| 6 | long-term-asset-quality | 长期资产质量与减值判读 | v-A16(f15,pr20), v-A17(f16), v-A18(f18), v-A19(f19), v-A20(pr11,pr28) |
| 7 | asset-allocation-strategy | 资源配置战略透视 | v-A21(f20), v-A22(f30), v-A23(f36) |
| 8 | capital-structure-four-forces | 负债与资本结构质量(四大动力) | v-A24(f21), v-A25(f22), v-A26(f23+pr25-27), v-A27(f24), v-A28(pr59) |
| 9 | profit-quality-3d | 利润质量三维与核心利润 | v-A29(f25), v-A30(f26,pr06), v-A31(f29,f17), v-A32(f34,pr36), v-A33(pr38) |
| 10 | revenue-quality-three-questions | 收入质量三问 | v-A34(f27,pr37) |
| 11 | non-operating-income-quality | 非经营性损益判读 | v-A35(f33), v-A36(f35+pr32,33,41), v-A37(f39,pr39) |
| 12 | cash-flow-three-activities | 现金流量三性分析 | v-A38(f42,pr45), v-A39(f43,pr47), v-A40(f44,pr48), v-A41(f45,pr50), v-A42(f46,pr44), v-A43(pr46) |
| 13 | consolidation-pitfalls | 合并报表的局限与比率失真 | v-A44(pr12), v-A45(pr52), v-A46(pr53,pr56), v-A47(pr54), v-B20(ce22) |
| 14 | differential-analysis | 差量分析法 | v-A48(f47), v-A49(f48,f59,pr24), v-A50(f49), v-A51(f50), v-A52(f51), v-A53(f52,f53) |
| 15 | ratio-revision-rules | 常规比率修正纪律(含失灵机理) | v-A54(pr15), v-A55(pr29), v-A56(pr30), v-A57(pr31), v-A58(pr58), v-B18(ce20) |
| 16 | earnings-manipulation-tactics | 利润粉饰手法识别(十法) | v-B02(ce04), v-B03(ce05), v-B04(ce06), v-B05(ce07), v-B06(ce08), v-B07(ce09), v-B09(ce11), v-B12(ce14), v-B13(ce15), v-B19(ce21) |
| 17 | profit-deterioration-sweep | 利润质量恶化扫雷与业绩变脸 | v-B08(ce10), v-B11(ce13), v-B14(ce16), v-B15(ce17), v-B16(ce18), v-B17(ce19) |
| 18 | off-statement-strategy-blindspots | 报表之外的盲区(治理失效与并购战略) | v-B01(ce01), v-B23(ce25) |

**重叠消解**(验证官 A/B 两包方案的合并处理):
- B 包 `ratio-trap-corrections`(v-B18/20/22)拆解:v-B18 并入 #15(失灵机理与修正纪律同属一线),v-B20 并入 #13,ce24(格力误判/资产金融性负债率)与 v-A54 高度同源,归 #15 的 OPM 悖论主线。
- B 包 `cash-quality-funding-risk`(v-B10/21)并入 #3:v-A08(获现率检验+五类归因)与 v-B21(有利润没钱)是同一检验程序的正反两面。
- v-A31(三表对应总图)与 v-A30(利润表分层)同属利润口径纪律,归 #9。

## 质量门核对

- [x] 全部 81 单元 V1/V2/V3 三项通过(含 boundary_note 6 条,供 B 段引用)
- [x] 通过率 56%(144 条中),处于方法论文书合理区间(30-50% 上沿,反例池 92% 为高密度池属正常)
- [x] rejected/ 有完整淘汰记录(36 条,逐条注明 V 项与原因)
- [x] 用户轻确认:用户委托自治执行,最终方案在交付报告呈现

## 淘汰名单摘要(详见 rejected/)

- V3 常识/准则转述主力:审计意见五类型细节、抵销清单、法规体系、四假设转述、收付实现制缺陷、"要对比分析"、"看现金流"
- V1 单一语境:银行"三品"、新证券法条款、纯边栏存目案例
- 并入而非淘汰:27 条跨文件重复(如 pr25-27→f23、f59+pr24→f48)
