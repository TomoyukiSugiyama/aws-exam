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

## AWS Snowball
* AWS から物理搬送される耐久性の高い筐体に 80 TB までのデータを保管し、AWS 内のストレージへ転送するサービス
* Snowball 内のデータは自動的に暗号化
* 拡張版として AWS Snowball Edge があり、100 TB のストレージ、より多くのネットワークインターフェイスをサポート
