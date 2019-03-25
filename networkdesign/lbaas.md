# ロードバランサー

## 目次  

<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. 変更ポイント](#1-変更ポイント)

<!-- /TOC -->


---

### 1. 変更ポイント  

| 項目                             | 旧リージョン                       | 新リージョン                   |
|:---------------------------------|:-----------------------------------|:-------------------------------|
| 提供インスタンス                 | 富士通独自開発                     | OpenStack標準                  |
| グレード                         | ３タイプ（Standard、Middle、High） | １タイプ（Standard）           |
| アクセス方式                     | FQDN                               | 仮想IPアドレス                 |
| Sorryページリダイレクト          | 機能あり                           | 機能なし                       |
| 通信制御（セキュリティグループ） | セキュリティグループ制御対象       | セキュリティグループ制御対象外 |
| 冗長化                           | 多重化＋DNSラウンドロビン          | アクティブ・スタンバイ         |

新リージョンのロードバランサー仕様については、[「IaaS機能説明書 → ロードバランサーサービス（lbaas）」](https://doc.cloud.global.fujitsu.com/lib/iaas/jp/function-manual/index.html#intro/intro_elb_lbaas_v3.html)をご覧ください。  


---
