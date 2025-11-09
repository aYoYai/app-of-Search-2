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

<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Search & Quiz App</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .fade-in { animation: fadeIn 0.3s ease-out; }
    </style>
</head>
<body class="bg-gradient-to-br from-purple-50 to-blue-50 min-h-screen">
    <div id="app"></div>

    <script>
        class SearchQuizApp {
            constructor() {
                this.apiKey = '';
                this.isApiKeySet = false;
                this.searchQuery = '';
                this.searchResults = null;
                this.searchHistory = [];
                this.activeTab = 'search';
                this.selectedQuiz = null;
                this.userAnswer = null;
                this.showExplanation = false;
                this.expandedResults = {};
                
                // 複数のAPIエンドポイントを試す
                this.apiEndpoints = [
                    'https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent',
                    'https://generativelanguage.googleapis.com/v1/models/gemini-pro:generateContent',
                    'https://generativelanguage.googleapis.com/v1beta/models/gemini-1.5-flash:generateContent',
                    'https://generativelanguage.googleapis.com/v1/models/gemini-1.5-flash:generateContent'
                ];
                
                this.init();
            }

            init() {
                const savedKey = localStorage.getItem('gemini_api_key');
                const savedHistory = localStorage.getItem('search_history');
                
                if (savedKey) {
                    this.apiKey = savedKey;
                    this.isApiKeySet = true;
                }
                
                if (savedHistory) {
                    try {
                        this.searchHistory = JSON.parse(savedHistory);
                    } catch (e) {
                        this.searchHistory = [];
                    }
                }
                
                this.render();
            }

            saveApiKey() {
                const input = document.getElementById('apiKeyInput');
                if (input.value.trim()) {
                    this.apiKey = input.value.trim();
                    localStorage.setItem('gemini_api_key', this.apiKey);
                    this.isApiKeySet = true;
                    this.render();
                }
            }

            clearApiKey() {
                if (confirm('APIキーを削除しますか？')) {
                    localStorage.removeItem('gemini_api_key');
                    this.apiKey = '';
                    this.isApiKeySet = false;
                    this.render();
                }
            }

            async callGeminiAPI(prompt) {
                let lastError = null;
                
                // 複数のエンドポイントを順番に試す
                for (const endpoint of this.apiEndpoints) {
                    try {
                        console.log('Trying endpoint:', endpoint);
                        
                        const response = await fetch(`${endpoint}?key=${this.apiKey}`, {
                            method: 'POST',
                            headers: { 'Content-Type': 'application/json' },
                            body: JSON.stringify({
                                contents: [{
                                    parts: [{ text: prompt }]
                                }],
                                generationConfig: {
                                    temperature: 0.7,
                                    maxOutputTokens: 2048,
                                }
                            })
                        });

                        const data = await response.json();
                        console.log('API Response:', data);

                        // エラーチェック
                        if (!response.ok) {
                            console.warn(`Endpoint ${endpoint} failed:`, data);
                            lastError = new Error(data.error?.message || `HTTP ${response.status}`);
                            continue;
                        }

                        // レスポンス構造の確認（複数のパターンに対応）
                        let resultText = null;
                        
                        // パターン1: candidates[0].content.parts[0].text
                        if (data.candidates?.[0]?.content?.parts?.[0]?.text) {
                            resultText = data.candidates[0].content.parts[0].text;
                        }
                        // パターン2: candidates[0].output
                        else if (data.candidates?.[0]?.output) {
                            resultText = data.candidates[0].output;
                        }
                        // パターン3: text フィールド直接
                        else if (data.text) {
                            resultText = data.text;
                        }
                        // パターン4: content フィールド
                        else if (data.content) {
                            resultText = data.content;
                        }

                        if (resultText) {
                            console.log('Success with endpoint:', endpoint);
                            return resultText;
                        }

                        console.warn(`Unexpected response structure from ${endpoint}:`, data);
                        lastError = new Error('レスポンスの形式が不正です');
                        
                    } catch (error) {
                        console.warn(`Error with endpoint ${endpoint}:`, error);
                        lastError = error;
                    }
                }

                // すべてのエンドポイントが失敗
                throw lastError || new Error('すべてのAPIエンドポイントで失敗しました');
            }

            async performSearch() {
                const input = document.getElementById('searchInput');
                this.searchQuery = input.value.trim();
                
                if (!this.searchQuery || !this.isApiKeySet) return;

                const searchBtn = document.getElementById('searchBtn');
                searchBtn.disabled = true;
                searchBtn.innerHTML = '<span class="animate-spin">🔄</span> 検索中...';

                try {
                    // 検索と要約
                    const searchPrompt = `以下の検索クエリについて、詳しく調べて回答してください。

検索クエリ: ${this.searchQuery}

以下の2つを必ず含めてください:
1. 300文字以内の簡潔な要約
2. 詳細な説明（できるだけ詳しく）

以下のJSON形式で必ず回答してください:
{
  "summary": "ここに300文字以内の要約",
  "fullText": "ここに詳細な説明"
}`;

                    console.log('Searching for:', this.searchQuery);
                    const resultText = await this.callGeminiAPI(searchPrompt);
                    
                    let parsedResult;
                    try {
                        // JSONを抽出
                        const jsonMatch = resultText.match(/\{[\s\S]*\}/);
                        if (jsonMatch) {
                            parsedResult = JSON.parse(jsonMatch[0]);
                        } else {
                            // JSONが見つからない場合は、テキストをそのまま使用
                            const text = resultText.trim();
                            parsedResult = {
                                summary: text.substring(0, 300),
                                fullText: text
                            };
                        }
                    } catch (e) {
                        console.warn('JSON parsing failed, using raw text:', e);
                        parsedResult = {
                            summary: resultText.substring(0, 300),
                            fullText: resultText
                        };
                    }

                    console.log('Parsed result:', parsedResult);

                    // クイズ生成
                    const quizPrompt = `以下の情報から4択クイズを作成してください。

検索クエリ: ${this.searchQuery}
説明: ${parsedResult.summary}

重要なルール:
1. 問題文は「${this.searchQuery}」を60文字程度で説明する文章にしてください
2. 問題文に「${this.searchQuery}」という単語自体は絶対に含めないでください
3. 正解の選択肢は「${this.searchQuery}」にしてください
4. 他の3つの選択肢は間違いで、でも関連する言葉にしてください
5. 解説は教育的でわかりやすく書いてください

必ず以下のJSON形式で回答してください:
{
  "question": "問題文（60文字程度）",
  "options": ["${this.searchQuery}", "間違い選択肢1", "間違い選択肢2", "間違い選択肢3"],
  "correctAnswer": 0,
  "explanation": "解説文"
}`;

                    let quiz = null;
                    try {
                        console.log('Generating quiz...');
                        const quizText = await this.callGeminiAPI(quizPrompt);
                        const quizJsonMatch = quizText.match(/\{[\s\S]*\}/);
                        if (quizJsonMatch) {
                            quiz = JSON.parse(quizJsonMatch[0]);
                            console.log('Quiz generated:', quiz);
                        }
                    } catch (e) {
                        console.warn('Quiz generation failed:', e);
                    }

                    const newResult = {
                        id: Date.now(),
                        query: this.searchQuery,
                        summary: parsedResult.summary,
                        fullText: parsedResult.fullText,
                        quiz: quiz,
                        timestamp: new Date().toISOString()
                    };

                    this.searchResults = newResult;
                    this.searchHistory.unshift(newResult);
                    localStorage.setItem('search_history', JSON.stringify(this.searchHistory));
                    
                    console.log('Search completed successfully');
                    this.render();
                    
                } catch (error) {
                    console.error('Search error:', error);
                    let errorMessage = '検索エラーが発生しました: ' + error.message;
                    
                    if (error.message.includes('API key') || error.message.includes('401')) {
                        errorMessage += '\n\n❌ APIキーが無効です。以下を確認してください:\n';
                        errorMessage += '1. Google AI Studio (https://makersuite.google.com/app/apikey) でAPIキーを取得\n';
                        errorMessage += '2. APIキーを正しくコピーしているか確認\n';
                        errorMessage += '3. APIキーが有効化されているか確認';
                    } else if (error.message.includes('quota') || error.message.includes('429')) {
                        errorMessage += '\n\n❌ API利用制限に達しました。しばらく待ってから再試行してください。';
                    }
                    
                    alert(errorMessage);
                } finally {
                    searchBtn.disabled = false;
                    searchBtn.innerHTML = '🔍 検索';
                }
            }

            clearHistory() {
                if (confirm('検索履歴を全て削除しますか？')) {
                    this.searchHistory = [];
                    localStorage.removeItem('search_history');
                    this.render();
                }
            }

            toggleExpand(id) {
                this.expandedResults[id] = !this.expandedResults[id];
                this.render();
            }

            selectQuiz(item) {
                this.selectedQuiz = item;
                this.userAnswer = null;
                this.showExplanation = false;
                this.render();
            }

            submitAnswer(index) {
                if (!this.showExplanation) {
                    this.userAnswer = index;
                    this.showExplanation = true;
                    this.render();
                }
            }

            render() {
                const app = document.getElementById('app');
                
                if (!this.isApiKeySet) {
                    app.innerHTML = this.renderApiKeyScreen();
                } else {
                    app.innerHTML = this.renderMainScreen();
                }
                
                this.attachEventListeners();
            }

            renderApiKeyScreen() {
                return `
                    <div class="min-h-screen flex items-center justify-center p-4">
                        <div class="bg-white rounded-2xl shadow-xl p-8 max-w-md w-full fade-in">
                            <div class="flex items-center justify-center mb-6">
                                <div class="w-12 h-12 text-4xl">🔑</div>
                            </div>
                            <h1 class="text-2xl font-bold text-center mb-2 text-gray-800">
                                AI Search & Quiz
                            </h1>
                            <p class="text-center text-gray-600 mb-6">
                                Google AI Studio APIキーを入力してください
                            </p>
                            <input
                                id="apiKeyInput"
                                type="password"
                                placeholder="AIzaSy... で始まるAPIキーを入力"
                                class="w-full px-4 py-3 border-2 border-gray-200 rounded-lg focus:border-purple-500 focus:outline-none mb-4"
                            />
                            <button
                                onclick="app.saveApiKey()"
                                class="w-full bg-purple-600 text-white py-3 rounded-lg font-semibold hover:bg-purple-700 transition"
                            >
                                開始
                            </button>
                            <div class="mt-6 p-4 bg-blue-50 rounded-lg">
                                <p class="text-sm font-semibold text-gray-700 mb-2">
                                    📝 APIキーの取得方法:
                                </p>
                                <ol class="text-sm text-gray-600 list-decimal list-inside space-y-1">
                                    <li>下のリンクをクリック</li>
                                    <li>Googleアカウントでログイン</li>
                                    <li>「Create API Key」をクリック</li>
                                    <li>APIキーをコピーして上に貼り付け</li>
                                </ol>
                                <a href="https://aistudio.google.com/app/apikey" target="_blank" class="inline-block mt-3 text-sm text-white bg-purple-600 hover:bg-purple-700 px-4 py-2 rounded-lg transition">
                                    🔗 Google AI Studioを開く
                                </a>
                            </div>
                            <p class="text-xs text-gray-500 mt-4 text-center">
                                APIキーはブラウザのローカルストレージにのみ保存されます
                            </p>
                        </div>
                    </div>
                `;
            }

            renderMainScreen() {
                return `
                    <div class="max-w-6xl mx-auto p-4">
                        <header class="bg-white rounded-2xl shadow-lg p-6 mb-6 fade-in">
                            <div class="flex items-center justify-between mb-4">
                                <h1 class="text-3xl font-bold bg-gradient-to-r from-purple-600 to-blue-600 bg-clip-text text-transparent">
                                    AI Search & Quiz
                                </h1>
                                <button
                                    onclick="app.clearApiKey()"
                                    class="text-red-500 hover:text-red-700 text-sm flex items-center gap-1"
                                >
                                    🔑 APIキー削除
                                </button>
                            </div>
                            ${this.activeTab === 'search' ? `
                                <div class="flex gap-2">
                                    <input
                                        id="searchInput"
                                        type="text"
                                        placeholder="検索クエリを入力... (例: 人工知能、量子コンピュータ)"
                                        class="flex-1 px-4 py-3 border-2 border-gray-200 rounded-lg focus:border-purple-500 focus:outline-none"
                                        onkeypress="if(event.key==='Enter') app.performSearch()"
                                    />
                                    <button
                                        id="searchBtn"
                                        onclick="app.performSearch()"
                                        class="bg-purple-600 text-white px-6 py-3 rounded-lg font-semibold hover:bg-purple-700 transition"
                                    >
                                        🔍 検索
                                    </button>
                                </div>
                            ` : ''}
                        </header>

                        <div class="flex gap-2 mb-6">
                            <button
                                onclick="app.activeTab='search'; app.render()"
                                class="flex-1 py-3 rounded-lg font-semibold transition ${
                                    this.activeTab === 'search'
                                        ? 'bg-purple-600 text-white'
                                        : 'bg-white text-gray-600 hover:bg-gray-50'
                                }"
                            >
                                🔍 検索
                            </button>
                            <button
                                onclick="app.activeTab='history'; app.render()"
                                class="flex-1 py-3 rounded-lg font-semibold transition ${
                                    this.activeTab === 'history'
                                        ? 'bg-purple-600 text-white'
                                        : 'bg-white text-gray-600 hover:bg-gray-50'
                                }"
                            >
                                📜 履歴
                            </button>
                            <button
                                onclick="app.activeTab='quiz'; app.render()"
                                class="flex-1 py-3 rounded-lg font-semibold transition ${
                                    this.activeTab === 'quiz'
                                        ? 'bg-purple-600 text-white'
                                        : 'bg-white text-gray-600 hover:bg-gray-50'
                                }"
                            >
                                📚 クイズ
                            </button>
                        </div>

                        ${this.renderTabContent()}
                    </div>
                `;
            }

            renderTabContent() {
                if (this.activeTab === 'search') {
                    return this.renderSearchTab();
                } else if (this.activeTab === 'history') {
                    return this.renderHistoryTab();
                } else {
                    return this.renderQuizTab();
                }
            }

            renderSearchTab() {
                if (!this.searchResults) return '';
                
                return `
                    <div class="bg-white rounded-2xl shadow-lg p-6 fade-in">
                        <h2 class="text-xl font-bold mb-4 text-gray-800">検索結果</h2>
                        <div class="mb-4">
                            <h3 class="font-semibold text-purple-600 mb-2">検索クエリ:</h3>
                            <p class="text-gray-700">${this.searchResults.query}</p>
                        </div>
                        <div class="mb-4">
                            <h3 class="font-semibold text-purple-600 mb-2">要約 (300文字以内):</h3>
                            <p class="text-gray-700 leading-relaxed">${this.searchResults.summary}</p>
                        </div>
                        <div>
                            <div class="flex items-center justify-between mb-2">
                                <h3 class="font-semibold text-purple-600">全文:</h3>
                                <button
                                    onclick="app.toggleExpand(${this.searchResults.id})"
                                    class="text-purple-600 hover:text-purple-700 text-sm"
                                >
                                    ${this.expandedResults[this.searchResults.id] ? '▲ 閉じる' : '▼ 展開'}
                                </button>
                            </div>
                            ${this.expandedResults[this.searchResults.id] ? `
                                <div class="bg-gray-50 p-4 rounded-lg">
                                    <p class="text-gray-700 leading-relaxed whitespace-pre-wrap">${this.searchResults.fullText}</p>
                                </div>
                            ` : ''}
                        </div>
                    </div>
                `;
            }

            renderHistoryTab() {
                if (this.searchHistory.length === 0) {
                    return `
                        <div class="bg-white rounded-2xl shadow-lg p-6">
                            <h2 class="text-xl font-bold mb-4 text-gray-800">検索履歴</h2>
                            <p class="text-gray-500 text-center py-8">検索履歴がありません</p>
                        </div>
                    `;
                }

                return `
                    <div class="bg-white rounded-2xl shadow-lg p-6 fade-in">
                        <div class="flex items-center justify-between mb-4">
                            <h2 class="text-xl font-bold text-gray-800">検索履歴</h2>
                            <button
                                onclick="app.clearHistory()"
                                class="text-red-500 hover:text-red-700 text-sm"
                            >
                                🗑️ 全削除
                            </button>
                        </div>
                        <div class="space-y-4">
                            ${this.searchHistory.map(item => `
                                <div class="border-2 border-gray-200 rounded-lg p-4 hover:border-purple-300 transition">
                                    <div class="flex items-start justify-between mb-2">
                                        <h3 class="font-semibold text-gray-800">${item.query}</h3>
                                        <span class="text-xs text-gray-500">
                                            ${new Date(item.timestamp).toLocaleString('ja-JP')}
                                        </span>
                                    </div>
                                    <p class="text-gray-600 text-sm mb-2">${item.summary.substring(0, 100)}...</p>
                                    <button
                                        onclick="app.toggleExpand(${item.id})"
                                        class="text-purple-600 hover:text-purple-700 text-sm"
                                    >
                                        ${this.expandedResults[item.id] ? '▲ 閉じる' : '▼ 全文を見る'}
                                    </button>
                                    ${this.expandedResults[item.id] ? `
                                        <div class="mt-3 bg-gray-50 p-3 rounded-lg">
                                            <p class="text-gray-700 text-sm leading-relaxed whitespace-pre-wrap">${item.fullText}</p>
                                        </div>
                                    ` : ''}
                                </div>
                            `).join('')}
                        </div>
                    </div>
                `;
            }

            renderQuizTab() {
                const quizHistory = this.searchHistory.filter(item => item.quiz);
                
                if (quizHistory.length === 0) {
                    return `
                        <div class="bg-white rounded-2xl shadow-lg p-6">
                            <h2 class="text-xl font-bold mb-4 text-gray-800">クイズ</h2>
                            <p class="text-gray-500 text-center py-8">
                                クイズがありません。検索を行うとクイズが生成されます。
                            </p>
                        </div>
                    `;
                }

                if (!this.selectedQuiz) {
                    return `
                        <div class="bg-white rounded-2xl shadow-lg p-6 fade-in">
                            <h2 class="text-xl font-bold mb-4 text-gray-800">クイズ</h2>
                            <div class="space-y-3">
                                ${quizHistory.map((item, index) => `
                                    <button
                                        onclick='app.selectQuiz(${JSON.stringify(item).replace(/'/g, "&#39;")})'
                                        class="w-full text-left border-2 border-gray-200 rounded-lg p-4 hover:border-purple-300 transition"
                                    >
                                        <h3 class="font-semibold text-gray-800 mb-1">${item.query}</h3>
                                        <p class="text-sm text-gray-600">
                                            ${new Date(item.timestamp).toLocaleString('ja-JP')}
                                        </p>
                                    </button>
                                `).join('')}
                            </div>
                        </div>
                    `;
                }

                const quiz = this.selectedQuiz.quiz;
                return `
                    <div class="bg-white rounded-2xl shadow-lg p-6 fade-in">
                        <button
                            onclick="app.selectedQuiz=null; app.render()"
                            class="text-purple-600 hover:text-purple-700 mb-4 text-sm"
                        >
                            ← クイズ一覧に戻る
                        </button>
                        <div class="bg-purple-50 rounded-lg p-6 mb-6">
                            <h3 class="text-lg font-semibold mb-4 text-gray-800">
                                ${quiz.question}
                            </h3>
                            <div class="space-y-3">
                                ${quiz.options.map((option, index) => `
                                    <button
                                        onclick="app.submitAnswer(${index})"
                                        ${this.showExplanation ? 'disabled' : ''}
                                        class="w-full text-left p-4 rounded-lg border-2 transition ${
                                            this.showExplanation
                                                ? index === quiz.correctAnswer
                                                    ? 'border-green-500 bg-green-50'
                                                    : index === this.userAnswer
                                                    ? 'border-red-500 bg-red-50'
                                                    : 'border-gray-200 bg-gray-50'
                                                : 'border-gray-200 hover:border-purple-300 bg-white cursor-pointer'
                                        }"
                                    >
                                        <span class="font-semibold mr-2">${String.fromCharCode(65 + index)}.</span>
                                        ${option}
                                    </button>
                                `).join('')}
                            </div>
                        </div>
                        ${this.showExplanation ? `
                            <div class="rounded-lg p-6 ${
                                this.userAnswer === quiz.correctAnswer
                                    ? 'bg-green-50 border-2 border-green-200'
                                    : 'bg-red-50 border-2 border-red-200'
                            }">
                                <h4 class="font-bold text-lg mb-2">
                                    ${this.userAnswer === quiz.correctAnswer ? '✅ 正解!' : '❌ 不正解'}
                                </h4>
                                <p class="text-gray-700 mb-2">
                                    <strong>正解:</strong> ${quiz.options[quiz.correctAnswer]}
                                </p>
                                <div class="bg-white rounded-lg p-4 mt-4">
                                    <h5 class="font-semibold mb-2 text-purple-600">解説:</h5>
                                    <p class="text-gray-700 leading-relaxed">
                                        ${quiz.explanation}
                                    </p>
                                </div>
                            </div>
                        ` : ''}
                    </div>
                `;
            }

            attachEventListeners() {
                const apiKeyInput = document.getElementById('apiKeyInput');
                if (apiKeyInput) {
                    apiKeyInput.addEventListener('keypress', (e) => {
                        if (e.key === 'Enter') this.saveApiKey();
                    });
                }
            }
        }

        const app = new SearchQuizApp();
    </script>
</body>
</html>
---

⭐ このプロジェクトが役立ったら、スターをお願いします!
