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
* Site to Site PVN
* Virtual Private Gateway (VGW)
* VPC ピアリング
* VPC エンドポイント (ゲートウェイ型, インターフェイス型)
* Auto Scaling
* VPC フローログ
* Elastic IP (EIP)

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
* インスタンスに適用するファイアウォール機能
* アウトバウンドとインバウンドを設定
* アウトバウンドは、インスタンスから出る通信を制御
* インバウンドは、インスタンスへの通信を制御
* デフォルトでアウトバウンド通信は全て許可、インバウンド通信は全て拒否
* 1 つのインスタンスに複数設定可
* 設定追加、変更は即時に反映
* **ステートフル**な通信が可能

