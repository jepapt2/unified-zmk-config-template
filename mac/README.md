# 双掌 TH-601：Mac用Karabiner設定

Bluetooth接続の双掌（vendor_id: 7504 / product_id: 24926）用です。

- 数字レイヤー＋左上キー（ZMKのGRAVE）：日本語／英字を切り替え
- 左Control：Command
- Alt：Mac標準のOptionとして動作
- マウス機能を持つ双掌もKarabinerの処理対象になるよう `ignore: false` を設定
- キーの変更は双掌だけに適用

## 別のMacへの導入

1. Karabiner-Elementsをインストールし、案内に従って必要な権限とドライバを有効にします。
2. macOSの入力ソースに日本語（ローマ字入力）とABCを追加します。
3. 同じフォルダの `karabiner.json` をダウンロードします（GitHubのRawまたはDownload raw file）。
4. Finderで「移動」→「フォルダへ移動」を選び、 `~/.config/karabiner/` を開きます。
5. 既存の `karabiner.json` があれば別名でバックアップしてから、ダウンロードしたファイルを `karabiner.json` として置きます。
6. 双掌をBluetooth接続し、数字レイヤー＋左上キーで日本語／英字を往復できることと、Control＋C／Vでコピー・貼り付けできることを確認します。

**これは設定全体を置き換えるファイルです。既存のKarabiner設定を残したい場合は上書きせず、選択中プロファイルの `complex_modifications.rules` と双掌の `devices` 設定を統合してください。**

仕事用Macでは所属先のソフトウェア利用ルールに従ってください。
