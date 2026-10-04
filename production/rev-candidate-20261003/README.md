# 製造データ候補 2026-10-03

## 状態

**REVIEW ONLY / 発注禁止**

KiCad 9.0.6で最新のKiCad 9設計から再生成した候補です。ZIPの展開テストは成功していますが、次のゲートが未完了です。

- R611は回路図上の値が`DNF`だがDNP属性が未設定で、BOMとpositions.csvへ実装対象として出力されている
- DRCの除外済みシルク警告13件について、量産設計としての個別承認がない
- Gerberビューアによる全層の独立目視確認が未実施
- BOMの空欄メーカー／MPN、先頭空白を含むLCSC番号、代替部品を未精査
- 実装業者に合わせたCPL座標・回転・面の照合が未実施
- PCB改版番号が確定していない

## 生成元

| ファイル | SHA-256 |
| --- | --- |
| `1000base-t1-converter.kicad_pcb` | `39f19e0db8caf9f3ee50c4f104040aa54f8d8428ede1d6f5c5506d4c71c6c89a` |
| `1000base-t1-converter.kicad_pro` | `04e3a872d091ac316b95ced9243e1744807b8d18f09c49d4c0c43a7c4322b8a2` |
| `1000base-t1-converter.kicad_sch` | `8671466f502bb807748ccc2ea3cad4585c9afba949d94d68f33a9b55802f8613` |
| `DP83867.kicad_sch` | `ea6dbeef47ba0d5e0bd44dba4850a7e887f1e323af9dff55cd907de02c6a82b6` |
| `DP83TG720.kicad_sch` | `2bfef88832683ec0fa30e439b523f9e7a96a52dbda9652bb8e640351c4304501` |
| `Power.kicad_sch` | `033050160d7e59a1da7220aea5fb30917da546387c32324bf1fee72fe70a14a6` |
| `RJ45.kicad_sch` | `be175a06a1691977088916a4aacf7e18c24b759a2b87d16f6a21169e9e2d5ceb` |
| `RP2040.kicad_sch` | `9a05cbad667cbf3bed45ec609839d20e31443f11df2af5036d3647b161567c9a` |

生成元は、このリポジトリの`hardware/`へ収録したKiCad 9設計です。設計が変更された場合、
この候補との同一性は上記ハッシュで判断します。

## 構成

- `gerber/`: 4層銅箔、ペースト、シルク、マスク、外形、PTH/NPTHドリル、ジョブファイル
- `assembly/bom.csv`: メーカー、MPN、LCSC番号を含むグループ化BOM
- `assembly/positions.csv`: 181フットプリントの実装位置（現時点では全てtop）
- `gerber-rev-candidate-20261003.zip`: 基板製造候補
- `assembly-rev-candidate-20261003.zip`: 実装候補

基板外形はEdge.Cutsの座標範囲から125 × 62 mmです。包装寸法ではありません。

## ZIP SHA-256

| ファイル | SHA-256 |
| --- | --- |
| `gerber-rev-candidate-20261003.zip` | `fab8a6460da0a6be730d73fbcc40a4952f79abf201c7ce58917c34c29af3895a` |
| `assembly-rev-candidate-20261003.zip` | `20e9eda32f95b6da56265c542a5356204abac931bfd297d8b1267c546bec60d0` |
