# おかしまーじ！ 効果音(SE)仕様書

`assets/` に下記ファイル名で置くと**自動で差し替わります**。無ければ今のシンセ生成音にフォールバック（1個ずつ差し替えOK）。

## 共通
- 形式：**MP3**（短いワンショット。ループ不要）
- できるだけ**短く・軽く**（合体/落下は連打されるので、長いと重なって濁ります）
- 世界観：パステルで可愛い・高め・柔らかい（電子音すぎ／怖い音はNG）
- 最初のタップ後から鳴り始めます（ブラウザの自動再生制限）
- 音量はゲーム側で調整済み（作り込みすぎなくてOK）

## SE一覧（全10種）
| ファイル名 | 鳴る場面 | 長さ目安 | イメージ |
|---|---|---|---|
| `se_drop.mp3` | お菓子を落とした瞬間 | 0.1〜0.2秒 | 軽い「ぷりゅ」っとした高めのポップ |
| `se_merge.mp3` | 同じお菓子が合体 | 0.15〜0.3秒 | ぷにっと弾む可愛い合体音。気持ちいい |
| `se_fulfill.mp3` | おねがい(BONUS)達成 | 0.4〜0.6秒 | キラキラ上昇の達成音。ご褒美感 |
| `se_fever.mp3` | フィーバー発動／SWEET BURST／ラストスパート | 0.6〜1.0秒 | 派手で盛り上がる。キラ＋ミニファンファーレ |
| `se_golden.mp3` | ゴールデン合体（得点×3） | 0.5〜0.8秒 | 特別感のあるキラキラ「チャリーン✨」 |
| `se_clear.mp3` | おじゃまスプーンを3つ一掃 | 0.3〜0.5秒 | スッキリ片付く爽快音「ぷるるん」 |
| `se_anticip.mp3` | 「あと1回でフィーバー」予告 | 0.25〜0.4秒 | 期待が高まる上昇「タタタ↑」 |
| `se_tick.mp3` | 残り5秒の秒読み | 0.08〜0.15秒 | 高めの「ピッ」。緊張感（うるさすぎない） |
| `se_win.mp3` | クリア（時間まで生き残り） | 1.0〜1.5秒 | 明るい勝利ジングル |
| `se_over.mp3` | ゲームオーバー（あふれ） | 0.8〜1.2秒 | しょんぼり下降。可愛く切ない（怖くない） |

## 生成AI向けプロンプト例（英語）
- drop: `cute soft bubble pop, short, high pitched, kawaii game UI blip`
- merge: `cute bouncy pop merge sound, springy, high pitched, satisfying, kawaii`
- fulfill: `sparkly success chime, rising arpeggio, cute reward, short`
- fever: `exciting kawaii fanfare burst with sparkles, upbeat, celebratory`
- golden: `magical sparkle coin chime, special reward, shiny`
- clear: `cute cleanup pop swoosh, refreshing, satisfying`
- anticip: `rising anticipation blip, tension building, cute, short`
- tick: `soft high clock tick, short, gentle tension`
- win: `cheerful victory jingle, kawaii, bright, short`
- over: `cute sad descending sound, gentle disappointment, not scary`

## 任意（今は未対応・希望あれば実装）
- `se_count.mp3`（3・2・1のカウント音）／`se_start.mp3`（スタート音）

## 補足
- SEはコードでも生成しているので「ファイル無し」でも鳴ります。**気になる音だけ差し替える**運用が手軽です。
- フィーバー中のBGMループは別途 `bgm_fever.mp3`（→ SPEC_MUSIC.md）。
