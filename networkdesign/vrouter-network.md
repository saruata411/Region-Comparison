# 仮想ルータとネットワークの接続

仮想ルータとネットワークの接続の差異があります。




## 旧リージョン

１つのネットワークを複数の仮想ルータに接続可能です。

![old-sample00](images/old-sample00.png)



**2階層ネットワーク構成の例**

![old-sample01](images/old-sample01.png)

------



## 新リージョン

１つのネットワークは１つの仮想ルータに接続するシンプル構成です。

![new-sample00](images/new-sample00.png)

具体的な構成例については、[複数ネットワークの構成例](#複数ネットワークの構成例)、および[バックLAN構成例](#バックlan構成例)をご参照ください。また参考としてIPCOM VAを使う[参考構成例](#参考構成例)も記載しています。



### 複数ネットワークの構成例

**仮想ルータ1つで両階層ネットワークを接続する構成例**

![new-sample01](images/new-sample01.png)



------

### バックLAN構成例

**仮想ルータによる構成例１**

![new-backlan-sample01](images/new-backlan-sample01.png)



**仮想ルータによる構成例2**

![new-backlan-sample02](images/new-backlan-sample02.png)



------

### 参考構成例

以降はIPCOM VAを使った参考の構成例です。



**IPCOM VAで階層を分ける構成例**

![new-sample02](images/new-sample02.png)



**IPCOM VAで階層を分け一部通信を仮想ルータ経由とする構成例**

![new-sample03](images/new-sample03.png)



**IPCOM VAによるバックLAN構成例1**

![new-backlan-sample03](images/new-backlan-sample03.png)



**IPCOM VAによるバックLAN構成例2**

![new-backlan-sample04](images/new-backlan-sample04.png)



**IPCOM VAによるバックLAN構成例3**

![new-backlan-sample05](images/new-backlan-sample05.png)

