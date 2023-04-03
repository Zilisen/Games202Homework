# 作业 3: Screen Space Ray Tracing

## 实现对场景直接光照的着色 (考虑阴影)

实现EvalDiffuse、EvalDirectionalLight和直接光照

![Direct_Light](images/Direct_Light.png)

## 实现屏幕空间下光线的求交 (SSR)

![LinearRaymarch](images/LinearRaymarch.png)

实现RayMarch并用镜面反射来验证正确性

![SSR_RayMarch](images/SSR_RayMarch.png)

## 实现对场景间接光照的着色

参考给出的伪代码实现间接光照

![Pseudocode](images/Pseudocode.png)

场景一，SAMPLE_NUM = 2

![SSR_1](images/SSR_1.png)

场景二，SAMPLE_NUM = 2

![SSR_2](images/SSR_2.png)

场景三，SAMPLE_NUM = 1(笔记本显卡拖不动了)

直接光照

![cave_direct](images/cave_direct.png)

间接光照

![cave](images/cave.png)

## 实现 Mipmap 优化的 Screen Space Ray Tracing

![SSR_Mipmap](images/SSR_Mipmap.png)