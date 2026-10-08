# HyperDiff

PDF・Word・Excelの差分確認と文書変換を行う、Windows x64向けのアプリセットです。
このリポジトリでは、配布ファイルと利用案内を公開しています。

## ダウンロード

[最新の配布版をダウンロード](https://github.com/mezon-web/HyperDiff-Releases/releases/latest)

Releaseの **Assets** から `HyperDiff.vX.Y.Z.7z` をダウンロードし、フォルダーごと展開してください。
GitHubが自動生成する「Source code (zip / tar.gz)」にはアプリ本体は含まれません。

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

展開先の各アプリフォルダー内の `.exe` を起動してください。
通常版DoclingMはPython本体を同梱し、依存ライブラリとモデルはアプリ内で準備します。
実行に必要なPython workerも通常配布版に含まれます。

詳しい操作は各アプリのヘルプと同梱マニュアルを参照してください。
PDF比較は、同梱の「PDF比較ワークフロー.html」を参照してください。
比較とレポート生成にMicrosoft Excel本体は必要ありません。

## ダウンロードの整合性確認

Releaseに添付する `.sha256` と、以下のコマンドで得たハッシュ値を照合できます。

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\HyperDiff.v0.16.1.7z'
```

## 更新履歴

各Releaseの説明と [CHANGELOG.md](CHANGELOG.md) を参照してください。
