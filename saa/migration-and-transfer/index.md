# 移行、転送

* AWS Database Migration Service (AWS DMS)
* AWS DataSync
* AWS Migration Hub
* AWS Server Migration Service (SMS)
* AWS Snowball
* AWS Transfer Family

## AWS Database Migration Service (AWS DMS)
* データベースを AWS に移行するサービス
* 移行中でも、ソースデータベースは完全に利用可能
* 異なるデータベースプラットフォーム間の移行をサポート

## AWS DataSync
* オンプレミス環境のストレージと AWS のストレージサービス間でデータ転送を高速に行うサービス
* エージェントを導入することで利用可
* 転送先は、 S3、EFS、FSx for Windows など

## AWS Migrartion Hub
* AWS での移行とモダナザイゼーションの準備を支援
* 既存のアプリケーション、インフラストラクチャ、およびそれらの依存関係とモダナザイゼーションの能力を評価
* サーバーや移行中のデータベースのステータスなど、追跡する必要のある多くのコンポーネントを一元管理
* AWS が移行した類似パターンの数千のアプリケーションを基にした実証済みの定義済みワークフローテンプレートを使用して、移行を高速化
* アプリケーションのリファクタリング、開発と運用の簡素化、既存のアプリケーションとマイクロサービスを単一のアプリケーションとして管理することを支援

## AWS Server Migration Service (SMS)
* SMS は、サービス終了しており、AWS Application Migration Service (AWS MGN) に移行を推奨
* AWS MGN は、ソースサーバーを物理インフラストラクチャ、仮想インフラストラクチャ、およびクラウドインフラストラクチャから AWS でネイティブに実行するように自動的に変換

## AWS Snowball
* AWS から物理搬送される耐久性の高い筐体に 80 TB までのデータを保管し、AWS 内のストレージへ転送するサービス
* Snowball 内のデータは自動的に暗号化
* 拡張版として AWS Snowball Edge があり、100 TB のストレージ、より多くのネットワークインターフェイスをサポート
