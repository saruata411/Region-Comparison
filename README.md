# 本サイトについて

FUJITSU Cloud Service for OSS IaaS (旧FUJITSU Clould Service K5 IaaS) の2018年6月以降開設のリージョン(以降、新リージョン)について、それ以前のリージョン(以降、旧リージョン)との**差異のポイント**を解説します。

------



# 対象者

旧リージョンをご利用、またはIaaSに関する基本的な知識をお持ちの方。

------



# 新リージョン

| リージョン名       | 開設時期  |
| ------------------ | --------- |
| 西日本リージョン３ | 2018年6月 |
| 東日本リージョン３ | 2018年7月 |

------



# Index

1. [AZ (Availability Zone)](AZ/README.md)
2. [サーバ機能](serverfunction/README.md)
3. [ストレージ機能](storagefunction/README.md)
4. [ネットワーク機能](networkdesign/README.md)
5. データベース機能(新リージョンでは2018年7月末より提供予定)
6. [CDP (Cloud Design Patterns)](CDP/README.md)
7. [ユーザーポータル](userportal/README.md)
8. [API](API/README.md)
9. [Heatテンプレート](HeatTemplate/README.md)
10. [認証／規格](audit/README.md)
11. [FAQ](FAQ/README.md)

------



# 公開ドキュメント

| 概要                                    | 格納先                                                       |
| --------------------------------------- | ------------------------------------------------------------ |
| FUJITSU Cloud Serviceの公開ドキュメント | [FUJITSU Cloud Service]( https://k5-doc.jp-east-1.paas.cloud.global.fujitsu.com/doc/jp/iaas/document/list/doclist_iaas.html ) |

------



# 略称

| 略称         | 英語名称                 | 日本語名称                   |
| ------------ | ------------------------ | ---------------------------- |
| AZ           | Availability Zone        | アベイラビリティゾーン       |
| CDP          | Cloud Design Patterns    | クラウドデザインパターン     |
| VM           | Virtual Machine          | 仮想サーバ                   |
| IPCOM VA(*1) | IPCOM Virtual Appliance  | IPCOM 仮想アプライアンス     |
| LB           | Load Balancer            | ロードバランサー             |
| FW           | Firewall                 | ファイアーウォール           |
| SLA          | Service Level Agreement  | サービスレベルアグリーメント |
| BCP          | Business Continuity Plan | 事業継続計画                 |
| DRP          | Disaster Recovery Plan   | 災害復旧計画                 |

(*1)IPCOMは富士通のネットワークアプライアンス製品名です。IPCOM VAはIPCOMがイメージとして提供され仮想インスタンスとして利用できます。

------



# 商標

- Microsoft、Windows、Windows Serverまたはその他のマイクロ ソフト製品の名称および製品名は、米国Microsoft Corporationの、米国およびその他の国における登録商標または商標です。
- Linuxは米国及びその他の国におけるLinus Torvaldsの登録商標です。
- Red Hat、Red Hat Enterprise Linux、OpenShiftは米国およびその他の国において登録されたRed Hat, Inc.の商標です。
- Ubuntuは、Canonical Ltd.の登録商標です。
- OpenStackのワードマークは、米国とその他の国におけるOpenStack Foundationの登録商標/サービスマークまたは商標/サービスマークのいずれかであり、OpenStack Foundationの許諾の下に使用されています。
- SAP及びSAPロゴ、SAP R/3、mySAP.com、mySAP Business Suite、その他のSAP製品は、ドイツ及びその他の国におけるSAP AGの商標または登録商標です。
- そのほか、本書に記載されている会社名および製品名は、それぞれ各社の商標または登録商標です。



尚、本書では、システム名または製品名に付記される登録表示（™または®）は、省略しています。 