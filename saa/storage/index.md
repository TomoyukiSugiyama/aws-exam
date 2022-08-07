# ストレージ

* Amazon Elastic Block Store (Amazon EBS)
* Amazon Elastic File System (Amazon EFS)
* Amazon FSx
* Amazon S3
* Amazon S3 Glacier
* AWS Storage Gateway

## Amazon Elastic Block Store (Amazon EBS)
* 永続可能なブロックストレージサービス
* AZ 内で自動的に複製される仕組み有り
* 複数のボリュームタイプに分類
* 汎用 SSD (General Purpose SSD : gp2) は、デフォルトで提供されるボリュームタイプで、SSD を安価で利用でき、確保した要領に応じた IOPS が設定される
* プロビジョンド IOPS SSD (PIOPS SSD : io1 および io2) は、高パフォーマンスを実現でき、自由に IOPS を設定可能
* スループット最適化 HHD (st1) は、HDD タイプで、大容量のストレージを安価に利用可
* コールド HDD (sc1) は、アクセス頻度の低い大量データの保存に適した HDD
* マグネティックは、旧世代のボリュームタイプで、アクセス頻度の低い用途に適した旧世代 HDD
* スナップショットを用いてバックアップを取得可能
* スナップショットは自動的に S3 へ保管
* スナップショットは、初回はフルバックアップを行うが、以後は増分で取得

## Amazon Elastic File System (Amazon EFS)
* スケーラブルな共有ストレージサービス
* 複数の AZ に冗長化してデータを保管
* マネージド型のサービスで、ストレージ容量やパフォーマンスを自動的にスケーリング
* 標準的なファイルシステムである NFS によってアクセス
* オンプレミスサーバーからも利用可

## Amazon FSx
* コスト効率の良いファイルシステムを提供するサービス
* マルチ AZ に対応し高い可用性を持つ
* S3 へのバックアップも可能であり高い耐久性を持つ
* データ保存用ストレージは HDD や SSD に対応
* データや通信中のデータは全て暗号化
* IAM ポリシーによる API コールのアクセス制御や、セキュリティグループを使ったアクセス制御が可能
* FSx for Windows、FSx for Lustre に分類
* FSx for Windows は、SMB プロトコルを利用して、データへのアクセスが可能なファイルシステム
* FSx for Lustre は、機械学習や HPC (High Performance Computing) など、処理速度を重視するシステムに利用される Linux ベースのファイルシステム

