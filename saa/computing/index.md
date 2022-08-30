# コンピューティング

* AWS Batch
* Amazon EC2
* Amazon EC2 Auto Scaling
* AWS Elastic Beanstalk
* AWS Outposts
* AWS Serverless Application Repository
* VMware Cloud on AWS
* AWS Wavelength
* () Elastic Load Balancing

## AWS Batch

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

## AWS Elastic Beanstalk
* Web アプリケーションやサービスをサーバーにデプロイ
* 実行環境の管理
* 自動的に容量のプロビジョニング、負荷分散、拡張、アプリケーションの状態の監視
* Java、.NET、PHP、Node.js、Python、Ruby、Go が利用可
* アプリケーションのデプロイ先は、Apache HTTP Server、Nginx、Passenger、Microsoft Internet Information Service (IIS)など

## AWS Outposts

## AWS Serverless Application Repository

## VMware Cloud on AWS

## AWS Wavelength

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
