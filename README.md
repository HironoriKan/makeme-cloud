# MakeMe Cloud

Beautician training platform for the cosmetics industry.

## Vercelへのデプロイ方法

このプロジェクトはVercelでのデプロイに対応しています。以下の手順でデプロイしてください：

### 1. Vercelアカウントの作成

[Vercel](https://vercel.com)にアクセスし、アカウントを作成します。GitHubアカウントでログインすると簡単です。

### 2. プロジェクトのインポート

1. Vercelダッシュボードで「New Project」をクリック
2. 「Import Git Repository」でこのリポジトリを選択
3. デフォルト設定で「Deploy」をクリック

### 3. 自動デプロイの設定

GitHub Actionsを使用した自動デプロイを有効にするには：

1. Vercelでプロジェクトの設定ページを開く
2. 「Settings」→「General」→「Tokens」から新しいトークンを作成
3. GitHubリポジトリの「Settings」→「Secrets and variables」→「Actions」で新しいシークレットを追加
   - 名前: `VERCEL_TOKEN`
   - 値: 作成したVercelトークン

これで、mainブランチへのプッシュ時に自動的にVercelへデプロイされます。
