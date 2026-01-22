# 🚀 itsMe - エンジニア向けポートフォリオ作成サービス

## 🎯 プロジェクトの背景と目的 (Background & Purpose)

### 1. 開発プロセスの正常化：API主導のモダン開発への転換
現在、実務では **CodeIgniter / Zend** 環境下で **Smarty / Twig** などのテンプレートエンジンを使用。<br>
バックエンドエンジニアがHTML内に直接 **変数バインド、ループ、条件分岐（if文など）** を記述しており、ロジックとビューが 密結合していることが大きな課題。

本プロジェクトでは、一人で全行程を担当しながらも、あえて **APIサーバーとクライアントを完全に独立させたモダンなアーキテクチャ** を採用し、以下の実現を目指す。

- **完全な責務分離**: テンプレート内でのロジック制御を排除。バックエンドは純粋なデータ（JSON）提供に特化し、フロントエンド側でレンダリングを行うシステムを構築。
- **専門性の向上**: HTMLの雑務から解放され、ビジネスロジック、APIデザイン、DB設計といったバックエンド本来の専門領域に注力できる環境を自ら作り出す。

### 2. 技術的挑戦とモダン化 (Modernization)
- **Framework**: Laravel 11 を活用し、RESTful な API 設計とモダンな PHP 開発を。
- **Infrastructure**: **AWS RDS** を活用したクラウドネイティブな構成を導入することで、本番運用を想定したスケーラビリティを確保します。

## 📅 開発ログ (Development Log)
### [2026-01-22] プロジェクトのキックオフ
- **Laravel 11 プロジェクト生成**: Composer を使用した最新バージョンの Laravel 環境構築。
- **GitHub**: リポジトリの初期化およびリモート連携、コードPUSH完了。
- **IDE Setup**: PhpStorm を活用した開発ワークフローの最適化（Artisan構成の自動化、実行構成の設定）
- **Issue Handling**:
    - `MissingAppKeyException`: `key:generate` による**Application Key** の生成と設定
    - `Database.sqlite`: 初期DBエラーの解消, MySQL(`.env`) への切り替え準備
- **Current Status**: ローカルでの基本動作を確認。(LaravelHome画面ブラウザーで確認)

🚀 次のステップ (Next Steps)
- AWS RDS 構築着手

