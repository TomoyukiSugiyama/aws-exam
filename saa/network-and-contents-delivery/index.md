# ネットワーク、コンテンツ配信

* Amazon API Gateway
* Amazon CloudFront
* AWS Direct Connect
* AWS Global Accelerator
* Amazon Route 53
* AWS Transit Gateway
* Amazon Virtual Private Cloud (Amazon VPC)
* サブネット
* Internet Gateway (IGW)
* ルートテーブル
* NAT ゲートウェイ
* セキュリティグループ
* ネットワーク ACL
* Site to Site VPN
* Virtual Private Gateway (VGW)
* VPC ピアリング
* VPC エンドポイント
* Auto Scaling
* VPC フローログ
* Elastic IP (EIP)

## AWS Direct Connect
オンプレミス環境と AWS 間を専用線で接続

## AWS Transit Gateway
VPC 内のハブの機能を持ったゲートウェイ

## Amazon Virtual Private Cloud (Amazon VPC)
論理的に分割された、特定のユーザーだけが利用できるプライベートネットワーク

## サブネット
* VPC 内に構成するネットワークセグメント
* 1 つの VPC に対して複数作成可
* VPC の IP アドレスの範囲内で CIDR を指定
* パブリックサブネットとプライベートサブネットに分類
* パブリックサブネットは、インターネットとの通信が可能

## Internet Gateway (IGW)
インターネットへアクセスするためのゲートウェイ

## ルートテーブル
静的ルーティングを指定したもの

## NAT ゲートウェイ
プライベートサブネットからインターネットへ接続するための NAT 機能

## セキュリティグループ
* インスタンス単位のファイアウォール機能
* アウトバウンドとインバウンドを設定
* アウトバウンドは、インスタンスから出る通信を制御
* インバウンドは、インスタンスへの通信を制御
* デフォルトでアウトバウンド通信は全て許可、インバウンド通信は全て拒否
* 1 つのインスタンスに複数設定可
* 設定追加、変更は即時に反映
* **ステートフル**な通信が可能

## ネットワーク ACL
* サブネット単位のファイアウォール機能
* アウトバウンド通信、インバウンド通信は全て許可
* ルールに番号を割り当て、番号順に許可または拒否のルールを適用
* **ステートレス**な通信

## Site to Site VPN
* インターネットを経由して、オンプレミス環境と AWS 間を接続
* 低コスト、短期間で導入可能

## Virtual Private Gateway (VGW)
* オンプレミス環境と AWS を接続する際のゲートウェイ
* Direct Connect 接続、Site to Site VPN で利用

## VPC ピアリング
VPC 間をプライベート接続

## VPC エンドポイント
* プライベートネットワークから AWS サービスへアクセスするためのエンドポイント
* ゲートウェイ型とインターフェイス型に分類
* ゲートウェイ型は、ルートテーブルに指定されたターゲットを追加
* インターフェイス型は、「AWS Private Link」とも呼ばれ、インターネットを経由せずプライベート接続
