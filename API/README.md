# API

## 目次  

<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. 変更ポイント](#1-変更ポイント)
- [2. 新リージョンでの実行例](#2-新リージョンでの実行例)

<!-- /TOC -->


---

### 1. 変更ポイント  

旧リージョンの[「API実行サンプル」](https://doc.cloud.global.fujitsu.com/jp/iaas/api-sample.html)を元に、変更箇所を抽出しています。  

| 変更箇所                                 | 変更ポイント                                                                                                                     |
|:-----------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------|
| AZ                                       | 新リージョンはシングルAZ構成のため「AZ」の概念がありません。そのためAPIに含まれる「availability_zone」系のパラメータは不要です。 |
| [APIバージョン](knowledge/APIVersion.md) | API発行時のpathに含まれるバージョンが変更されています。                                                                          |
| [APIのpath](knowledge/APIPath.md)        | pathが変更されているAPIがあります。                                                                                              |

新リージョンのAPI仕様については、[「IaaS API リファレンス」](https://doc.cloud.global.fujitsu.com/lib/iaas/jp/api-reference/v3/web/k5-iaas-api-reference/index.html)をご覧ください。  


---

### 2. 新リージョンでの実行例

- [プロジェクトIDの取得方法](knowledge/getProjectID.md)  
- [APIエンドポイントの取得方法](knowledge/getAPIendpoint.md)  
- [リモートコンソールでのアクセス方法](knowledge/connectRemoteConsole.md)  


------
