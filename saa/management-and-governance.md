- [マネジメント、ガバナンス](#マネジメントガバナンス)
  - [AWS Auto Scaling](#aws-auto-scaling)
  - [AWS CloudFormation](#aws-cloudformation)
  - [AWS CloudTrail](#aws-cloudtrail)
  - [Amazon CloudWatch](#amazon-cloudwatch)
  - [AWS Command Line Interface (AWS CLI)](#aws-command-line-interface-aws-cli)
  - [AWS Compute Optimizer](#aws-compute-optimizer)
  - [AWS Config](#aws-config)
  - [AWS Control Tower](#aws-control-tower)
  - [AWS License Manager](#aws-license-manager)
  - [Amazon Managed Grafana](#amazon-managed-grafana)
  - [Amazon Managed Service for Prometheus](#amazon-managed-service-for-prometheus)
  - [AWS Management Console](#aws-management-console)
  - [AWS Organizations](#aws-organizations)
  - [AWS Personal Health Dashboard](#aws-personal-health-dashboard)
  - [AWS Proton](#aws-proton)
  - [AWS Service Catalog](#aws-service-catalog)
  - [AWS Systems Manager](#aws-systems-manager)
  - [AWS Trusted Advisor](#aws-trusted-advisor)

# マネジメント、ガバナンス

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

## AWS CloudFormation
* AWS 内のすべてのインフラストラクチャリソースを自動でプロビジョニングできるサービス
* テンプレートに、JSON あるいは YAML フォーマットでプロビジョニングしたい AWS リソースを記述
* スタックは、AWS リソースの集合体
* スタックセットは、複数の AWS アカウントと複数のリージョンに対してスタックを作成できる機能
* 変更セットは、変更による影響度を確認するためのスタック
* ドリフトは、テンプレートによって展開した AWS リソースを展開後に変更した場合に、元テンプレートとの差分を検出するチェック機能
* サービス終了時にデータを保存するためには、S3 は DeletionPolicy 属性に Retain を設定し。RDS リソースに対しては、Snapshot を設定

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

## AWS Command Line Interface (AWS CLI)
* AWS のサービスを管理するための統合ツール
* ダウンロードおよび設定用の単一のツールのみを使用して、コマンドラインから AWS の複数のサービスを制御し、スクリプトを使用してこれらを自動化

## AWS Compute Optimizer
* ワークロードに最適な AWS リソースを推奨し、機械学習を使って過去の使用率メトリクスを分析することで、コストを削減し、パフォーマンスを向上

## AWS Config
* AWS のサービスで管理されているリソースの構成変更を追跡するサービス

## AWS Control Tower
* セキュアなマルチアカウント AWS 環境をセットアップおよび管理するための最も簡単な方法

## AWS License Manager
* Microsoft、SAP、Oracle、IBM といったベンダーが提供するライセンスの管理を、AWS とオンプレミス環境で簡単に行えるサービス

## Amazon Managed Grafana
* Grafana Labs と共同で開発したオープンソースの Grafana 向けのフルマネージドサービス

## Amazon Managed Service for Prometheus
* Prometheus との互換性を持つモニタリングおよびアラートサービス

## AWS Management Console
* AWS クラウドにアクセスして管理するウェブインターフェイス

## AWS Organizations
* 複数の AWS アカウント作成の自動化やグループ化による集中管理、グループにポリシーを適用したアクセス管理を実現するサービス
* サービスコントロールポリシー (SCP) によって複数の AWS アカウントに対して、IAM ポリシーのような権限制御を統合的に管理・適用

## AWS Personal Health Dashboard
* お客様の環境に影響を及ぼす可能性のある AWS イベントのアラートやガイダンス

## AWS Proton
* セルフサービスのインフラストラクチャテンプレートとプロビジョニングの自動化

## AWS Service Catalog
* AWS での使用が承認された IT サービスのカタログを作成および管理

## AWS Systems Manager
* AWS 内の様々なリソースの運用情報を統合定期に可視化、および制御するサービス
* AWS 内で利用する様々なパラメータを一元管理
* オートメーション機能や実行コマンド機能により、EC2 インスタンスなど様々な AWS リソースに対する運用タスクの制御を自動化

## AWS Trusted Advisor
* AWS のベストプラクティスに基づいて、「コスト最適化」「セキュリティ」「耐障害性」「パフォーマンス」「サービスの制限」の 5 項目で、ユーザーの AWS　利用状況をチェックし、改善すべき事項を推奨するサービス
