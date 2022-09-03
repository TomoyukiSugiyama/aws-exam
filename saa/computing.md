- [コンピューティング](#コンピューティング)
  - [AWS Batch](#aws-batch)
  - [Amazon EC2](#amazon-ec2)
  - [Amazon EC2 Auto Scaling](#amazon-ec2-auto-scaling)
  - [AWS Elastic Beanstalk](#aws-elastic-beanstalk)
  - [AWS Outposts](#aws-outposts)
  - [AWS Serverless Application Repository](#aws-serverless-application-repository)
  - [VMware Cloud on AWS](#vmware-cloud-on-aws)
  - [AWS Wavelength](#aws-wavelength)

# コンピューティング

## AWS Batch
* フルマネージド型バッチ処理

## Amazon EC2
* 仮想サーバ
* Amazon Machine Image (AMI) から起動
* AWS Marketplace にはミドルウェアがインストール済みのサードパーティー製 AMP が用意
* AMI は、EBS-Backed、Instance Store-Backed に分類
* EBS-Backed インスタンスは、EBS を OS のルート領域として利用
* Instance Store-Backed インスタンスは、インスタンスストアを OS のルート領域として利用
* Instance Store-Backed インスタンスは、インスタンスの存続期間中のみデータを保持するため、インスタンスが終了すると同時にデータは自動的に削除
* Dedicated Host は、物理的にサーバーを占有するインスタンスタイプ
* ハードウェア占有インスタンスはホスト HW のレベルで他の AWS アカウントに属するインスタンスから物理的に分離するが、同じ AWS アカウントのインスタンスとは HW を共有する可能性有り
* ベアメタルは、アプリケーションが基盤となるサーバーのプロセッサとメモリーに直接アクセス可能なインスタンス
* オンデマンドインスタンスは、複数のアカウントで物理的なサーバーを共有

## Amazon EC2 Auto Scaling
* 条件に応じて EC2 インスタンスを自動的に追加または削除

## AWS Elastic Beanstalk
* Web アプリケーションやサービスをサーバーにデプロイ
* 実行環境の管理
* 自動的に容量のプロビジョニング、負荷分散、拡張、アプリケーションの状態の監視
* Java、.NET、PHP、Node.js、Python、Ruby、Go が利用可
* アプリケーションのデプロイ先は、Apache HTTP Server、Nginx、Passenger、Microsoft Internet Information Service (IIS)など

## AWS Outposts
* AWS インフラストラクチャとサービスを事実上すべてのオンプレミスまたはエッジロケーションに提供

## AWS Serverless Application Repository
* サーバーレスアプリケーション用のマネージド型リポジトリ

## VMware Cloud on AWS
* VMwareのエンタープライズクラスのSoftware-Defined データセンターアーキテクチャをクラウド上で実現する、フルマネージドで共同エンジニアリングされたサービス

## AWS Wavelength
* AWS コンピューティングおよびストレージサービスを 5G ネットワーク内に組み込んで、超低レイテンシーアプリケーションの開発、デプロイおよびスケーリングのためのモバイルエッジコンピューティングインフラストラクチャ
