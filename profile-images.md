# プロフィール画像 URL マッピング

> AI がサンプルテキスト生成時に画像も指定できるよう、各キャラクターに固定のプロフィール画像 URL を割り当てる。

---

## 画像タイプ検証ルール（必読）

キャラクターの属性と画像タイプの整合性を必ず守ること。**このルールに違反する画像は使用禁止。**

| アーティストタイプ | 必須画像タイプ | NG画像タイプ | 理由 |
|---|---|---|---|
| アイドル / ダンスボーカル | 実写ポートレート | イラスト | 実在アーティストとしての存在感が必要 |
| シンガーソングライター | 実写ポートレート | イラスト | 同上 |
| 声優アーティスト | 実写ポートレート | イラスト | 同上 |
| バンド | 実写ポートレート | イラスト | 同上 |
| **VTuber** | **イラスト / アニメ風アバター** | **実写** | VTuberは中の人を出さない。実写はキャラ設定と矛盾する |
| ファン（ペルソナ） | 実写カジュアル写真 | アーティスト風の写真 | 一般ユーザーらしさが必要 |
| モブファン | 実写カジュアル写真 | アーティスト風の写真 | 同上 |

### 画像選定時のチェックリスト
- [ ] キャラクターの属性と画像タイプが一致しているか？（上表参照）
- [ ] 日本人向けサービスとして、日本人らしい見た目か？
- [ ] 商用利用可能なライセンスか？
- [ ] 画像の品質は十分か？（低解像度・圧縮ノイズがないか）

---

## 根本原因分析：VTuber画像に実写を割り当てた問題

### 何が起きたか
VTuberキャラクター（星月ルナ、闇夜カゲロウ）に実写の人物写真を割り当てた。VTuberは「中の人を出さない」キャラクターであり、実写はキャラクター設定と根本的に矛盾する。

### なぜ起きたか
1. **画像タイプの検証ルールが存在しなかった** — 「全キャラクターに Unsplash の写真を割り当てる」という一律のアプローチで進め、キャラクター属性ごとに必要な画像タイプが異なることを考慮しなかった
2. **属性→画像タイプのマッピング思考が抜けていた** — アーティスト名と画像URLの1対1対応だけを考え、アーティストタイプ→画像タイプという中間ステップを踏まなかった

### 再発防止策
1. **上記「画像タイプ検証ルール」を本ドキュメントに常設** — 画像追加・変更時に必ず参照する
2. **チェックリストによるセルフレビュー** — 画像選定後、属性との整合性を1件ずつ確認する
3. **AI にサンプルテキスト生成を依頼する際も、このルールを読み込ませる** — AI が画像を選ぶ場合も同じ検証が走る

---

## 使い方

プロフィール画像が必要な箇所で、以下の URL をそのまま使用する：
- **実写画像**：Unsplash（商用利用OK・高品質・帰属表示不要）を使用
  - サイズ変更は `w=` と `h=` の数値を変える（例: `w=300&h=300` で 300×300px）
  - `fit=crop&crop=face` で顔を中心にクロップされる
- **VTuber画像**：DiceBear API（CC0 / パブリックドメイン）のイラストアバターを使用
  - サイズ変更は `size=` の数値を変える（例: `size=300` で 300×300px）

---

## Lumière メンバー

> 画像タイプ：実写ポートレート（5人組男性アイドルグループ）

