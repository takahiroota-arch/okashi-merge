# 発注シート ② お菓子＆アイテム（1枚に9個レイアウト）

このシートは **9個のアイテムを1枚の画像にグリッド配置**して一気に生成する指示です。
（あとで僕が1個ずつ切り出して使います）

## 出力
- 1枚の画像・**3列 × 3行 のグリッド（計9マス）**
- 背景：**透過PNG**（不可なら真っ白 #FFFFFF。各アイテムをはっきり離して配置）
- 推奨キャンバス：1536 × 1536 px（1マス 512×512、中央に配置・はみ出さない）
- 各アイテムは**同じ大きさ・同じ画風・等間隔**で、重ならないように

## 配置と内容（左上から右下へ）
| マス | アイテム | 内容 |
|---|---|---|
| 1（左上） | キャンディ | 丸い包み飴。うずまき模様。ピンク |
| 2 | クッキー | まる型クッキー。チョコチップ |
| 3（右上） | カップケーキ | 生クリームの渦＋さくらんぼ |
| 4 | ドーナツ | リング型。ピンクのアイシング＋スプリンクル |
| 5（中央） | ショートケーキ | 三角ショートケーキ。いちご1粒乗せ |
| 6 | プリン | カラメルがけのプリン |
| 7（左下） | ソフトクリーム | コーンの上に渦巻きクリーム |
| 8 | ホールケーキ | まるごとケーキ。いちご＆ろうそく |
| 9（右下） | スプーン | 縦長の角丸ブロックに銀のスプーン（おじゃま用・他と質感を変える） |

## 共通スタイル
- かわいい kawaii フラットイラスト／パステル／太めのクリーンな輪郭／ツヤのあるステッカー風
- 各お菓子は正方形マスの中央に、上下左右に少し余白を残して
- スプーンだけは縦長で“食べ物じゃない異物感”

## そのまま貼れるプロンプト（英語）
```
A 3x3 grid sprite sheet of 9 cute kawaii dessert game icons, evenly spaced, each item centered in its own cell, equal size, not overlapping, transparent background, soft pastel colors, thick clean outlines, glossy sticker style, mobile game assets.
Items, left-to-right, top-to-bottom:
1) round wrapped candy with swirl (pink)
2) round cookie with chocolate chips
3) cupcake with cream swirl and cherry
4) ring donut with pink icing and sprinkles
5) triangular strawberry shortcake slice with one strawberry on top
6) caramel pudding (creme caramel)
7) soft-serve ice cream on a cone
8) whole round cake with strawberries and candles
9) a tall rounded rectangular block with a silver spoon on it (looks like a non-food obstacle)
Consistent art style across all 9. High resolution.
```

## 完成後
このシートを `candy_0`〜`candy_7`（順番通り）＋ `spoon` に切り出します。送ってくれれば僕が分割・配置します。
