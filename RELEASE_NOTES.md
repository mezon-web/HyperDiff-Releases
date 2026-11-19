# HyperDiff v0.20.0

PDF・Word・Excelの差分確認と文書変換を行うWindows x64向けアプリセットです。

## 主な変更

- PDFDiffで、改訂により見出しの所属が変わった段落も、本文の類似性と前後の対応から確認できる場合は対応付けます。繰り返される行や図の表セルも、対応済みの見出しや図題で範囲を確認して比較します。数値・文言の変更は差分として保持します。
- PDFDiffとWordDiffで、結果画面の表示オプションから比較条件を変更できます。
- PDFDiffで、各ファイルのJSON情報ボタンから原本情報・変換設定・変換環境を確認してコピーできます。
- PDFDiffとExcelDiffで、情報を取得できなかった箇所も通常の差分一覧に理由付きで表示します。
- DoclingMのDoclingを2.150.1に更新しました。Docling Core、Docling Parse、PDF処理に使う関連ライブラリも更新しました。

## ダウンロードと起動

Assetsの `HyperDiff.v0.20.0.7z` を取得し、フォルダーごと展開して各アプリの `.exe` を起動してください。ExcelDiffViewer・PdfDiffViewer・WordDiffViewer・DoclingMを同梱しています。

Windows x64と.NET 10 Windows Desktop Runtime x64が必要です。Wordの文書表示・画像付きレポートにはWebView2 Runtimeも必要です。DoclingMの初回セットアップ・モデル取得にはインターネット接続が必要です。比較とレポート生成にMicrosoft Officeのインストールは必要ありません。

操作説明とPDF比較ワークフローは配布ファイルに同梱しています。アーカイブの整合性は添付の `.sha256` で確認できます。
