<!-- ELUCENIA technical documentation · sistema-de-bethesda-tireoide · zh · no clinical/professional/rights approval -->

# 甲状腺细胞学 Bethesda 报告系统

[条件、来源与许可](https://elucenia.org/zh/tools/sistema-de-bethesda-tireoide)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 报告类别

`cat`

- `1` — I · 无法诊断
- `2` — II · Benigna
- `3` — III · 意义不明确的异型性（AUS）
- `4` — IV · 滤泡性肿瘤
- `5` — V · 可疑恶性
- `6` — VI · Maligna

## 方法版本

Bethesda甲状腺2023第3版：6个类别、ROM及核性/其他AUS；文献核查仅限所选类别代码

## 已记录的公式

六个诊断类别各有平均恶性风险（ROM）及预期范围，第三版2023更新：每类统一名称，AUS分核异型及其他异型。

## 限制与适用人群

Bethesda类别应来自甲状腺细针穿刺细胞病理报告，不能由计算器判定。平均风险及区间是该版本的估计值，并非个体诊断。2023版讨论了专门的儿科风险与管理；不能将成人值自动外推至儿童。 本次核查直接访问2023年文章仅获得出版社摘要；ROM表是在第三方转载的原始文章中查阅的，图像分辨率较低。转载的表2给出AUS范围13–30%，而同一文章正文给出20–32%。本次未对这些范围作出裁定。测试仅核查所选类别代码；成人ROM、儿科ROM及管理方案均未在本次核查中得到验证。

## 参考文献

- [Ali SZ et al. The 2023 Bethesda System for Reporting Thyroid Cytopathology. Thyroid, 2023.](https://doi.org/10.1089/thy.2023.0141)

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
