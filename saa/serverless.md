# サーバレス

* AWS AppSync
* AWS Fargate
* AWS Lambda

## AWS AppSync

## AWS Fargate
* コンテナ向けサーバレスコンピューティングエンジン
* ECS と EKS で利用可
* ビルド、デプロイなどのコンテナの管理を移譲

## AWS Lambda
* アプリケーションコードのデプロイのみで動作するサーバレスなサービス
* ExecutionRole でアクセス制御を設計
* ログは、CloudWatch Logs に保存
* Lambda@Edge は、Lambda とは異なり CloudFront の機能であり、ユーザーに最も近い場所で実行
* Lambda レイヤーは、複数の Lambda 関数でライブラリを共有できる仕組み

