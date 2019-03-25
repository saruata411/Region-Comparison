# IaaS構築ガイド・クラウドデザインパターン(CDP)  

## 目次  

<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. IaaS初期構築ガイド](#1-iaas初期構築ガイド)
- [2. クラウドデザインパターン(CDP)](#2-クラウドデザインパターンcdp)
- [3. ベアメタルサービス構築ガイド(VMware ESXi)](#3-ベアメタルサービス構築ガイドvmware-esxi)

<!-- /TOC -->


---

### 1. IaaS初期構築ガイド  

FUJITSU Cloud Service for OSS IaaSを用いて、初めてシステムを構築する方向けの手順書  

- 新リージョン用ドキュメントを作成  

- 「[IaaS初期構築ガイド](https://doc.cloud.global.fujitsu.com/lib/iaas/jp/initial_guide/index.html)」の主な掲載内容  
    - 事前準備  
        - ユーザ／ロール作成  
        - ユーザをプロジェクトに登録  
    - ネットワーク構築  
    - SSL-VPN構築／接続  
    - 仮想サーバ構築／接続  
    - API操作方法  


---

### 2. クラウドデザインパターン(CDP)  

FUJITSU Cloud Service for OSS IaaSを用いた、代表的な設計パターンと構築手順  

- 「[クラウドデザインパターン・実装サンプル集](https://doc.cloud.global.fujitsu.com/lib/iaas/jp/cdp/index.html)」に、新リージョンの対応状況を掲載  
- 次回は、2019年3月末に更新予定です。


---

### 3. ベアメタルサービス構築ガイド(VMware ESXi)  

ベアメタルサーバの申込から、VMware ESXiにログインするまでの手順書  

- 「[ベアメタルサービス構築ガイド](https://doc.cloud.global.fujitsu.com/lib/iaas/jp/baremetal_inst_guide/index.html)」の主な掲載内容  
    - サンプル構成の説明  
    - 申込前の準備作業  
        - ベアメタルサーバと接続する、管理用ネットワークを構築  
        - 申込書の作成 → 管理用ネットワークに関する情報を記載  
    - ベアメタルサーバ配備後の環境構築  
        - 業務用ネットワーク  
        - ストレージ用ネットワーク  
        - トランク(VLAN)  
        - コンソール接続(iRMC)  
    - 接続確認  
        - iRMC  
        - VMware ESXi 管理コンソール  
        - vSphere Web Client  


---
