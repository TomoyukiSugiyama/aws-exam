- [サーバレス](#サーバレス)
  - [AWS AppSync](#aws-appsync)
  - [AWS Fargate](#aws-fargate)
  - [AWS Lambda](#aws-lambda)

# サーバレス

## AWS AppSync
* 最新のウェブおよびモバイルアプリケーションの構築を簡素化するサーバーレス GraphQL および Pub/Sub API のサービス
* GraphQL は複数のデータベース、マイクロサービス、および API から安全にデータをクエリまたは更新するための単一のエンドポイントを提供すること
* Pub/Sub API はサーバーレスの WebSocket 接続を介してサブスクライブした API クライアントにデータの更新を自動的に発行

## AWS Fargate
* コンテナ向けサーバレスコンピューティングエンジン
* ECS と EKS で利用可
* ビルド、デプロイなどのコンテナの管理を移譲
* バックエンドインフラストラクチャをプロビジョニングおよび管理が不要

## AWS Lambda
* アプリケーションコードのデプロイのみで動作するサーバレスなサービス
* ExecutionRole でアクセス制御を設計
* ログは、CloudWatch Logs に保存
* Lambda@Edge は、Lambda とは異なり CloudFront の機能であり、ユーザーに最も近い場所で実行
* Lambda レイヤーは、複数の Lambda 関数でライブラリを共有できる仕組み
