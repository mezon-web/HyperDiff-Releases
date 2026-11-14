# HyperDiff

PDF・Word・Excelの差分確認と文書変換を行う、Windows x64向けのアプリセットです。
このリポジトリでは、配布ファイルと利用案内を公開しています。

## ダウンロード

**[最新版をダウンロード（v0.19.8・Windows x64・7z）](https://github.com/mezon-web/HyperDiff-Releases/releases/download/v0.19.8/HyperDiff.v0.19.8.7z)**

2026-11-14更新。PDFDiffで、複数ページの要件に続く本文や、句読点・数字の字間が異なる表題の対応付けを改善したv0.19.8を配布しています。

[更新内容](https://github.com/mezon-web/HyperDiff-Releases/releases/tag/v0.19.8) · [過去バージョン](https://github.com/mezon-web/HyperDiff-Releases/releases)

上の「最新版をダウンロード」から `HyperDiff.v0.19.8.7z` を取得し、フォルダーごと展開してください。
GitHubが自動生成する「Source code (zip / tar.gz)」にはアプリ本体は含まれません。

## Pdf2Excel（単独配布）

DoclingMで作成した画像付きJSONを、段落や図表ごとのExcelに変換する独立ツールです。

- **[Pdf2Excelの最新版をダウンロード（v0.1.0・プレビュー版・Windows x64・ZIP）](https://github.com/mezon-web/HyperDiff-Releases/releases/download/pdf2excel-v0.1.0/Pdf2Excel-v0.1.0.zip)**
- [Pdf2Excelの更新内容](https://github.com/mezon-web/HyperDiff-Releases/releases/tag/pdf2excel-v0.1.0) · [過去バージョン](https://github.com/mezon-web/HyperDiff-Releases/releases)
- [使い方・必要環境](PDF2EXCEL.md) / [更新履歴](PDF2EXCEL_CHANGELOG.md)
- Windows x64、.NET 10 Desktop Runtime（x64）が必要です。.NETは同梱していません。

## 同梱アプリ

| アプリ | 用途 |
| --- | --- |
| ExcelDiffViewer | Excelブックのセル・シート構造を比較 |
| WordDiffViewer | Word文書の段落・表・図形・注釈などを比較 |
| PdfDiffViewer | DoclingMで変換したJSONからPDFの本文・表・画像・配置差分を確認 |
| DoclingM | PDFやOffice文書を解析し、JSON・Markdown・HTML・Textへ変換 |

## 必要環境と起動

- Windows x64
- [.NET 10 Windows Desktop Runtime x64](https://dotnet.microsoft.com/ja-jp/download/dotnet/10.0)
- Wordの文書表示・画像付きレポートには[Microsoft Edge WebView2 Runtime](https://developer.microsoft.com/ja-jp/microsoft-edge/webview2/)
- DoclingMの初回セットアップ・モデル取得にはインターネット接続

最上位フォルダーは `HyperDiff v0.19.8`、その中のアプリフォルダーは `ExcelDiffViewer`、`PdfDiffViewer`、`WordDiffViewer`、`DoclingM` です。
各アプリフォルダー内の `.exe` を起動してください。
DoclingMは初回利用時に必要な依存ライブラリ・モデルを準備します。
v0.17.7以前から更新する場合は、初回に実行環境を再セットアップします。Windowsのパス長制限がある場合は、DoclingMの配置先の絶対パスを105文字以下にしてください。

詳しい操作は各アプリのヘルプと同梱マニュアルを参照してください。
PDF比較は、同梱の「PDF比較ワークフロー.html」を参照してください。
比較とレポート生成にMicrosoft Excel本体は必要ありません。

## ダウンロードの整合性確認

Releaseに添付する `.sha256` と、以下のコマンドで得たハッシュ値を照合できます。

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\HyperDiff.v0.19.7.7z'
```

## 更新履歴

各Releaseの説明と [CHANGELOG.md](CHANGELOG.md) を参照してください。

<!-- 配布案内の更新手順: 実行用Assetは版番号付きのため、次回リリース公開時にREADME内のHyperDiff・Pdf2Excelそれぞれの版番号・直リンク・展開先名を新しいAssetに合わせて更新する。更新内容・過去バージョンへのリンクを残し、匿名のHEADリクエスト等で直リンクの到達先を確認する。GitHub Actionsは使用しない。 -->
