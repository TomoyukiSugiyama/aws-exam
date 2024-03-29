- [AWS の請求情報とコスト管理](#aws-の請求情報とコスト管理)
  - [AWS Badgets](#aws-badgets)
  - [AWS Cost and Usage Report](#aws-cost-and-usage-report)
  - [Cost Explorer](#cost-explorer)
  - [Savings Plans](#savings-plans)

# AWS の請求情報とコスト管理

## AWS Badgets
* 予算の作成が可能
* あらかじめ予算額やリソース使用量を設定し、どれだけ消費しているか確認可能
* 予算額を超過しそうな場合、超過した場合に CloudWatch アラームや SNS トピック、メールなどで通知

## AWS Cost and Usage Report
* AWS のコストと使用状況データをより詳しく見る

## Cost Explorer
* AWS Cost and Usage Report のデータをグラフィカルに可視化
* 可視化、分析、予測の ３ つの機能を提供
* サービスごと、アカウントごとの月次コスト、日次コスト、月次の EC2 使用時間、コスト、リザーブドインスタンスのコスト、オンデマンドインスタンスを利用した場合のコスト削減額など
* サービス、AWS アカウント、リージョン、アベイラビリティゾーン、インスタンスタイプ、タグなどの条件でフィルタリンクして表示、カスタムレポートの作成が可能
* 過去の使用量のトレンドから今後 3 ヶ月間のコストを予測可能

## Savings Plans
* 1 年または 3 年の期間で特定の使用量 (USD/時間で測定) を契約するかわりに、オンデマンド料金と比較して低料金を実現する柔軟な料金モデル
