# 盲测结果 — vc-dynamics-demystified（标杆）

- 判卷方式：独立评审代理只看 16 skill 菜单（name+description），对 7 条 prompt 做选择题，未见 expected_behavior。
- 首轮 6/7：T3（风投内部一票否决/谁说了算）被误判给 vet-investors-and-advisors——原因是菜单中 #7 含"理解风投内部政治"措辞，与 #4 的决策机制重叠。
- 修正：#7 菜单描述改为"背调具体投资人"，风投整体决策机制归 #4；复测 T3 → 正确。
- 最终结果：**7/7 通过**。
- 给 builder 的约束：vet-investors-and-advisors 的 description 不得宣称"理解风投内部政治/整体决策机制"场景（那归 vc-dynamics-demystified）。
