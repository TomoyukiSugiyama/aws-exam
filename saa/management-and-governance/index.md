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

