<!-- ELUCENIA technical documentation · gasto-energetico-por-mets · zh · no clinical/professional/rights approval -->

# 基于 METs 的能量消耗

[条件、来源与许可](https://elucenia.org/zh/tools/gasto-energetico-por-mets)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 活动强度（Compendium 值）

`met`

METs · 范围: 1–25

### 体重

`peso`

kg · 范围: 20–300

### 每次持续时间

`min`

min · 范围: 1–600

### 每周次数

`sessoes`

选填 · 范围: 1–14

## 方法版本

标准MET 3.5 mL O₂/kg/min；kcal/min=MET×3.5×kg/200；参考Compendium 2024

## 已记录的公式

kcal/min = METs × 3.5 × 体重 (kg) ÷ 200（1 MET = 3.5 mL O2/kg/min；每升O2约5 kcal）。

MET-min = METs × 分钟。等效近似：kcal ≈ METs × 体重 (kg) × 小时。

## 限制与适用人群

2024年成人活动汇编中的MET对应19–59岁成人活动；该版排除了≥60岁人群的数据。标准化值，包括估计值，不能测量个体能量消耗。儿童、老年人及特殊临床状况需要适合这些人群的来源和方法。

## 参考文献

- [Herrmann SD et al. 2024 Adult Compendium of Physical Activities: a third update of the energy costs of human activities. J Sport Health Sci, 2024.](https://doi.org/10.1016/j.jshs.2023.10.010)

- [Garber CE et al. Quantity and quality of exercise for developing and maintaining cardiorespiratory, musculoskeletal, and neuromotor fitness in apparently healthy adults. Med Sci Sports Exerc, 2011.](https://doi.org/10.1249/MSS.0b013e318213fefb)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

高强度（≥ 6 METs）

| 结果详情 | |
| --- | --- |
| 每分钟能量消耗 | 9.8 kcal/min |
| 训练量 | 240 MET-min |


### 2

中等强度（3 到 5,9 METs）

| 结果详情 | |
| --- | --- |
| 每分钟能量消耗 | 4.9 kcal/min |
| 训练量 | 158 MET-min |
| 每周总量 | 630 MET-min/周（达到 500 到 1000 的目标） |


### 3

轻度强度（< 3 METs）

| 结果详情 | |
| --- | --- |
| 每分钟能量消耗 | 2.6 kcal/min |
| 训练量 | 150 MET-min |

