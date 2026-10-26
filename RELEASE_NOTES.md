# HyperDiff v0.18.6

- DoclingMの仮想環境の作成・更新で、必要なライブラリを取得できず停止する問題を修正しました。v0.18.5で停止した場合も、v0.18.6で「仮想環境を作成/更新」を再実行すると、取得済みの資材を利用できます。
- DoclingMの出力先で、処理後に `.doclingm-output.lock` が残らないようにしました。旧版が残した同名ファイルは自動削除しないため、旧版を終了してから手動で削除してください。

## ダウンロードと起動

Assetsの `HyperDiff.v0.18.6.7z` をダウンロードし、フォルダーごと展開して各アプリの `.exe` を起動してください。ExcelDiffViewer・PdfDiffViewer・WordDiffViewer・DoclingMを同梱しています。

Windows x64、.NET 10 Windows Desktop Runtime x64が必要です。Wordの文書表示・画像付きレポートにはWebView2 Runtimeも必要です。DoclingMの初回セットアップ・モデル取得にはインターネット接続が必要です。

操作説明とPDF比較ワークフローは配布ファイルに同梱しています。アーカイブの整合性は添付の `.sha256` で確認できます。
