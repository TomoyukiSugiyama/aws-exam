# セキュリティ、アイデンティティ、コンプライアンス

* AWS Certificate Manager (ACM)
* AWS CloudHSM
* Amazon Cognito
* Amazon Detective
* AWS Directory Service
* AWS Firewall Manager
* Amazon GuardDuty
* AWS Identity and Access Management (IAM)
* Amazon Inspector
* AWS Key Management Service (AWS KMS)
* Amazon Macie
* AWS Network Firewall
* AWS Resource Access Manager (AWS RAM)
* AWS Secrets Manager
* AWS Security Hub
* AWS Shield
* AWS Single Sign-On
* AWS WAF

## AWS Certificate Manager (ACM)
* SSL/TLS 証明書の購入や登録、更新などの一元管理ができるサービス

## AWS CloudHSM

## Amazon Cognito

## Amazon Detective

## AWS Directory Service
* AWS のクラウド内で管理されるマネージド型の Microsoft AD
* Mictosoft AD、Simple AD、AD Connector の３つのディレクトリタイプを提供
* Microsoft AD は、AWS 上で AD サービスを利用可
* Simple AD は、AWS 上で AD 互換の Samba サービスを利用可
* AD Connector は、既存の AD 環境へ接続するためのプロキシサービス

## AWS Firewall Manager

## Amazon GuardDuty
* CloudTrail、VPC フローログ、Amazon Route 53 のクエリログといった各種ログを監視し、悪意のある第 3 者による攻撃や不正操作などのセキュリティ脅威を検知するサービス
* 機械学習により不正な動作の学習、異常検知

## AWS Identity and Access Management (IAM)
* AWS へのアクセスを安全に制御するための仕組み
* AWS アカウントの登録
* IAM ポリシーによる権限の付与
* AWS マネジメントコンソールへのログイン、AWS CLI でのコマンド操作、AWS SDK でプログラムから API を利用する際に利用される
* 最小権限の原則に従い、ネットワークセキュリティ、データの保護、セキュリティの監視を行う

## Amazon Inspector
* EC2 インスタンスのセキュリティを高めるサービス
* EC2 インスタンスに Inspector のエージェントをインストールすることで、EC2 インスタンス上のアプリケーションの脆弱性などを診断

## AWS Key Management Service (AWS KMS)
* AWS 上で鍵管理を提供するマネージドサービス
* 暗号化鍵 (CMK) の作成・無効の管理、ローテーション、削除などを行うことが可能
* 鍵は AWS 上に保存
* S3 上のファイルのサーバーサイドでの暗号化 (SSE) や、データ送信前にクライアントサイドでの暗号化 (CSE) が可能
* AWS SDK や CLI を利用したクライアントアプリケーションと連携
* S3、EBS、RDS、Redshift などのストレージやデータベースサービスと連携

## Amazon Macie
* 機械学習とパターンマッチングを使用して AWS の機密データを検出して保護する、フルマネージドのデータセキュリティとデータプライバシーのサービス

## AWS Network Firewall

## AWS Resource Access Manager (AWS RAM)
* AWS Organizations 組織内で、サブネットや AWS Transit Gateway のリソースを共有するサービス

## AWS Secrets Manager
* RDS や Redshift などのデータベースの認証情報を暗号化して集中管理・保管するサービス
* アプリケーションから Secret Manager の API を実行することで、保管されているデータベースの認証情報をセキュアに取得
* データベースの認証情報を自動的に更新
* AWS KMS などと連携し、認証情報を暗号化する際にカギの管理を KMS で行うことが可能

## AWS Security Hub

## AWS Shield
* DoS (Denial of Services) や DDoS (Distributed Denial of Services) に代表される一斉攻撃に対する防御

## AWS Single Sign-On
* AWS 上でワークフォースアイデンティティを作成、または接続し、AWS 組織全体のアクセスを一元管理
* AWS SSO からだけでなく、Microsoft アクティブディレクトリや、Okta Universal Directory や Azure AD などの標準ベースの ID プロバイダーから利用可

## AWS WAF
* SQL インジェクションやクロスサイトスプリクティングのような攻撃から保護
* 送信元の IP アドレスに基づくアクセス制限
* HTTP プロトコル情報に対してフィルタリングを設定し、特定の攻撃パターンから防御
* CloudFront や ELB にアタッチし、各サービスへのアクセスを制限
* Refer 制限により、直接に URL リンクを参照することを制限