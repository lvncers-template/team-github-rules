# Team GitHub Rules

このリポジトリは、チームでの効率的な Git 作業のためのガイドラインとテンプレートを提供します。

## プロジェクト構造

```sh
your-project-root/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── default.md
│   └── PULL_REQUEST_TEMPLATE/
│       ├── default.md
│       └── review_template.md  # レビューテンプレート
│
├── documents/
│   ├── adr/                        # 設計判断の記録
│   │   ├── 0001-use-postgresql.md
│   │   └── 0002-adopt-graphql.md
│   ├── guides/
│   │   └── getting-started.md
│   ├── runbooks/
│   │   └── incident-response.md    # 障害対応手順書
│   ├── tutorials/
│   │   └── quick-start.md
│   ├── API.md                      # API 仕様とエンドポイント
│   ├── ARCHITECTURE.md             # システム構成・設計思想
│   ├── COMMIT_CONVENTION.md        # コミットメッセージ規約
│   ├── DATABASE.md                 # データベース設計書・スキーマ定義書
│   ├── DESIGN.md                   # 設計ドキュメント
│   ├── REQUIREMENTS.md             # 要件定義書
│   └── TECH-STACK.md               # 使用技術スタック
│
├── .editorconfig       # エディタ設定
├── .gitignore
├── CHANGELOG.md        # 変更履歴
├── CODE_OF_CONDUCT.md  # 行動規範
├── CODEOWNERS          # コードオーナー定義
├── CONTRIBUTING.md     # コントリビューションガイド
├── LICENSE
├── README.md
├── RELEASE.md          # リリースノート
└── SECURITY.md         # セキュリティポリシー
```

## 作業の流れ

### 1. イシューの作成

[イシューテンプレート](./.github/ISSUE_TEMPLATE/default.md)に従って作成

### 2. ブランチの作成

ブランチ命名規則（[.github/CONTRIBUTING.md](./.github/CONTRIBUTING.md)）に準拠

### 3. 開発作業

- ローカルで作業を実施
- 定期的にコミット

### 4. コミット＆プッシュ

[コミットメッセージ規約](./.github/COMMIT_CONVENTION.md)に従う

### 5. プルリクエスト

- [PR テンプレート](./.github/PULL_REQUEST_TEMPLATE/bugfix_pr.md)に従って作成
- [レビューガイドライン](./.github/PULL_REQUEST_TEMPLATE/review_template.md)を参考にレビューを依頼

### 6. コードレビュー

建設的なレビューを実施

### 7. マージ

- レビュー承認後にマージ
- ブランチのクリーンアップ
