# Hardware

KiCad 9で作成した1000BASE-T1コンバーター本体の設計データです。

`1000base-t1-converter.kicad_pro`を開いてください。回路図は次の階層シートに分かれています。

- `DP83867.kicad_sch`: 1000BASE-T PHY
- `DP83TG720.kicad_sch`: 1000BASE-T1 PHY
- `RJ45.kicad_sch`: RJ45インターフェース
- `RP2040.kicad_sch`: PHY管理マイコン
- `Power.kicad_sch`: 電源回路

製造データは[production/](../production/)にあります。

フットプリントと回路記号はKiCadファイルへ保存されています。3Dモデルの一部は
EasyEDA2KiCadのライブラリを参照するため、完全な3D表示にはKiCadで`EASYEDA2KICAD`
パス変数を設定してください。回路図・PCB編集と製造出力の確認には必須ではありません。
