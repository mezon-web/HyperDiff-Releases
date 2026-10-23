# HyperDiff リリース案内

PDF・Word・Excelの差分確認とDoclingMをまとめたWindows x64向けの配布版です。

## v0.18.1の変更点

PDFDiffでは、ページの上下を比較から除外する範囲を実際のページで確認しながら調整できます。3つのDiffの表示オプションは別ダイアログになり、変更は「OK」で確定します。ExcelDiffの比較後に検索できない場合を修正し、DoclingMの進捗表示には現在の処理内容を追加しました。

## ダウンロードと起動

[最新のリリース](https://github.com/mezon-web/HyperDiff-Releases/releases/latest)のAssetsからHyperDiffの7zファイルをダウンロードし、フォルダーごと展開して各アプリの `.exe` を起動してください。「Source code (zip / tar.gz)」にはアプリ本体は含まれません。

.NET 10 Windows Desktop Runtime x64が必要です。Wordの文書表示・画像付きレポートにはWebView2 Runtimeも必要です。DoclingMの依存ライブラリとモデルは初回に準備します。

## 同梱アプリ

- ExcelDiffViewer
- PdfDiffViewer
- WordDiffViewer
- DoclingM

操作説明とPDF比較ガイドは配布ファイル内にあります。各版の変更点と注意事項は[更新履歴](CHANGELOG.md)および[リリース一覧](https://github.com/mezon-web/HyperDiff-Releases/releases)を確認してください。
