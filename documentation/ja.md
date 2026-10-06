<!-- ELUCENIA technical documentation · gasto-energetico-por-mets · ja · no clinical/professional/rights approval -->

# METsによるエネルギー消費量

[条件・出典・許諾](https://elucenia.org/ja/tools/gasto-energetico-por-mets)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 活動強度（Compendiumの値）

`met`

METs · 範囲: 1–25

### 体重

`peso`

kg · 範囲: 20–300

### 1回の時間

`min`

min · 範囲: 1–600

### 週あたりの回数

`sessoes`

任意 · 範囲: 1–14

## 方法の版

標準MET 3.5 mL O₂/kg/min；kcal/min=MET×3.5×kg/200；Compendium 2024参照

## 記載された計算式

kcal/min = MET × 3.5 × 体重 (kg) ÷ 200（1 MET = 3.5 mL O2/kg/min；O2の1リットル当たり約5 kcal）。

MET-min = MET × 分。等価な近似はkcal ≈ MET × 体重 (kg) × 時間。

## 限界・対象集団

2024年の成人用コンペンディウムのMETsは、19–59歳の成人の活動に対応し、この版からは≥60歳の人のデータが除外されました。推定値を含む標準化された値は、個人のエネルギー消費量を測るものではありません。小児、高齢者、特別な臨床状態には、その集団に適した出典と方法が必要です。

## 参考文献

- [Herrmann SD et al. 2024 Adult Compendium of Physical Activities: a third update of the energy costs of human activities. J Sport Health Sci, 2024.](https://doi.org/10.1016/j.jshs.2023.10.010)

- [Garber CE et al. Quantity and quality of exercise for developing and maintaining cardiorespiratory, musculoskeletal, and neuromotor fitness in apparently healthy adults. Med Sci Sports Exerc, 2011.](https://doi.org/10.1249/MSS.0b013e318213fefb)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

高強度（≥ 6 METs）

| 結果の詳細 | |
| --- | --- |
| 1分あたりの消費量 | 9.8 kcal/min |
| セッション量 | 240 MET-min |


### 2

中等度の強度（3～5,9 METs）

| 結果の詳細 | |
| --- | --- |
| 1分あたりの消費量 | 4.9 kcal/min |
| セッション量 | 158 MET-min |
| 週間量 | 630 MET-min/週（500～1000 の目標を満たす） |


### 3

軽度の強度（< 3 METs）

| 結果の詳細 | |
| --- | --- |
| 1分あたりの消費量 | 2.6 kcal/min |
| セッション量 | 150 MET-min |

