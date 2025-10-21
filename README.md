# 概要
マークダウンファイルでスライドを作成することができる Marp (Markdown Presentation Ecosystem) の自作テンプレートです．

html/cssを用いて，画像，数式，表などを柔軟にカスタマイズができます．

## 使い方 🚀

### 1. 準備

まず、このテンプレートをローカル環境にクローンまたはダウンロードします。
次に、VSCodeの拡張機能マーケットプレイスから **"Marp for VS Code"** をインストールしてください。

![Marp拡張機能](./img/marp_for_vscode.png)

### 2. VSCodeの設定

1. `Ctrl + ,` でコマンドパレットを開き、右上のファイルアイコンをクリックして **`settings.json`** を開きます。

   ![settings.json](./img/settings_json.png)

2. `settings.json` に以下の設定を追記します。これにより、カスタムテーマの適用やPowerPointへのエクスポート設定が有効になります。

   ```json
   {
       // ... 他の設定 ...
   
       // --- 以下を追記 ---
   
       // デフォルトのエクスポート形式をPowerPointに設定
       "markdown.marp.exportType": "pptx",
   
       // エクスポートしたPowerPointファイルを編集可能にする
       "markdown.marp.pptx.editable": "on",
   
       // 使用するカスタムテーマのCSSファイルを指定
       "markdown.marp.themes": [
           "[https://raw.githubusercontent.com/kaisugi/marp-theme-academic/main/themes/academic.css](https://raw.githubusercontent.com/kaisugi/marp-theme-academic/main/themes/academic.css)",
           "./custom.css"
       ],
   
       // Markdown内でのHTMLタグの使用を許可
       "markdown.marp.html": "all",
   
       // エクスポート時にローカルファイルのパスを正しく解決する
       "markdown.marp.strictPathResolutionDuringExport": true
   }
    ```

### 3. スライドの作成とプレビュー
"main.md" ファイルを編集してスライドを作成します。 エディタ上で右クリックし、"Open Preview" を選択すると、スライドの見た目をリアルタイムで確認できます。

  ![プレビュー](./img/open_preview.png)

### 4. スライドのエクスポート
"main.md" を開いた状態で、エディタ右上のMarpアイコン（再生ボタンが2つ重なったようなアイコン）をクリックし、 "Export Slide Deck..." を選択します。 これにより、スライドを PowerPoint (.pptx) や PDF などの形式で出力できます。

  ![エクスポート](./img/export.png)
