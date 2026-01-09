# Marpスライド置き場(Private)

- 青スタ・Scratch講義の模擬授業用スライド
- 42Tokyo CTF

## Marp CLIの使い方

Marp CLIを使用すると、Markdownファイルをコマンドラインからスライド(HTML, PDF, PPTX)に変換できる。

### インストール方法

Node.jsがインストールされている必要がある。

**1. グローバルインストール (推奨)**
```bash
npm install -g @marp-team/marp-cli
```

**2. プロジェクトごとのインストール**
```bash
npm install --save-dev @marp-team/marp-cli
```

### 基本的な使い方

**HTMLへの変換 (デフォルト)**
```bash
marp slide.md
```
`slide.html`が生成される。

**PDFへの変換**
```bash
marp slide.md --pdf
```

**PowerPoint (PPTX) への変換**
```bash
marp slide.md --pptx
```

**画像への変換**
```bash
marp slide.md --image png
```

### 便利なオプション

**プレビューモード (Watch mode)**
ファイルを監視し、変更があるたびに自動的に再生成してプレビューする。
```bash
marp slide.md --preview
# または
marp -p slide.md
```

**テーマの指定**
```bash
marp slide.md --theme gaia
```

**npxを使用する場合 (インストールなしで実行)**
```bash
npx @marp-team/marp-cli slide.md
```

詳細なドキュメントは[公式リポジトリ](https://github.com/marp-team/marp-cli)を参照。

