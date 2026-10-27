# MATEnetアダプタ

本体CN201とMATEnet A-codeを、ツイストペア線で接続するケース付きアダプタです。

| フォルダ | 内容 |
| --- | --- |
| [hardware/](hardware/) | 基板Rev1のKiCadプロジェクト・回路図・PCB・専用ライブラリ |
| [case/](case/) | 上下ケースの造形用STL・編集用STEP |
| [production/](production/) | 基板Rev1のGerber ZIP・JLCPCB用BOM・実装位置データ |

## 構成と結線

基板は22 × 34 mm、厚さ1.6 mm、2層です。J1はTE Connectivity 2304372-1（MATEnet A-code）、J2はツイストペア線を手はんだする接続部です。電線のもう一端を本体側プラグ（C71370）に接続します。

| 信号 | 本体CN201・プラグ | 電線側J2 | MATEnet側J1 |
| --- | --- | --- | --- |
| T1_P | pin 1 | pin 1 | pin 1 |
| T1_N | pin 2 | pin 2 | pin 2 |

J1のシールド端子S1〜S6はアダプタ基板のGND銅箔につながっています。本体CN201へGNDを配線する構成ではありません。
接続方法は[取扱説明書](../docs/user-manual.md#matenetアダプタの結線)を参照してください。

## KiCadデータ

[hardware/cn201-matenet-pigtail.kicad_pro](hardware/cn201-matenet-pigtail.kicad_pro)をKiCad 9で開いてください。専用フットプリントと回路記号を同じフォルダに収録しています。

基板Rev1の回路図・PCBを収録しています。

部品メーカー由来の3Dモデルと、部品モデルを含むFreeCAD組立ファイルは収録していません。ケース形状はSTL・STEPで利用できます。

## ライセンス

JP WORKS作成の設計・ケース形状・文書は[CC BY 4.0](../LICENSE)で公開します。
