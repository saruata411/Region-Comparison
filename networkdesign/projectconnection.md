# プロジェクト間通信

プロジェクト間の通信方式が異なります。



## 旧リージョン

仮想ルータに他プロジェクトのサブネット（ポート）を接続してプロジェクト間で通信します。

![old-projectconnection](images/old-projectconnection.png)



------



## 新リージョン

外部ネットワーク経由でグローバルIPアドレスやIPSecVPNでプロジェクト間で通信します。（外部ネットワークを使用しない方式を検討中）

![new-projectconnection](images/new-projectconnection.png)