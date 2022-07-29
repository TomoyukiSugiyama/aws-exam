# コンピューティング

* Amazon EC2
* AWS Elastic Beanstalk
* Amazon Elastic Container Service (Amazon ECS)
* Amazon Elastic Kubernetes Service (Amazon EKS)
* Elastic Load Balancing
* AWS Fargate
* AWS Lambda

# Amazon EC2
* 仮想サーバ
* Amazon Machine Image (AMI) から起動
* AWS Marketplace にはミドルウェアがインストール済みのサードパーティー製 AMP が用意
* AMI は、EBS-Backed、Instance Store-Backed に分類
* EBS-Backed インスタンスは、EBS を OS のルート領域として利用
* Instance Store-Backed インスタンスは、インスタンスストアを OS のルート領域として利用

## Amazon Elastic Container Service (Amazon ECS)
* フルマネージド型のコンテナオーケストレーション
* Docker 向け

## Amazon Elastic Kubernetes Service (Amazon EKS)
* フルマネージド型のコンテナオーケストレーション
* Kubernetes 向け

## Elastic Load Balancing
* ロードバランシング
* CLB、ALB、NLB に分類
* CLB は、標準的なロードバランシング
* ALB は、リクエストレベル (レイヤー7) で動作し、HTTP、HTTPS トラフィックを振り分ける
* NLB は、レイヤー7 で動作し、低レイテンシー、高いスループット
* 複数の AZ へ分散する高可用性
* ELB 自体に冗長化が確保され、自動でスケール
* SSL 復号
* ヘルスチェックを行い、インスタンスへの振り分けを停止
* スティッキーセッションにより、一度セッションを確立したインスタンスへユーザのリクエストを送信
* Connection Draining によりサーバーの処理が完了するまで解除を遅延
* クロスゾーン負荷分散により、複数の AZ にリクエストを均等に分散
* 外部 ELB (インターネット公開向け) と内部 ELB に分類

## AWS Fargate
* コンテナ向けサーバレスコンピューティングエンジン
* ECS と EKS で利用可
* ビルド、デプロイなどのコンテナの管理を移譲

## AWS Lambda
* アプリケーションコードのデプロイのみで動作するサーバレスなサービス
* ExecutionRole でアクセス制御を設計
* ログは、CloudWatch Logs に保存
* Lambda@Edge は、Lambda とは異なり CloudFront の機能であり、ユーザーに最も近い場所で実行

