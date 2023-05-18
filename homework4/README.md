# 作业4: Kulla-Conty BRDF

微表面模型的 BRDF(Microfacet BRDF) 存在一个根本问题，就是忽略了微平面间的多次弹射，这就导致了材质的能量损失，并且当材质的粗糙度越高时，能量的损失会越严重。
通过引入一个微表面BRDF 的补偿项，来补偿光线的多次弹射，使得材质的渲染结果可以近似保持能量守恒，这个BRDF 的补偿模型就是本轮作业需要重点完成的 Kulla-Conty BRDF 近似模型。
完成 Kulla-Conty BRDF 模型，关键在于计算 BRDF 的补偿项 fms，而 fms的计算需要 E(μ) 和 Eavg 两个前置变量。由此本轮作业将分为以下两个部分：

- 在离线端 (lut-gen 文件夹中) 预计算 E(μ) 和 Eavg。
- 在实时端(homework4 文件夹中) 通过查询预计算数据构建BRDF 的补偿项。

