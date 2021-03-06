# IaaSポータル機能一覧表

## 目次  

<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. 変更ポイント](#1-変更ポイント)

<!-- /TOC -->


---

### 1. 変更ポイント  

ユーザーポータルの新リージョン対応状況です。
- [✓]：提供  
- [N/A]：今後提供予定  
- [×]：提供なし  

| 区分                     | 機能                       | 提供 | 備考                                                                    |
|:-------------------------|:---------------------------|:----:|:------------------------------------------------------------------------|
| コンピュート             | 仮想サーバ                 |  ✓   | －                                                                      |
|                          | キーペア                   |  ✓   | －                                                                      |
|                          | イメージ                   |  ✓   | －                                                                      |
|                          | スケジュール               |  ✓   | 「分」は指定できません、「00分」に実行されます。                        |
| ストレージ               | ブロックストレージ         |  ✓   | －                                                                      |
|                          | オブジェクトストレージ     |  ✓   | －                                                                      |
|                          | スナップショット           |  ✓   | －                                                                      |
|                          | 共有ディスク               |  ✓   | ベアメタル用：東日本リージョン3のみで利用可能です。                     |
| ネットワーク             | 仮想ネットワーク           |  ✓   | －                                                                      |
|                          | 仮想ルータ                 |  ✓   | －                                                                      |
|                          | セキュリティグループ       |  ✓   | －                                                                      |
|                          | グローバルIP               |  ✓   | －                                                                      |
|                          | ファイアーウォール         |  ✓   | 現在制限あり (\*1) (\*2)：制限に該当する機能は、APIを利用してください。 |
|                          | DNS                        |  ×   | －                                                                      |
|                          | ロードバランサー           |  ✓   | 編集はAPIを利用してください。                                           |
|                          | VPNサービス</br>(SSL-VPN)  |  ✓   | －                                                                      |
|                          | VPNサービス</br>(IPSecVPN) |  ✓   | －                                                                      |
| データベース             | データベース仮想サーバ     | N/A  | －                                                                      |
| テンプレート             | スタック                   |  ✓   | －                                                                      |
| 監視                     | モニタリング               |  ✓   | －                                                                      |
|                          | アラーム                   |  ✓   | －                                                                      |
| インポート・エクスポート | VMインポート               |  ✓   | 現在制限あり (\*2) ：Windows ServerのOSイメージは80GBまでとなります。   |
|                          | VMエクスポート             |  ✓   | －                                                                      |
| API実行                  | API実行                    |  ✓   | －                                                                      |
| ログ                     | 操作ログ                   |  ✓   | －                                                                      |


(\*1)：[「ファイアーウォールサービスの制限事項」](https://doc.cloud.global.fujitsu.com/lib/iaas/jp/restriction/v3/firewall_limitation.pdf)をご覧ください。  
(\*2)：[「IaaS 制限事項・注意事項」](https://doc.cloud.global.fujitsu.com/lib/iaas/jp/restriction/v3/k5-limitation2.pdf)をご覧ください。  
