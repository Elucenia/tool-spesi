<!-- ELUCENIA technical documentation · spesi · ja · no clinical/professional/rights approval -->

# sPESI（簡易PESI）

[条件・出典・許諾](https://elucenia.org/ja/tools/spesi)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 年齢 \> 80 歳

`idade`

### がん（活動性または過去1年の治療）

`cancer`

### 慢性心肺疾患（心不全または慢性肺疾患）

`cardiopulm`

### 心拍数 ≥ 110 bpm

`fc`

### 収縮期血圧 \< 100 mmHg

`pas`

### 酸素飽和度 \< 90%

`sat`

## 方法の版

sPESI/Jiménez 2010：6二値変数、0低リスク他高リスク、11変数原PESIとは別

## 記載された計算式

各1点: 年齢\>80、がん、慢性心肺疾患、心拍数≥110、収縮期\<100、O₂飽和度\<90%. 0 = 低リスク; ≥ 1 = 高リスク (sPESI).

## 限界・対象集団

sPESIは急性肺塞栓症の予後を推定しますが、肺塞栓症を確定も除外もしません。研究の低リスク群でも死亡があり、単独で外来治療を許可するものではありません。不安定性、併存疾患、臨床因子、実施上の条件を、対応するプロトコルで評価する必要があります。

## 参考文献

- [Jiménez D et al. Simplification of the pulmonary embolism severity index for prognostication in patients with acute symptomatic pulmonary embolism. Arch Intern Med, 2010.](https://doi.org/10.1001/archinternmed.2010.199)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism developed in collaboration with the European Respiratory Society (ERS). Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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

低リスク：30日死亡率1,0%

他に支障がなければ、早期退院または在宅治療の候補（Hestia基準）。


### 2

低リスクではない：30日死亡率10,9%

ESCでは中等度リスク：右心室（心エコーまたはCT血管造影）とトロポニンを評価する。


### 3

低リスクではない：30日死亡率10,9%

ESCでは中等度リスク：右心室（心エコーまたはCT血管造影）とトロポニンを評価する。

