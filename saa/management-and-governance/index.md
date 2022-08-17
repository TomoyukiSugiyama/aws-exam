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
* 閾値を超えたにもかかわらずインスタンスの起動に繰り返し失敗すると、スケーリングがうまく実行されず 24 時間以上たっだ場合は、自動的に Auto Scaling が停止
* インスタンスの状態が Impaired となると数分間リカバリーされるかチェック
* リカバリーされない場合は新しいインスタンスを起動して、Impaired のインスタンスを終了
* Auto Scaling グループを一時的に停止しないでインスタンスを停止すると新規インスタンスが起動

## AWS Backup
* AWS 内におけるデータのバックアップを一元化・自動化するサービス
* バックアップポリシーに基づいて、EBS ボリューム、EC2 インスタンス、RDS データベースなどのバックアップの定期実行、バックアップ状況を監視

## AWS CloudFormation
* AWS 内のすべてのインフラストラクチャリソースを自動でプロビジョニングできるサービス
* テンプレートに、JSON あるいは YAML フォーマットでプロビジョニングしたい AWS リソースを記述
* スタックは、AWS リソースの集合体
* スタックセットは、複数の AWS アカウントと複数のリージョンに対してスタックを作成できる機能
* 変更セットは、変更による影響度を確認するためのスタック
* ドリフトは、テンプレートによって展開した AWS リソースを展開後に変更した場合に、元テンプレートとの差分を検出するチェック機能

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

## AWS Resource Access Manager
* AWS Organizations 組織内で、サブネットや AWS Transit Gateway のリソースを共有するサービス

## AWS Systems Manager
* AWS 内の様々なリソースの運用情報を統合定期に可視化、および制御するサービス
* AWS 内で利用する様々なパラメータを一元管理
* オートメーション機能や実行コマンド機能により、EC2 インスタンスなど様々な AWS リソースに対する運用タスクの制御を自動化

## AWS Trusted Advisor
* AWS のベストプラクティスに基づいて、「コスト最適化」「セキュリティ」「耐障害性」「パフォーマンス」「サービスの制限」の 5 項目で、ユーザーの AWS　利用状況をチェックし、改善すべき事項を推奨するサービス
