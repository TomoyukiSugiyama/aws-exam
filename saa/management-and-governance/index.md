# マネジメント、ガバナンス

* AWS Auto Scaling
* AWS Backup
* AWS CloudFormation
* AWS CloudTrail
* Amazon CloudWatch
* AWS Config
* Amazon EventBridge (Amazon CloudWatch Events)
* AWS Organizations
* AWS Resource Access Manager
* AWS Systems Manager
* AWS Trusted Advisor

## AWS Auto Scaling
* 自動でスケールアウト、スケールインするサービス
* EC2 Auto Scaling、Application Auto Scaling、AWS Auto Scaling に分類
* EC2 Auto Scaling は、EC2 が対象
* Application Auto Scaling は、ECS サービス、EMR サービス、Aurora レプリカなどが対象
* AWS Auto Scaling は、自動スケーリングと予測スケーリングの機能を持つ
* 予測スケーリングでは、CPU の使用率などを分析し、その結果に基づいて今後の利用量を予測し適切なシステム利用状況になるように管理

## AWS Backup
* AWS 内におけるデータのバックアップを一元化・自動化するサービス
* バックアップポリシーに基づいて、EBS ボリューム、EC2 インスタンス、RDS データベースなどのバックアップの定期実行、バックアップ状況を監視

## AWS CloudFormation
* AWS 内のすべてのインフラストラクチャリソースを自動でプロビジョニングできるサービス
* テンプレートに、JSON あるいは YAML フォーマットでプロビジョニングしたい AWS リソースを記述
* スタックは、AWS リソースの集合体

## AWS CloudTrail
* AWS アカウントで利用された操作 (API コール) をログとして記録するサービス
* AWS アカウントを取得した時点で有効かされ、過去 90 日間のサービスに対する操作を表示
* 取得されたログはデフォルトで S3 に保存され、 CloudWatch Logs への連携も可能
* 記録内容は、サービスの API コールもと、時間、送信元 IP アドレス、呼び出した API、対象リソース

## Amazon CloudWatch
* AWS 上で稼働する様々なシステムや AWS のリソースの情報を収集・監視・可視化するサービス
* メトリクスを収集監視し、ある一定以上の使用率になった場合に通知 (アラート)
* メトリクスを時系列でグラフ化
* CPU 使用率などの標準メトリクスと独自のメトリクスを定義したカスタムメトリクスに分類
* 基本メトリクスは、最大 15 ヶ月分保存し、5 分間隔で無料で利用
* 詳細モニタリングは、最大 15 ヶ月分保存し、1 分感覚で追加料金が必要

## AWS Config
* AWS のサービスで管理されているリソースの構成変更を追跡するサービス

## Amazon EventBridge (Amazon CloudWatch Events)
* AWS の各種サービスや各種サービスや外部の SaaS などの様々なイベントリソースで発生するイベントを、あらかじめ設定したルールに基づいて、他サービスなどの様々なターゲットにリアルタイムに連携できるサービス

# AWS Organizations
* 複数の AWS アカウント作成の自動化やグループ化による集中管理、グループにポリシーを適用したアクセス管理を実現するサービス
* サービスコントロールポリシー (SCP) によって複数の AWS アカウントに対して、IAM ポリシーのような権限制御を統合的に管理・適用

