# セキュリティ、アイデンティティ、コンプライアンス

* AWS Certificate Manager (ACM)
* AWS Directory Service
* Amazon GuardDuty
* AWS Identity and Access Management (IAM)
* Amazon Inspector
* AWS Key Management Service (AWS KMS)
* Amazon Macie
* AWS Secrets Manager
* AWS Shield
* AWS Single Sign-On
* AWS WAF

## AWS Certificate Manager (ACM)
* SSL/TLS 証明書の購入や登録、更新などの一元管理ができるサービス

## AWS Directory Service
* AWS のクラウド内で管理されるマネージド型の Microsoft AD
* Mictosoft AD、Simple AD、AD Connector の３つのディレクトリタイプを提供
* Microsoft AD は、AWS 上で AD サービスを利用可
* Simple AD は、AWS 上で AD 互換の Samba サービスを利用可
* AD Connector は、既存の AD 環境へ接続するためのプロキシサービス

## Amazon GuardDuty
* CloudTrail、VPC フローログ、Amazon Route 53 のクエリログといった各種ログを監視し、悪意のある第 3 者による攻撃や不正操作などのセキュリティ脅威を検知するサービス
* 機械学習により不正な動作の学習、異常検知

## AWS Identify and Access Management (IAM)
* AWS へのアクセスを安全に制御するための仕組み
* AWS アカウントの登録
* IAM ポリシーによる権限の付与
* AWS マネジメントコンソールへのログイン、AWS CLI でのコマンド操作、AWS SDK でプログラムから API を利用する際に利用される
* 最小権限の原則に従い、ネットワークセキュリティ、データの保護、セキュリティの監視を行う

