# アプリケーション統合

* Amazon AppFlow
* AWS AppSync
* Amazon EventBridge (Amazon CloudWatch Events)
* Amazon MQ
* Amazon Simple Notification Service (Amazon SNS)
* Amazon Simple Queue Service (Amazon SQS)
* AWS Step Functions
* (試験ガイド外) Amazon Simple Email Service (Amazon SES)

## Amazon AppFlow
* Salesforce、SAP、Zendesk、Slack、および ServiceNow などの SaaS アプリケーションと、Amazon S3 や Amazon Redshift などの AWS のサービスとの間で、たった数回のクリックでデータを安全に転送できるフルマネージド統合サービス

## AWS AppSync
* サーバレスに記載

## Amazon EventBridge (Amazon CloudWatch Events)
* AWS の各種サービスや各種サービスや外部の SaaS などの様々なイベントリソースで発生するイベントを、あらかじめ設定したルールに基づいて、他サービスなどの様々なターゲットにリアルタイムに連携できるサービス

## Amazon MQ
* 業界標準 API やプロトコルを利用して、クラウド内のメッセージブローカーを利用できる Apache ActiveMQ 向けのマネージド型メッセージブローカーサービス

## Amazon Simple Notification Service (Amazon SNS)
* メッセージ通知サービス
* トピック、購読者 (サブスクライバ) 、メッセージの発行 (パブリッシュ) からなる
* トピックは、メッセージを送信、通知を受信するためのアクセスポイント
* 購読者 (サブスクライバ) は、 トピックから発信されるメッセージの購読者
* メッセージの発行 (パブリッシュ) は、トピックに対して。アプリケーションなどからメッセージを発行

## Amazon Simple Queue Service (Amazon SQS)
* メッセージキュー
* 複数のインスタンスへ非同期で分散
* キューのタイプは標準キューと FIFO キューに分類
* 標準キューは、メッセージの 1 つ以上のコピーが順序通りに配信できない場合がある
* 標準キューは、メッセージが少なくとも 1 回配信される方式であり、キューには重複が発生する可能性がある
* 標準キューは、1 秒あたりのトランザクション数はほぼ無制限
* FIFO キューは、配信順番を守る
* FIFO キューは、メッセージが 1 回だけ配信され、コンシューマがプロセスを処理して削除するまで使用可能なキューの状態を保つため、キューの重複がない
* FIFO キューは、1 秒あたり 300 トランザクションに限定

## AWS Step Functions
* デベロッパーが分散アプリケーションの構築、IT およびビジネスプロセスの自動化、AWS のサービスを利用したデータと機械学習のパイプラインの構築に使用するローコードのビジュアルワークフローサービス

## (試験ガイド外) Amazon Simple Email Service (Amazon SES)
* E メールの送受信機能を提供するサービス
* アプリケーション上の E メール通知機能を実装
