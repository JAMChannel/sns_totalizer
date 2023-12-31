# sns_totalizer

## SNSTotalizer 用件定義

### 1. 基本情報
- **アプリ名**: SNSTotalizer
- **目的**: 複数のSNSプラットフォームのフォロワー情報を一元管理し、分析や追跡を効率化する。

### 2. 対応SNSプラットフォーム
- Instagram
- Twitter
- YouTube
- TikTok

### 3. 主要機能
#### 3.1 アカウント連携機能
- 各SNSアカウントとのOAuth連携。
- 連携時に必要なパーミッションの選択。

#### 3.2 フォロワー数表示機能
- 各SNSのフォロワー数をリアルタイムで表示。
- 総フォロワー数の集計と表示。

#### 3.3 フォロワー増減分析機能
- 日次、週次、月次での増減数と増減率をグラフ表示。

#### 3.4 インタラクション分析機能
- 各SNSの投稿ごとのいいね数、コメント数、シェア数等を表示。

#### 3.5 通知機能
- 特定の条件を満たした際に通知。

#### 3.6 フォロワーデモグラフィックス分析
- 年齢、性別、地域などのユーザーデモグラフィックス情報の分析。

### 4. 追加の便利な機能
#### 4.1 キーワードトラッキング
- ユーザーが指定したキーワードに関する言及や反応を追跡。

#### 4.2 コンペティター分析
- 他の類似アカウントや競合とのフォロワー数やエンゲージメントを比較分析。

#### 4.3 自動レポート生成
- 定期的な分析結果をPDFや画像形式で出力。

#### 4.4 フォロワーセグメンテーション
- フォロワーを特定の属性や行動に基づいてグループ化。

#### 4.5 AI推薦機能
- AIを用いて、投稿内容やタイミングの最適化提案。

### 5. セキュリティ
- ユーザー情報の暗号化と安全なストレージ。
- OAuthを用いた安全なAPI連携。
- パスワードなどのセンシティブ情報は保存しない。

### 6. ユーザーインターフェース
- モダンで直感的なUI。
- グラフやチャートでの情報表示。
- モバイル最適化とレスポンシブデザイン。


# **SNSTotalizer 機能要件一覧**

## 1. **アカウント連携機能**
- **Instagram, Twitter, YouTube, TikTok 連携**
  - OAuth認証を使用したセキュアなログイン方法
  - 各SNSのAPIとのデータ同期

## 2. **フォロワー数表示**
- **リアルタイムフォロワー数表示**
  - 各SNSごとのフォロワー数の現在値
- **フォロワー数変動グラフ**
  - 過去のデータとの比較での増減をグラフで視覚化

## 3. **フォロワー管理**
- **フォロワー一覧表示**
  - 各SNSのフォロワーとそのアクティビティ一覧
- **フォロワーの追加・削除通知**
  - リアルタイムでのフォロワーの変動通知
- **未フォローバック/相互フォロワー識別**
  - 未フォローバックや相互フォロワーのユーザーをハイライト表示

## 4. **アカウント分析**
- **投稿のエンゲージメント分析**
  - いいね、コメント、シェア数等の分析
- **投稿頻度の統計**
  - 過去の投稿頻度やアクティビティのトレンド表示

## 5. **多言語対応**
- **言語オプション**
  - 英語, 日本語, スペイン語等の選択

## 6. **通知機能**
- **アクティビティベースの通知**
  - フォロワーの増減、メンション、タグなどの主要アクティビティ通知

## 7. **ダッシュボード機能**
- **全SNS一覧画面**
  - 一覧画面で各SNSの主要情報と最新のアクティビティ表示

## 8. **セキュリティ対策**
- **パスワード暗号化**
  - 安全なパスワードストレージ
- **二要素認証オプション**
  - セキュリティ強化のための2FA導入

## 9. **バックアップ機能**
- **自動バックアップ**
  - 定期的なデータの自動バックアップ
- **バックアップからの復元**
  - バックアップデータを用いたデータ復元

## 10. **ユーザーフィードバック機能**
- **フィードバックフォーム**
  - ユーザーからのフィードバックや要望受付

## 11. **ヘルプ&サポート**
- **FAQセクション**
  - よくある質問とその回答のセクション
- **サポート問い合わせフォーム**
  - テクニカルサポートや一般的な問い合わせのためのフォーム

## 12. **プレミアム機能/サブスクリプションモデル**
- **基本無料プラン**
  - 基本的な機能を無料で提供
- **有料プラン**
  - 高度な分析や追加機能を含む有料プランオプション

# SNSTotalizer 非機能要件

### 1. パフォーマンス
- **レスポンスタイム**
  - ユーザーアクションに対するシステムのレスポンスタイムは2秒以内とする。
  
- **同時接続数**
  - システムは、最低でも1,000人のユーザーが同時に接続できることを保証する。

### 2. 可用性
- **稼働率**
  - 99.5%のアップタイムを目指す。

- **バックアップ**
  - データは毎日自動的にバックアップされる。
  - バックアップは最低7日間保存される。

