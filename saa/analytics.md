- [アナリティクス](#アナリティクス)
  - [Amazon Athena](#amazon-athena)
  - [AWS Data Exchange](#aws-data-exchange)
  - [AWS Data Pipeline](#aws-data-pipeline)
  - [Amazon EMR](#amazon-emr)
  - [AWS Glue](#aws-glue)
  - [Amazon Kinesis](#amazon-kinesis)
  - [AWS Lake Formation](#aws-lake-formation)
  - [Amazon Managed Streaming for Apache Kafka (Amazon MSK)](#amazon-managed-streaming-for-apache-kafka-amazon-msk)
  - [Amazon OpenSearch Service (Amazon Elasticsearch Service)](#amazon-opensearch-service-amazon-elasticsearch-service)
  - [Amazon QuickSight](#amazon-quicksight)
  - [Amazon Redshift](#amazon-redshift)

# アナリティクス

## Amazon Athena
* サーバレスのクエリサービス
* Amazon S3 に保存されたデータに対して標準的な SQL を実行可能

## AWS Data Exchange
* サードパーティーが提供するデータセットを購読、利用できるサービス
* Amazon S3、Amazon API Gateway、Amazon Redshift、AWS Marketplace と関連する
* 購読者は、Amazon S3 にデータセットをエクスポート可能
* 購読者は、プログラムで API を呼び出したり、AWS Data Exchange コンソールから API を呼び出したり、OpenAPI 仕様ファイルをダウンロードしたりすることが可能
* Amazon Redshift のデータセットをサポート
* AWS Data Exchange はデータセットが AWS Marketplace で製品として公開されることを許可

## AWS Data Pipeline
* 指定された間隔で、AWS の様々なコンピューティングサービスやストレージサービスのほか、オンプレミスのデータソース間で信頼性の高いデータ処理やデータ移動を行うことを支援するサービス

## Amazon EMR
* 大量のデータを迅速、容易に、かつコスト効果よく処理するための Web サービス
* Apache Spark、Apache Hive、Presto などのオープンソース分析フレームワークを使用
* MACHINE LEARNING、抽出・変換・読み取り、クリックストリーム分析、リアルタイムストリーミング データ処理、インタラクティブ分析、ゲノミクスなどに利用

## AWS Glue
* 分析、機械学習、アプリケーション開発のためのデータの検出、準備、結合を簡単に行える、サーバーレスデータ統合サービス

## Amazon Kinesis
* リアルタイムに流れてくるデータの処理 (ストリーミング処理)
* Kinesis Data Stream、Kinesis Data Firehose、Kinesis Data Analyticsからなる
* Kinesis Data Stream は、ストリーミングデータを収集。シャードと呼ばれる単位でデータを分割して並列処理
* Kinesis Data Firehose は、ストリーミングデータをデータレイクやデータストア、分析ツールに配信するサービスであり、Amazon S3、Amazon Redshift、Amazon Elasticsearch Serrvice にロード
* Kinesis Data Analytics は、ストリーミングデータの分析

## AWS Lake Formation
* 安全なデータレイクを数日で簡単にセットアップできるサービス

## Amazon Managed Streaming for Apache Kafka (Amazon MSK)
* フルマネージドな Apache Kafka
* ストリーミングデータの取り込みと処理をリアルタイムで簡単に行う

## Amazon OpenSearch Service (Amazon Elasticsearch Service)
* ログ分析、リアルタイムのアプリケーションモニタリング、クリックストリーム分析などのユースケース向けの、完全なオープンソースの検索および分析エンジン

## Amazon QuickSight
* フルマネージド型の BI サービス
* RDS や Redshift などのデータベースサービス、S3、Athena、RDS、IAM、CloudTrail、Cloud Directory などと連携し、ダッシュボードで可視化

## Amazon Redshift
* データベースに記載