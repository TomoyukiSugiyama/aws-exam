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

## AWS Lambda
* アプリケーションコードのデプロイのみで動作するサーバレスなサービス
* ExecutionRole でアクセス制御を設計
* ログは、CloudWatch Logs に保存
* Lambda@Edge は、Lambda とは異なり CloudFront の機能であり、ユーザーに最も近い場所で実行

