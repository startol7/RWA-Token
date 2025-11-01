# RWA Token - 実世界資産トークン化プラットフォーム

![RWA Token](https://img.shields.io/badge/RWA-Token-blue)
![React](https://img.shields.io/badge/React-18-61dafb)
![License](https://img.shields.io/badge/license-MIT-green)

## 🚀 概要

RWA (Real World Asset) Tokenは、不動産、債券、コモディティなどの実世界の資産をブロックチェーン上でトークン化し、誰でも小口から投資できるプラットフォームのランディングページです。

## ✨ 特徴

- 💎 **モダンなUI/UX** - グラデーション、アニメーション、グラスモーフィズムを使用した洗練されたデザイン
- 📱 **レスポンシブデザイン** - モバイル、タブレット、デスクトップに完全対応
- ⚡ **高速表示** - CDN経由でライブラリを読み込み、最適化されたパフォーマンス
- 🎨 **アニメーション効果** - スムーズなホバーエフェクトとトランジション
- 🌐 **スタンドアロン** - 単一のHTMLファイルで完結

## 📦 技術スタック

- **React 18** - UIライブラリ
- **Tailwind CSS** - スタイリング
- **Lucide Icons** - カスタムSVGアイコン
- **Google Fonts (Inter)** - タイポグラフィ

## 🌐 GitHub Pagesへのデプロイ方法

### 方法1: GitHub Desktopを使用（初心者向け）

1. **GitHubアカウントを作成**
   - https://github.com にアクセスして無料アカウントを作成

2. **新しいリポジトリを作成**
   - GitHubにログイン後、右上の「+」→「New repository」をクリック
   - Repository名を入力（例: `rwa-token-site`）
   - 「Public」を選択
   - 「Create repository」をクリック

3. **ファイルをアップロード**
   - 「uploading an existing file」をクリック
   - `index.html`ファイルをドラッグ&ドロップ
   - 「Commit changes」をクリック

4. **GitHub Pagesを有効化**
   - リポジトリの「Settings」タブをクリック
   - 左サイドバーの「Pages」をクリック
   - 「Source」で「Deploy from a branch」を選択
   - 「Branch」で「main」と「/ (root)」を選択
   - 「Save」をクリック

5. **デプロイ完了！**
   - 数分待つと、`https://[あなたのユーザー名].github.io/[リポジトリ名]/` でサイトが公開されます

### 方法2: Git CLIを使用（上級者向け）

```bash
# リポジトリをクローン
git clone https://github.com/[あなたのユーザー名]/[リポジトリ名].git
cd [リポジトリ名]

# index.htmlファイルをコピー
cp /path/to/index.html .

# コミットしてプッシュ
git add index.html
git commit -m "Add RWA Token landing page"
git push origin main

# GitHub Pagesの設定
# GitHubのリポジトリページで Settings > Pages から設定
```

## 🎨 カスタマイズ方法

### 色の変更

`index.html`内のTailwind CSSクラスを編集します：

```html
<!-- 例: プライマリカラーを青から緑に変更 -->
<!-- 変更前 -->
<div class="bg-gradient-to-r from-blue-500 to-purple-600">

<!-- 変更後 -->
<div class="bg-gradient-to-r from-green-500 to-emerald-600">
```

### コンテンツの変更

以下の部分を編集してテキストを変更できます：

- **タイトル**: `<h1>`タグ内のテキスト
- **説明文**: `<p>`タグ内のテキスト
- **統計データ**: `stats`配列の値
- **資産情報**: `assets`配列のデータ
- **機能説明**: `features`配列のデータ

### アニメーションの調整

`<style>`タグ内のCSSアニメーションを編集：

```css
/* フロートアニメーションの速度を変更 */
@keyframes float {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-20px); }
}

/* 6秒を3秒に変更して速くする */
.animate-float {
    animation: float 3s ease-in-out infinite;
}
```

## 📱 ブラウザサポート

- ✅ Chrome (最新版)
- ✅ Firefox (最新版)
- ✅ Safari (最新版)
- ✅ Edge (最新版)
- ✅ モバイルブラウザ

## 🐛 トラブルシューティング

### サイトが表示されない場合

1. GitHub Pagesの設定を確認
2. index.htmlがリポジトリのルートディレクトリにあることを確認
3. ファイル名が正確に`index.html`（小文字）であることを確認
4. ブラウザのキャッシュをクリア

### スタイルが適用されない場合

1. インターネット接続を確認（CDNからCSSを読み込むため）
2. ブラウザのコンソールでエラーを確認

## 📄 ライセンス

MIT License - 自由に使用、修正、配布できます

## 🤝 貢献

プルリクエストを歓迎します！大きな変更の場合は、まずissueを開いて変更内容を議論してください。

## 📞 サポート

問題が発生した場合は、GitHubのIssuesセクションで報告してください。

---

Made with ❤️ by RWA Token Team