| キャラクター | プレビュー | 画像URL |
|---|---|---|
| ハルト | ![](https://images.unsplash.com/photo-1695800998493-ccff5ea292ea?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1695800998493-ccff5ea292ea?w=150&h=150&fit=crop&crop=face` |
| レン | ![](https://images.unsplash.com/photo-1643816831265-0a50e67e33cf?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1643816831265-0a50e67e33cf?w=150&h=150&fit=crop&crop=face` |
| ソラ | ![](https://images.unsplash.com/photo-1623948136036-0e3cec067ef1?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1623948136036-0e3cec067ef1?w=150&h=150&fit=crop&crop=face` |
| ユウキ | ![](https://images.unsplash.com/photo-1669626068866-22b1620be2e3?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1669626068866-22b1620be2e3?w=150&h=150&fit=crop&crop=face` |
| カイト | ![](https://images.unsplash.com/photo-1680058269094-20a5137ca4e5?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1680058269094-20a5137ca4e5?w=150&h=150&fit=crop&crop=face` |

## ファンペルソナ

> 画像タイプ：実写カジュアル写真（一般ユーザーらしさ）

| キャラクター | プレビュー | 画像URL |
|---|---|---|
| 夏希（23歳女性） | ![](https://images.unsplash.com/photo-1611403119860-57c4937ef987?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1611403119860-57c4937ef987?w=150&h=150&fit=crop&crop=face` |
| りな（19歳女性） | ![](https://images.unsplash.com/photo-1614252234498-1ab6d3926b57?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1614252234498-1ab6d3926b57?w=150&h=150&fit=crop&crop=face` |
| ケンタ（27歳男性） | ![](https://images.unsplash.com/photo-1582828102977-7210c1096e9e?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1582828102977-7210c1096e9e?w=150&h=150&fit=crop&crop=face` |

## サブアーティスト

> 画像タイプ：実写ポートレート

| キャラクター | プレビュー | 画像URL |
|---|---|---|
| 月島 遥（女性SSW） | ![](https://images.unsplash.com/photo-1545947288-c22ade2af79d?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1545947288-c22ade2af79d?w=150&h=150&fit=crop&crop=face` |
| 藤宮 朱音（女性声優） | ![](https://images.unsplash.com/photo-1676777493576-1432f14373bb?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1676777493576-1432f14373bb?w=150&h=150&fit=crop&crop=face` |
| THE ORBIT タクヤ（バンド） | ![](https://images.unsplash.com/photo-1665118439071-8bc2c89f73af?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1665118439071-8bc2c89f73af?w=150&h=150&fit=crop&crop=face` |

## 追加アーティスト（artists-list.md）

> 各キャラクターの画像タイプは属性に基づく（上記「画像タイプ検証ルール」参照）

| キャラクター | 画像タイプ | プレビュー | 画像URL |
|---|---|---|---|
| PRISM（女性アイドル） | 実写 | ![](https://images.unsplash.com/photo-1667498234868-dfb09fdd5c3b?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1667498234868-dfb09fdd5c3b?w=150&h=150&fit=crop&crop=face` |
| 蒼天（男性ダンスボーカル） | 実写 | ![](https://images.unsplash.com/photo-1701463387028-3947648f1337?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1701463387028-3947648f1337?w=150&h=150&fit=crop&crop=face` |
| 柊 咲良（女性SSW） | 実写 | ![](https://images.unsplash.com/photo-1642435395055-5dc8b870f00c?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1642435395055-5dc8b870f00c?w=150&h=150&fit=crop&crop=face` |
| 霧島 カナタ（男性SSW） | 実写 | ![](https://images.unsplash.com/photo-1701463205870-6b6ec3dbed2b?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1701463205870-6b6ec3dbed2b?w=150&h=150&fit=crop&crop=face` |
| Midnight Circus（バンド） | 実写 | ![](https://images.unsplash.com/photo-1695927521717-a0ad39d93505?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1695927521717-a0ad39d93505?w=150&h=150&fit=crop&crop=face` |
| 落陽（バンド） | 実写 | ![](https://images.unsplash.com/photo-1540541382853-9d06e3479235?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1540541382853-9d06e3479235?w=150&h=150&fit=crop&crop=face` |
| 天音 まひろ（女性声優） | 実写 | ![](https://images.unsplash.com/photo-1673802851107-a01850d12ce6?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1673802851107-a01850d12ce6?w=150&h=150&fit=crop&crop=face` |
| 御影 陸（男性声優） | 実写 | ![](https://images.unsplash.com/photo-1661854236305-b02cef4aa0af?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1661854236305-b02cef4aa0af?w=150&h=150&fit=crop&crop=face` |
| 星月ルナ（女性VTuber） | **イラスト** | ![](https://api.dicebear.com/9.x/lorelei/png?seed=HoshizukiLuna&size=150&backgroundColor=e0e7ff) | `https://api.dicebear.com/9.x/lorelei/png?seed=HoshizukiLuna&size=150&backgroundColor=e0e7ff` |
| 闇夜カゲロウ（男性VTuber） | **イラスト** | ![](https://api.dicebear.com/9.x/lorelei/png?seed=YamiyoKagerou&size=150&backgroundColor=1e1b4b) | `https://api.dicebear.com/9.x/lorelei/png?seed=YamiyoKagerou&size=150&backgroundColor=1e1b4b` |

## モブファン（コメント欄等で使う匿名アバター）

> 画像タイプ：実写カジュアル写真

| 用途 | プレビュー | 画像URL |
|---|---|---|
| モブファン1（女性） | ![](https://images.unsplash.com/photo-1590317198525-243e5aa18d5b?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1590317198525-243e5aa18d5b?w=150&h=150&fit=crop&crop=face` |
| モブファン2（男性） | ![](https://images.unsplash.com/photo-1609558930883-3f31fad3d4e6?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1609558930883-3f31fad3d4e6?w=150&h=150&fit=crop&crop=face` |
| モブファン3（女性） | ![](https://images.unsplash.com/photo-1647719518553-2a8091862f3f?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1647719518553-2a8091862f3f?w=150&h=150&fit=crop&crop=face` |
| モブファン4（男性） | ![](https://images.unsplash.com/photo-1605504836193-e77d3d9ede8a?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1605504836193-e77d3d9ede8a?w=150&h=150&fit=crop&crop=face` |
| モブファン5（女性） | ![](https://images.unsplash.com/photo-1677597889434-4f4cffec5220?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1677597889434-4f4cffec5220?w=150&h=150&fit=crop&crop=face` |