### 3. セキュリティ
- **データ保護**
  - ユーザーパスワードはハッシュ化して保存する。
  - 個人情報は暗号化して保存・転送する。

- **アクセス制御**
  - 管理画面へのアクセスは特定の管理者のみに制限される。
  - 未認証・未承認のユーザーは、保護されたリソースへのアクセスが制限される。

- **セキュリティアップデート**
  - システムおよび依存ライブラリは定期的にセキュリティアップデートを適用する。

### 4. 拡張性
- **モジュール性**
  - システムはモジュール方式で設計され、新しい機能やサービスの追加が容易であること。

- **APIの提供**
  - 外部サービスやアプリケーションとの連携のためのAPIを提供する。

### 5. 使いやすさ
- **モバイル対応**
  - モバイルデバイスでの利用を考慮し、レスポンシブデザインを採用する。

- **多言語対応**
  - 主要な言語（例：英語、日本語）での表示をサポートする。

- **アクセシビリティ**
  - 視覚障害者や高齢者などの利用者も考慮したアクセシビリティのガイドラインに準拠する。

# インフラ・クラウド提案 for SNSTotalizer（Docker対応版）

### ローカル開発環境

1. **Docker**:
    - アプリケーションとその依存関係をコンテナとして実行。
    - `docker-compose` を利用して、アプリケーション、データベース、キャッシュなどのサービスを一緒に起動・終了。

### クラウドプラットフォーム: AWS (Amazon Web Services)

#### a. コンテナの実行・管理
- **Amazon ECS (Elastic Container Service)**:
    - Dockerコンテナを実行するためのサービス。Fargate起動タイプを選択すると、サーバーの管理やスケーリングの手間を省略できる。

#### b. データベース
- **Amazon RDS (Relational Database Service)**:
    - データベースのホスティング。MySQLを選択し、マルチAZ展開で高可用性を確保。

#### c. ストレージ
- **Amazon S3**:
    - 静的ファイルやバックアップの保存先として利用。

#### d. コンテンツ配信
- **Amazon CloudFront**:
    - グローバルなCDNサービス。ユーザーに近い位置からコンテンツを提供し、レスポンスタイムの短縮を図る。

#### e. セキュリティ
- **AWS WAF (Web Application Firewall)**:
    - 不正アクセスやDDoS攻撃からの保護。
- **Amazon VPC (Virtual Private Cloud)**:
    - 専用の仮想ネットワーク内でリソースを起動。パブリックおよびプライベートサブネットを利用してアクセス制御。
- **IAM (Identity and Access Management)**:
    - ユーザーやサービスの権限管理。

#### f. モニタリングとアラート
- **Amazon CloudWatch**:
    - リソースとアプリケーションの監視。異常やパフォーマンスの低下を検出し通知。


# **SNSTotalizer アプリ画面設計**

### 一般ユーザー向け画面

#### 1. ログイン/登録画面
- ユーザー名とパスワード入力フィールド
- SNSアカウントでのログインボタン
- 新規登録とパスワードを忘れた場合のリンク

#### 2. ダッシュボード
- 各SNSアカウントのフォロワー数を一覧表示
- 最近のアクティビティや通知のハイライト
- サイドバーに主要なナビゲーションリンク

#### 3. SNS詳細画面
- 選択したSNSのフォロワー数のグラフ表示
- 未フォローバック/相互フォロワーのリスト
- 最近のアクティビティと投稿のエンゲージメント分析

#### 4. アカウント設定画面
- ユーザー情報の編集
- 連携しているSNSアカウントの管理
- 通知設定
- 言語やテーマの選択

#### 5. 通知センター
- フォロワーの増減、メンション、タグなどの通知一覧
- 未読/既読の管理

#### 6. バックアップ&復元画面
- 最後のバックアップ日時の表示
- バックアップの手動トリガー
- 以前のバックアップからのデータ復元オプション

#### 7. ユーザーフィードバック/サポート
- ユーザーフィードバックの送信フォーム
- FAQセクション
- カスタマーサポートへの問い合わせフォーム

#### 8. プレミアム機能/サブスクリプション画面
- 現在のプランの詳細
- 他の利用可能なプランのリスト
- プランのアップグレード/ダウングレードオプション

### 管理者専用画面

#### 1. ユーザー管理
- ユーザー一覧表示
- ユーザー検索
- ユーザーの停止/有効化

#### 2. フィードバック管理
- ユーザーフィードバックの一覧表示
- フィードバックのステータス変更

#### 3. 通知管理
- システム全体の通知作成

#### 4. コンテンツ管理
- FAQの編集/追加
- ヘルプセクションの編集

#### 5. システム設定
- 連携可能なSNSの追加/削除
- システムのメンテナンスモード切替

#### 6. 統計情報
- アクティブユーザー数、新規登録数などの基本的な統計情報を表示
- 各SNSの人気度や使用率の統計

