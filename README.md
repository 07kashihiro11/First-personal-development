## 概要
「DailyDrift」は、日々の学習や趣味活動を1分以内の動画でシェアし、ポジティブなAIフィードバックをもらえるメディアプラットフォームです。

## 主な機能
・ユーザーが1分間の短い動画を録音し、日々の学習や趣味の取り組みを投稿する。  
・AIアシスタント「どりちゃん」が、ユーザーの投稿に対してポジティブなフィードバックを提供する。  
・デイリーチャレンジ機能で、ユーザーが小さな目標を達成したときにお祝いメッセージを送る。

## プロジェクト計画
MVPの設定:  
最初のリリースでは、1分間の動画/音声投稿、フィードバックコメント生成、デイリーチャレンジの3つの基本機能に絞る。  
スプリント1: Reactでのフロントエンド設計、ユーザーインターフェースの構築（4日）  
スプリント2: Node.jsとSupabaseを使ったバックエンドの構築、データベース設計（1週間）  
スプリント3: AWSへのデプロイ、OpenAI APIによるフィードバックシステムの統合（1週間）  
スプリント4: テスト、バグ修正、UI/UXの微調整（3日）

## 使用技術
- フロントエンド: React (TypeScript)
- バックエンド: Node.js,Express,AWS (EC2, S3)
- データベース：Supabase
- API:OpenAI
- 認証とセキュリティ:Supabase
- デプロイ:AWS (EC2, S3)

## その他
・GitHubプロジェクト管理...  
GitHubでリポジトリを作成し、Issueをベースにしたスプリント計画を立てます。Issueには各機能ごとのタスクを細かく書き、コミットとプルリクエストを管理する。  
・Dockerで環境構築  
・CI/CDパイプラインの構築...  
GitHub Actionsを使い、リポジトリにプッシュされたコードが自動的にビルドされ、テストが行われるよう設定する。テストに成功すれば、AWSEC2に自動的にデプロイされる。  
・CloudWatchでのログ管理...  
サーバーの状態やエラーログを常時監視し、異常が発生した場合はすぐにアラートを受け取れるようにする。

