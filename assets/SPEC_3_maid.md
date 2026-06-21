# 発注シート ③ メイドさん キャラクターシート（1枚にまとめて生成）

このシートは **同じメイドのキャラを1枚に複数レイアウト**して一気に生成する指示です。
（あとで僕が表情・ポーズごとに切り出して使います）

## 最重要ルール
- **全部 同一人物・同じ衣装・同じ画風**。表情とポーズだけが違う
- 顔の位置・大きさ・向き（正面）を揃えると差し替えがきれいに揃います

## 出力
- 1枚の画像
- 背景：**透過PNG**（不可なら真っ白 #FFFFFF。各カットをはっきり離して配置）
- 推奨キャンバス：2048 × 2048 px
- レイアウト：
  - **上2段＝表情差分7個**（バストアップの顔。4列×2行のうち7マスを使用）
  - **下1段＝カットイン2個**（半身のダイナミックなポーズ。横長で大きめ）

## キャラ設定
- 可愛いメイドの女の子（カフェ風）。パステル＆元気。丸ゴシックの世界観に合うフラット可愛い絵
- メイド服＋ホワイトのフリル・カチューシャ

## 表情差分 7個（上段）
| # | 表情 | 使う場面 |
|---|---|---|
| 1 | ふつう（にこやか待機） | 通常 |
| 2 | にこっ（うれしい） | ナイス・スッキリ |
| 3 | 大興奮（目キラキラ・口あけて） | コンボ・フィーバー・クリア |
| 4 | きらきら／ときめき（♡目） | 注文だいせいこう |
| 5 | どきどき／焦り（汗・期待） | あと1回でフィーバー |
| 6 | しょんぼり（涙目） | ゲームオーバー |
| 7 | やる気／気合い（むんっ） | ラストスパート |

## カットイン 2個（下段・半身ダイナミック）
| # | 内容 | 使う場面 |
|---|---|---|
| A | 大はしゃぎで応援する迫力ポーズ | フィーバー突入 |
| B | やりきった！の達成ガッツポーズ | タイムアップ（クリア） |

## そのまま貼れるプロンプト（英語）
```
A character expression sheet of ONE cute kawaii maid girl (cafe maid outfit, white frilly headband), consistent same character, same outfit, same flat kawaii pastel art style, thick clean outlines, transparent background.
Top area: 7 bust-up face variations in a grid, same framing and front view, only the expression changes:
1) normal gentle smile, 2) happy smile, 3) super excited with sparkling eyes and open mouth, 4) in-love with heart eyes, 5) nervous/anticipating with a sweat drop, 6) sad teary, 7) determined/fired-up.
Bottom area: 2 larger dynamic half-body action poses of the same maid:
A) cheering excitedly (for a "fever" moment), B) a triumphant victory pose (game clear).
Each cut clearly separated, evenly spaced, high resolution.
```

## 完成後
表情7個を `maid_normal / happy / excited / love / nervous / sad / determined`、
カットイン2個を `cutin_fever / cutin_clear` に切り出します。送ってくれれば僕が分割・配置します。
