# LATIA テスト用の架空抽選ページ

LATIA（抽選応募補助アプリ）の開発・動作確認専用の、架空の抽選サイトです。実在の店舗・商品・抽選ではありません。

- 告知 → 応募フォーム → 確認 → 完了（抽選番号・QRコード・店舗名）の流れを再現します。
- 入力内容はどこにも送信・保存されません（送信前に項目名を外し、次の画面のURLに値が載らないようにしています）。
- 検索エンジンに載らないよう noindex と robots.txt を設定しています。

## 構造を再現した3種（LATIA 動作確認用）

- `livepocket-type/` 架空チケット抽選（LivePocket型）
- `google-form-type/` 架空フォーム抽選（Googleフォーム型。`native=1` は汎用ロジック確認用で実サイトの再現ではない）
- `cardbox-type/` 架空カードショップ抽選（カードボックス型。`ad=dom|style|afterinput|storm|off`、`aframe=0|visible`、`item=2`、`entry_complete` の別シナリオ）

ルートの `index.html`〜`complete.html` はシンプル版として残しています。
