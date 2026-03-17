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

## 使い方

プロフィール画像が必要な箇所で、以下の URL をそのまま使用する：
- **実写画像**：Unsplash（商用利用OK・高品質・帰属表示不要）を使用
  - サイズ変更は `w=` と `h=` の数値を変える（例: `w=300&h=300` で 300×300px）
  - `fit=crop&crop=face` で顔を中心にクロップされる
- **VTuber画像**：高品質なアニメ風イラストを使用
  - 星月ルナ：thiswaifudoesnotexist.net（AI生成・高品質アニメ顔）
  - 闇夜カゲロウ：要差替（適切な男性VTuber用イラスト検討中）

---

## Lumière メンバー

> 画像タイプ：実写ポートレート（5人組男性アイドルグループ）

| キャラクター | プレビュー | 画像URL |
|---|---|---|
| ハルト | ![](https://images.unsplash.com/photo-1698250542924-1f5ca454bb5b?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1698250542924-1f5ca454bb5b?w=150&h=150&fit=crop&crop=face` |
| レン | ![](https://images.unsplash.com/photo-1679377451157-5b212bd9d6a0?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1679377451157-5b212bd9d6a0?w=150&h=150&fit=crop&crop=face` |
| ソラ | ![](https://images.unsplash.com/photo-1654917249474-e508a8f64600?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1654917249474-e508a8f64600?w=150&h=150&fit=crop&crop=face` |
| ユウキ | ![](https://images.unsplash.com/photo-1722110719850-f41e0e8bcd5c?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1722110719850-f41e0e8bcd5c?w=150&h=150&fit=crop&crop=face` |
| カイト | ![](https://images.unsplash.com/photo-1619253692124-56dd8f736ca3?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1619253692124-56dd8f736ca3?w=150&h=150&fit=crop&crop=face` |

## ファンペルソナ

> 画像タイプ：実写カジュアル写真（一般ユーザーらしさ）

| キャラクター | プレビュー | 画像URL |
|---|---|---|
| 夏希（23歳女性） | ![](https://images.unsplash.com/photo-1759853899768-1413926111cb?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1759853899768-1413926111cb?w=150&h=150&fit=crop&crop=face` |
| りな（19歳女性） | ![](https://images.unsplash.com/photo-1730387432242-c707a42503f5?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1730387432242-c707a42503f5?w=150&h=150&fit=crop&crop=face` |
| ケンタ（27歳男性） | ![](https://images.unsplash.com/photo-1620295694696-f57fc3ae9182?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1620295694696-f57fc3ae9182?w=150&h=150&fit=crop&crop=face` |

## サブアーティスト

> 画像タイプ：実写ポートレート

| キャラクター | プレビュー | 画像URL |
|---|---|---|
| 月島 遥（女性SSW） | ![](https://images.unsplash.com/photo-1623227146854-51b32ca7b84d?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1623227146854-51b32ca7b84d?w=150&h=150&fit=crop&crop=face` |
| 藤宮 朱音（女性声優） | ![](https://images.unsplash.com/photo-1759725415895-775562df4088?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1759725415895-775562df4088?w=150&h=150&fit=crop&crop=face` |
| THE ORBIT タクヤ（バンド） | ![](https://images.unsplash.com/photo-1665118439071-8bc2c89f73af?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1665118439071-8bc2c89f73af?w=150&h=150&fit=crop&crop=face` |

## 追加アーティスト（artists-list.md）

> 各キャラクターの画像タイプは属性に基づく（上記「画像タイプ検証ルール」参照）

| キャラクター | 画像タイプ | プレビュー | 画像URL |
|---|---|---|---|
| PRISM（女性アイドル） | 実写 | ![](https://images.unsplash.com/photo-1667498234868-dfb09fdd5c3b?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1667498234868-dfb09fdd5c3b?w=150&h=150&fit=crop&crop=face` |
| 蒼天（男性ダンスボーカル） | 実写 | ![](https://images.unsplash.com/photo-1641615873382-ab1541a039fa?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1641615873382-ab1541a039fa?w=150&h=150&fit=crop&crop=face` |
| 柊 咲良（女性SSW） | 実写 | ![](https://images.unsplash.com/photo-1642435395055-5dc8b870f00c?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1642435395055-5dc8b870f00c?w=150&h=150&fit=crop&crop=face` |
| 霧島 カナタ（男性SSW） | 実写 | ![](https://images.unsplash.com/photo-1596387167508-f2464e15f098?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1596387167508-f2464e15f098?w=150&h=150&fit=crop&crop=face` |
| Midnight Circus（バンド） | 実写 | ![](https://images.unsplash.com/photo-1617814053951-e3bd095192be?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1617814053951-e3bd095192be?w=150&h=150&fit=crop&crop=face` |
| 落陽（バンド） | 実写 | ![](https://images.unsplash.com/photo-1591128429893-ac9952c1c892?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1591128429893-ac9952c1c892?w=150&h=150&fit=crop&crop=face` |
| 天音 まひろ（女性声優） | 実写 | ![](https://images.unsplash.com/photo-1654907300621-78c0edc0570a?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1654907300621-78c0edc0570a?w=150&h=150&fit=crop&crop=face` |
| 御影 陸（男性声優） | 実写 | ![](https://images.unsplash.com/photo-1669626068866-22b1620be2e3?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1669626068866-22b1620be2e3?w=150&h=150&fit=crop&crop=face` |
| 星月ルナ（女性VTuber） | **イラスト** | ![](https://wsrv.nl/?url=https://www.thiswaifudoesnotexist.net/example-5555.jpg&w=150&h=150&fit=cover) | `https://www.thiswaifudoesnotexist.net/example-5555.jpg` |
| 闇夜カゲロウ（男性VTuber） | **イラスト** | ![](https://wsrv.nl/?url=https://nekos.best/api/v2/husbando/950eae96-5689-48f4-adb1-23555f3a2358.png&w=150&h=150&fit=cover) | `https://nekos.best/api/v2/husbando/950eae96-5689-48f4-adb1-23555f3a2358.png` |

## モブファン（コメント欄等で使う匿名アバター）

> 画像タイプ：実写カジュアル写真

| 用途 | プレビュー | 画像URL |
|---|---|---|
| モブファン1（女性） | ![](https://images.unsplash.com/photo-1752312640883-e8953a068d83?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1752312640883-e8953a068d83?w=150&h=150&fit=crop&crop=face` |
| モブファン2（男性） | ![](https://images.unsplash.com/photo-1678531730619-5c0cbb7735be?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1678531730619-5c0cbb7735be?w=150&h=150&fit=crop&crop=face` |
| モブファン3（女性） | ![](https://images.unsplash.com/photo-1647719518553-2a8091862f3f?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1647719518553-2a8091862f3f?w=150&h=150&fit=crop&crop=face` |
| モブファン4（男性） | ![](https://images.unsplash.com/photo-1742151103301-d16bc800c0d9?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1742151103301-d16bc800c0d9?w=150&h=150&fit=crop&crop=face` |
| モブファン5（女性） | ![](https://images.unsplash.com/photo-1677597889434-4f4cffec5220?w=150&h=150&fit=crop&crop=face) | `https://images.unsplash.com/photo-1677597889434-4f4cffec5220?w=150&h=150&fit=crop&crop=face` |