#### 7. サブスクリプション・支払い管理
- 有料プランのユーザー一覧と支払いステータスの確認
- 新しいプランやキャンペーンの設定




## テーブル設計とアソシエーション

### `users` テーブル
ユーザー情報を格納するテーブル。

| カラム名 | 型 | 説明 |
| :--- | :---: | ---: |
| id | INT | ユーザーID (PK) |
| username | VARCHAR | ユーザー名 |
| email | VARCHAR | メールアドレス |
| password_hash | VARCHAR | パスワードのハッシュ |
| created_at | TIMESTAMP | 登録日時 |
| updated_at | TIMESTAMP | 更新日時 |

- **アソシエーション**: 
  - `sns_accounts`: 一対多
  - `notifications`: 一対多
  - `feedbacks`: 一対多
  - `subscriptions`: 一対多

### `sns_accounts` テーブル

| カラム名 | 型 | 説明 |
| :--- | :---: | ---: |
| id | INT | ID (PK) |
| user_id | INT | ユーザーID (FK) |
| sns_type | ENUM('Instagram', 'Twitter', 'YouTube', 'TikTok') | SNSのタイプ |
| account_name | VARCHAR | アカウント名 |
| follower_count | INT | フォロワー数 |
| created_at | TIMESTAMP | 登録日時 |
| updated_at | TIMESTAMP | 更新日時 |

- **アソシエーション**: 
  - `users`: 多対一

### `notifications` テーブル

| カラム名 | 型 | 説明 |
| :--- | :---: | ---: |
| id | INT | ID (PK) |
| user_id | INT | ユーザーID (FK) |
| content | TEXT | 通知内容 |
| is_read | BOOLEAN | 既読/未読ステータス |
| created_at | TIMESTAMP | 通知日時 |

- **アソシエーション**: 
  - `users`: 多対一

### `feedbacks` テーブル

| カラム名 | 型 | 説明 |
| :--- | :---: | ---: |
| id | INT | ID (PK) |
| user_id | INT | ユーザーID (FK) |
| content | TEXT | フィードバック内容 |
| status | ENUM('New', 'In Progress', 'Resolved') | フィードバックのステータス |
| created_at | TIMESTAMP | 送信日時 |
| updated_at | TIMESTAMP | 更新日時 |

- **アソシエーション**: 
  - `users`: 多対一

### `subscriptions` テーブル

| カラム名 | 型 | 説明 |
| :--- | :---: | ---: |
| id | INT | ID (PK) |
| user_id | INT | ユーザーID (FK) |
| plan_type | ENUM('Basic', 'Premium') | プランタイプ |
| start_date | DATE | 開始日 |
| end_date | DATE | 終了日 |

- **アソシエーション**: 
  - `users`: 多対一

### `admins` テーブル

| カラム名 | 型 | 説明 |
| :--- | :---: | ---: |
| id | INT | 管理者ID (PK) |
| username | VARCHAR | 管理者ユーザー名 |
| password_hash | VARCHAR | パスワードのハッシュ |
| created_at | TIMESTAMP | 登録日時 |
| updated_at | TIMESTAMP | 更新日時 |





# SNSTotalizer ヒアリングシート

## 基本情報

- **名前**: 1. お名前をフルネームで教えてください。  
  回答: _______________

- **年齢**: 2. 年齢を教えてください。  
  回答: _______________

- **職業**: 3. ご職業を教えてください。  
  回答: _______________

## SNS使用状況

- **使用SNS**: 4. 使用しているSNSを全て教えてください。(複数回答可)  
  回答: _______________

- **使用目的**: 5. SNSを使用する主要な目的は何ですか？  
  回答: _______________

## 現行のフォロワー管理方法

- **管理方法**: 6. 現在、どのようにフォロワーを管理していますか？  
  回答: _______________

- **使用ツール**: 7. 現在使用しているツールやアプリがあれば、その名前と使用目的を教えてください。  
  回答: _______________

## 感じる課題や不便さ

- **課題・不便さ**: 8. 現在のフォロワー管理方法で感じる課題や不便さを具体的に教えてください。  
  回答: _______________

## 期待する機能

- **期待する機能**: 9. SNSTotalizerで特に実装してほしい機能やサービスは何ですか？  
  回答: _______________

## 既存ツールの不満点

- **不満点**: 10. 現在使用しているツールやアプリの具体的な不満点を教えてください。  
  回答: _______________

## 使用頻度

- **使用頻度**: 11. どのくらいの頻度でフォロワーの管理や分析を行っていますか？(例: 毎日、週1回など)  
  回答: _______________

## 予算感

- **予算**: 12. 月額または年額で考えた場合、このようなアプリに支払いたい金額の上限を教えてください。  
  回答: _______________

## オススメの参考ツールやサイト

- **参考ツール**: 13. フォロワー管理や分析に関連するおすすめのツールやサイトがあれば、教えてください。  
  回答: _______________

## その他の意見・要望

- **意見・要望**: 14. SNSTotalizerに関するその他の意見や要望、感想を自由に記載してください。  
  回答: _______________
