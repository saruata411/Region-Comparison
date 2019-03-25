# Heatテンプレート

## 目次  

<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. 変更ポイント](#1-変更ポイント)

<!-- /TOC -->


---

### 1. 変更ポイント  

| 項目             | 注意点                                                                                 |
|:-----------------|:---------------------------------------------------------------------------------------|
| AZ数             | 新リージョンはシングルAZ構成のため、マルチリージョン用のテンプレートは利用できません。 |
| 仮想サーバタイプ | 新旧リージョンで仮想サーバタイプ（フレーバー）が異なるため、修正してください。         |

新リージョンのテンプレート仕様については、[「IaaS機能説明書 → スタックの構築（東日本リージョン3／西日本リージョン3）」](https://doc.cloud.global.fujitsu.com/lib/iaas/jp/function-manual/index.html#concept/concept_orchestration_stackdeployment_v3.html)をご覧ください。  


---
