# リモートコンソールでのアクセス方法  

## 目次  

<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. API発行例](#1-api発行例)
- [2. 実行結果](#2-実行結果)
- [3. リモートコンソール接続](#3-リモートコンソール接続)

<!-- /TOC -->


---

### 1. API発行例  

仮想サーバを作成後、以下のコマンドで「リモートコンソールアクセス用のURL」を取得します。  
- $COMPUTE：コンピュートのAPIエンドポイント
- $PROJECT_ID：プロジェクトID  
- $SERVER_ID：リモートコンソールアクセスしたい仮想サーバのID  
- $TOKEN：トークン  

```
curl -X POST -i $COMPUTE/v2/$PROJECT_ID/servers/$SERVER_ID/action -H "X-Auth-Token: $TOKEN" -H "Content-Type:  application/json" -d '{"os-getVNCConsole": {"type": "novnc"}}'
```


---

### 2. 実行結果  

```
{"console": {"url": "https://console.jp-west-3.cloud.global.fujitsu.com/vnc_auto.html?token=e80958fa-2ec1-4658-8d84-aaaaaaaaaaa", "type": "novnc"}}
```


---

### 3. リモートコンソール接続  

chromeブラウザにて「リモートコンソールアクセス用のURL」へアクセスします。

```
https://console.jp-west-3.cloud.global.fujitsu.com/vnc_auto.html?token=e80958fa-2ec1-4658-8d84-aaaaaaaaaaa
```


---
