# リモートコンソールでのアクセス方法

#### 1. URL取得

仮想サーバを作成後、以下のコマンドで「リモートコンソールアクセス用のURL」を取得します。

※リモートコンソールアクセスしたい仮想サーバのID（$SERVER_ID）は、仮想サーバの参照APIで取得します。

##### 発行

```
curl -X POST -i $COMPUTE/v2/d64ecc60697f476e8fe3xxxxxxxx/servers/4f4bcae0-7935-4f78-b4fc-aaaaaaaa/action -H "X-Auth-Token: $OS_AUTH_TOKEN" -H "Content-Type:  application/json" -d '{"os-getVNCConsole": {"type": "novnc"}}'
```

##### 結果

```
{"console": {"url": "https://console.jp-west-3.cloud.global.fujitsu.com/vnc_auto.html?token=e80958fa-2ec1-4658-8d84-aaaaaaaaaaa", "type": "novnc"}}
```



#### 2. 接続

chromeブラウザにて「リモートコンソールアクセス用のURL」へアクセスします。

```
https://console.jp-west-3.cloud.global.fujitsu.com/vnc_auto.html?token=e80958fa-2ec1-4658-8d84-aaaaaaaaaaa
```

