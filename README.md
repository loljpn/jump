# ジャンプサイト

特定のURLに即座にリダイレクトするシンプルなサイトです。

## 使い方

**ジャンプ先を変更する方法**
- `index.html` を開く
- 7行目の `JUMP_URL` の値を変更する
```javascript
const JUMP_URL = "https://example.com"; // ← ここを編集
```

## VS CodeからGitHub Pagesにデプロイ

### 初回セットアップ（1回だけ）

1. **GitHubアカウント作成**（持っていない場合）
   - https://github.com にアクセスして登録

2. **VS Codeでソース管理を開く**
   - 左サイドバーの「ソース管理」アイコンをクリック
   - または `Ctrl+Shift+G`

3. **初回コミット**
   - 「変更をステージ」をクリック
   - メッセージ欄に「Initial commit」と入力
   - 「コミット」をクリック

4. **GitHubにプッシュ**
   - 「リモートの発行」をクリック
   - リポジトリ名を入力（例: `jump`）
   - 「GitHub に発行（公開）」を選択
   - GitHubアカウントでログイン

5. **GitHub Pagesを有効化**
   - ブラウザでGitHubリポジトリを開く
   - `Settings` タブ → 左メニューの `Pages`
   - Branch: `main` を選択 → `Save`
   - 数分待つと公開URL表示: `https://ユーザー名.github.io/jump`

### ジャンプ先を変更してデプロイ（2回目以降）

1. `index.html` の `JUMP_URL` を編集
2. VS Codeの「ソース管理」を開く
3. 「変更をステージ」→ メッセージ入力 → 「コミット」
4. 「同期の変更」をクリック
5. 1-2分で自動デプロイ完了！

## ローカルでテスト

`index.html` をブラウザで直接開くだけでテストできます。
