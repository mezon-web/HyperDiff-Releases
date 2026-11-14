# HyperDiff v0.19.8

PDF・Word・Excelの差分確認と文書変換を行うWindows x64向けアプリセットです。

## 主な変更

- PDFDiffで、要件が複数ページにまたがる文書や句読点の改訂がある文書について、前後の本文から対応を確認できる範囲を広げました。
- PDFDiffで、元の表全体から対応を確認できる範囲で、表題の比較を改善しました。数値の区切り変更は差分として保持します。

解析結果で見出しや表の所属を十分に確認できない場合は、対応する内容でも削除・追加として表示されることがあります。

## ダウンロードと起動

Assetsの `HyperDiff.v0.19.8.7z` をダウンロードし、フォルダーごと展開して各アプリの `.exe` を起動してください。ExcelDiffViewer・PdfDiffViewer・WordDiffViewer・DoclingMを同梱しています。

Windows x64、.NET 10 Windows Desktop Runtime x64が必要です。Wordの文書表示・画像付きレポートにはWebView2 Runtimeも必要です。DoclingMの初回セットアップ・モデル取得にはインターネット接続が必要です。比較とレポート生成にMicrosoft Officeのインストールは必要ありません。

操作説明とPDF比較ワークフローは配布ファイルに同梱しています。アーカイブの整合性は添付の `.sha256` で確認できます。
