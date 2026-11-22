# HyperDiff v0.20.2

PDF・Word・Excelの差分確認と文書変換を行うWindows x64向けアプリセットです。

## 主な変更

- ExcelDiffで、別のパス表記で指定しても比較元・比較先のブックをExcelレポートで上書きできないようにしました。
- DoclingMで、PDFの一部が変換できなかった場合やページ番号が一致しない場合は、出力を中止して既存のファイルを保護します。
- WordDiffで、「表示文字だけ比較」をOFFにすると、段落をまたぐフィールドの参照先変更も検出します。「書式も比較」がONの場合は、手動改行・改ページ・段区切りの違いも検出します。
- WordDiffで、Strict Open XML形式の文書を開いたときに、通常のWord文書（.docx）として保存し直す方法を案内します。
- PDFDiffで、解析JSONに読み込み順が指定されていないブロックが多い場合の読み込みを軽くしました。
- PDFDiff・ExcelDiffのヘルプを、取得できなかった項目も通常の差分一覧に表示する現在の動作に合わせました。

## ダウンロードと起動

Assetsの `HyperDiff.v0.20.2.7z` を取得し、フォルダーごと展開して各アプリの `.exe` を起動してください。ExcelDiffViewer・PdfDiffViewer・WordDiffViewer・DoclingMを同梱しています。

Windows x64と.NET 10 Windows Desktop Runtime x64が必要です。Wordの文書表示・画像付きレポートにはWebView2 Runtimeも必要です。DoclingMの初回セットアップ・モデル取得にはインターネット接続が必要です。比較とレポート生成にMicrosoft Officeのインストールは必要ありません。

操作説明とPDF比較ワークフローは配布ファイルに同梱しています。アーカイブの整合性は添付の `.sha256` で確認できます。
