## データベース

* Amazon Aurora
* Amazon Aurora Serverless
* Amazon DocumentDB (with MongoDB compatibility)
* Amazon DynamoDB
* Amazon ElastiCache
* Amazon Keyspaces (for Apache Cassandra)
* Amazon Neptune
* Amazon Quantum Ledger Database (Amazon QLDB)
* Amazon RDS
* Amazon Redshift
* Amazon Timestream

## Amazon Aurora
* AWS が開発した完全マネージ型のリレーショナルデータベースサービス
* PostgreSQL、MySQL と互換性有り
* マルチ AZ に分散されたクラスター構成により、標準的な MySQL データベースと比べて最大で 5 倍、標準的な PostgreSQL データベースと比べて最大で 3 倍高速
* 商用データベースと同等のセキュリティ、可用性、信頼性を、10 分の 1 のコストで実現
* SQL 処理を行うデータベースインスタンス
* データを格納するストレージ部分であるクラスターボリューム
* ３つの AZ に存在し、うちひとつのデータベースインスタンスはプライマリデータベースインスタンス
* その他の2つは、Aurora レプリカ
* １つの AZ につき２箇所のディスクに書き込まれる
* 曜日や時間帯を指定し自動でバッチ適用
* １日１回自動バックアップし、最大35日分を保存
* スナップショットからデータベースインスタンスを復元
* バックアップのデータベースとトランザクションログが残っている範囲内の特定の日時時点のデータを復元
* DB クラスタが設置されているリージョンとは異なるリージョンにリードレプリカを複数作成することで、障害発生時には他のリージョンで操作を継続可能

## Amazon Aurora Serverless
* Amazon Aurora のオンデマンドの Auto Scaling 設定

## Amazon DocumentDB (with MongoDB compatibility)
* ミッションクリティカルなMongoDB のワークロードを運用するための、スケーラブルかつ高い耐久性の、フルマネージドデータベースサービス

## Amazon DynamoDB
* マネージド型の NoSQL データベースサービス
* キーバリュー型のデータベース
* データは自動的にマルチ AZ に保存
* 結果生合成モデルがあり、書き込んだデータは時間が経てば正しく反映される
* 正しいデータが取得できないことに対して対策案として、Consistent Read (読み取り一貫性) というオプションを提供
* DynamoDB グローバルテーブルは、複数リージョンに配置しているデータベーステーブルでデータの整合性を取るフルマネージド型のソリューション
* DynamoDB ストリームは、DynamoDB のデーブルに対して行われたデータ変更の履歴情報をイベントとして検出し、24 時間保持
* DynamoDB の料金は、オンデマンド、プロビジョニング済みの２つのキャパシティモードで分類
* オンデマンドの料金は、パフォーマンスの予測や設定は不要で、実行したデータの読み書きに対して発生
* プロビジョニング済みの料金は、１秒当たりの読み書きの回数を予測し指定、Auto Scaling を利用しテーブルのキャパシティを自動的に調整可能
* DynamoDB Auto Scaling は、テーブツとインデックスを監視して、アプリケーショントラフィックの変化に応じて自動的にスループットを調整
* DynamoDB Accelerator (DAX) を有効化することで、DynamoDB テーブルはミリセカンドからマイクロセカンドへの最大 10 倍のパフォーマンス向上を実現
* Auto Scaling を設定することで、一時的な負荷に対して処理性能をスケーリングし、高負荷に対応

## Amazon ElastiCache
* マネージド型のインメモリデータベース
* ElastiCache Redis は、シングルスレッドで動作し全ての操作は排他的であり、データの永続化、スナップショット機能、pub/sub 機能を持つ
* ElastiCache Memcached は、マルチスレッドで動作し、データの永続化やスナップショットは無く、フェイルオーバーや復元もできない

## Amazon Keyspaces (for Apache Cassandra)
* スケーラブルで可用性の高い、Apache Cassandra 互換のマネージドデータベースサービス

## Amazon Neptune
* 高速で信頼性が高いフルマネージド型のグラフデータベースサービス

## Amazon Quantum Ledger Database (Amazon QLDB)

## Amazon RDS
* マネージド型のリレーショナルデータベースサービス
* Amazon Aurora、PostgreSQL、MySQL、MariaDB、Oracle Database、Microsoft SQL Server をサポート
* リードレプリカを配置することで、低コストで読取リクエストに対応可
* オートスケーリングを有効化することで、ストレージ容量を増加
* RDS プロキシを利用することで、アプリケーションと RDB データベースの間の仲介役として機能し、必要なコネクションをプーリングすることで、既存のコネクションを再利用しコネクションを効率的に実行

## Amazon Redshift
* ペタバイドクラスのデータも扱うことができるマネージド型のデータウェアハウスサービス
* ノードと呼ばれるコンピューティングリソースの集まりで構成
* リーダーノードが処理を受け付け
* リーダノードは、コンピュータノードに対して処理を依頼
* スナップショットによってバックアップ
* 自動スナップショットを有効にすると、8 時間ごとに自動でスナップショットを作成
* クロスリージョンスナップショットは、別のリージョンにもコピーするように設定可能
* スナップショット用に無料ストレージはあるが、上限の容量を超過すると課金が発生
* WLM (Work Load Manager) は、 Redshift のクエリ処理に対して割り当てる Redshift のリソースを指定する機能
* 拡張 VPC ルーティングにより、Redshift 間のすべてのトラフィックがインターネットを通過しないように設定

## Amazon Timestream
