# AI Search & Quiz App 🔍🧠

Google AI Studio APIを活用した、検索・学習・クイズ機能を統合したWebアプリケーションです。

![App Screenshot](https://img.shields.io/badge/React-18.x-blue?style=for-the-badge&logo=react)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

## 📖 概要

このアプリは以下の3つの主要機能を提供します:

1. **AI検索エンジン**: Google Gemini APIによる高度な検索と要約
2. **検索履歴管理**: 過去の検索を保存・閲覧
3. **自動クイズ生成**: 検索内容から学習用の4択クイズを自動作成

## ✨ 主な機能

### 🔍 検索機能
- Google AI Studio APIを使用したインテリジェント検索
- **300文字以内の分かりやすい要約**を自動生成
- 検索結果の**全文表示**にも対応
- 展開/折りたたみで読みやすく管理

### 📚 検索履歴
- すべての検索を自動保存
- 日時付きで履歴を管理
- 過去の検索結果をいつでも閲覧可能
- 履歴の一括削除機能

### 🎯 クイズ機能
- 検索内容から自動で4択問題を生成
- **問題文は検索キーワードを約60文字で説明**(キーワード自体は含まない)
- 正解は検索キーワード、他3つはAIが生成したフェイク選択肢
- 解答後に詳しい解説を表示
- 教育的価値の高い学習体験

## 🚀 デモ

**ライブデモ**: [https://YOUR_USERNAME.github.io/app-of-Search-2/](https://YOUR_USERNAME.github.io/app-of-Search-2/)

## 🛠️ 技術スタック

- **フロントエンド**: React 18.x
- **スタイリング**: Tailwind CSS
- **アイコン**: Lucide React
- **AI API**: Google AI Studio (Gemini Pro)
- **ストレージ**: Browser localStorage

## 📦 インストール・セットアップ

### 前提条件

- Node.js (v16以上推奨)
- npm または yarn
- Google AI Studio APIキー

### Google AI Studio APIキーの取得

1. [Google AI Studio](https://makersuite.google.com/app/apikey)にアクセス
2. Googleアカウントでログイン
3. 「Create API Key」をクリック
4. APIキーをコピー(このキーは後で使用します)

### ローカル環境での実行

```bash
# リポジトリをクローン
git clone https://github.com/YOUR_USERNAME/app-of-Search-2.git

# ディレクトリに移動
cd app-of-Search-2

# 依存パッケージをインストール
npm install

# 開発サーバーを起動
npm start
```

ブラウザで `http://localhost:3000` を開き、APIキーを入力してアプリを使用できます。

## 🌐 GitHub Pagesへのデプロイ

### 方法1: 手動デプロイ

```bash
# ビルド
npm run build

# GitHub Pagesにデプロイ
npm run deploy
```

### 方法2: GitHubの設定から

1. GitHubリポジトリページを開く
2. **Settings** → **Pages** に移動
3. **Source**: "Deploy from a branch"を選択
4. **Branch**: `main`、フォルダ: `/ (root)`を選択
5. **Save**をクリック

数分後、`https://YOUR_USERNAME.github.io/app-of-Search-2/`でアクセス可能になります。

## 🔒 セキュリティとプライバシー

### APIキーの安全性

✅ **完全にクライアントサイドで動作**
- APIキーはユーザーのブラウザのlocalStorageにのみ保存
- GitHubリポジトリには一切含まれません
- サーバーを経由せず、直接Google APIと通信

✅ **ユーザーが自分のAPIキーを管理**
- 各ユーザーが自分のAPIキーを使用
- アプリ側でAPIキーを保存・管理しません

### データ保護

- すべてのデータはブラウザのlocalStorageに保存
- 外部サーバーにデータは送信されません
- プライバシーを完全に保護

## 📱 使い方

### 1. 初回起動

アプリを開くと、APIキー入力画面が表示されます。

1. Google AI StudioでAPIキーを取得
2. APIキーを入力
3. 「開始」ボタンをクリック

### 2. 検索する

1. 検索バーにクエリを入力
2. 「検索」ボタンをクリック
3. 要約と全文が表示されます
4. 自動でクイズも生成されます

### 3. クイズに挑戦

1. 「クイズ」タブに移動
2. 過去の検索から選択
3. 4択問題に解答
4. 解説を読んで理解を深める

### 4. 履歴を確認

1. 「履歴」タブに移動
2. 過去の検索をすべて閲覧可能
3. 全文表示で詳細を確認

## 🎨 画面構成

```
┌─────────────────────────────────────┐
│  AI Search & Quiz        [APIキー削除] │
│  [検索バー]               [検索]     │
└─────────────────────────────────────┘
┌──────┬──────┬──────┐
│ 検索 │ 履歴 │クイズ│
└──────┴──────┴──────┘

[メインコンテンツエリア]
- 検索結果表示
- 履歴一覧
- クイズ画面
```

## 🤝 コントリビューション

プルリクエストを歓迎します!

1. このリポジトリをフォーク
2. 機能ブランチを作成 (`git checkout -b feature/AmazingFeature`)
3. 変更をコミット (`git commit -m 'Add some AmazingFeature'`)
4. ブランチにプッシュ (`git push origin feature/AmazingFeature`)
5. プルリクエストを開く

## 📝 ライセンス

このプロジェクトはMITライセンスの下で公開されています。詳細は[LICENSE](LICENSE)ファイルをご覧ください。

## 🐛 バグ報告・機能リクエスト

問題を発見した場合や新機能のアイデアがある場合は、[Issues](https://github.com/YOUR_USERNAME/app-of-Search-2/issues)で報告してください。

## 👨‍💻 作者

**Your Name**

- GitHub: [@YOUR_USERNAME](https://github.com/YOUR_USERNAME)

## 🙏 謝辞

- [Google AI Studio](https://makersuite.google.com/) - AIモデルの提供
- [React](https://react.dev/) - UIフレームワーク
- [Tailwind CSS](https://tailwindcss.com/) - スタイリング
- [Lucide](https://lucide.dev/) - アイコン

## 📊 プロジェクト統計

![GitHub Stars](https://img.shields.io/github/stars/YOUR_USERNAME/app-of-Search-2?style=social)
![GitHub Forks](https://img.shields.io/github/forks/YOUR_USERNAME/app-of-Search-2?style=social)
![GitHub Issues](https://img.shields.io/github/issues/YOUR_USERNAME/app-of-Search-2)

---

⭐ このプロジェクトが役立ったら、スターをお願いします!
