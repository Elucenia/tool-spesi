<!-- ELUCENIA technical documentation · spesi · zh · no clinical/professional/rights approval -->

# sPESI（简化 PESI）

[条件、来源与许可](https://elucenia.org/zh/tools/spesi)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 年龄 \> 80 岁

`idade`

### 癌症（活动性或过去一年治疗）

`cancer`

### 慢性心肺疾病（心力衰竭或慢性肺病）

`cardiopulm`

### 心率 ≥ 110 bpm

`fc`

### 收缩压 \< 100 mmHg

`pas`

### 氧饱和度 \< 90%

`sat`

## 方法版本

sPESI/Jiménez 2010：6二元变量、0低危其余高危；非11变量原PESI

## 已记录的公式

各一分: 年龄\>80、癌症、慢性心肺病、心率≥110、收缩压\<100、O₂饱和度\<90%. 0 = 低危; ≥ 1 = 高危 (sPESI).

## 限制与适用人群

sPESI估计急性肺栓塞的预后，不能确认或排除肺栓塞。研究中的低风险组仍发生死亡，不能单独授权门诊治疗。不稳定状态、合并疾病、临床因素及后勤条件应在对应方案中评估。

## 参考文献

- [Jiménez D et al. Simplification of the pulmonary embolism severity index for prognostication in patients with acute symptomatic pulmonary embolism. Arch Intern Med, 2010.](https://doi.org/10.1001/archinternmed.2010.199)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism developed in collaboration with the European Respiratory Society (ERS). Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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
