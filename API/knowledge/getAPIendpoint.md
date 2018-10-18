# APIエンドポイントの取得方法

## API発行例  

トークンを取得後、以下のようなコマンドで取得可能です。

- $REG：リージョン  
- $IDENTITY：利用者管理のAPIエンドポイント  
- $TOKEN：取得したトークン  

```
REG=jp-west-3
IDENTITY=https://identity.$REG.cloud.global.fujitsu.com
TOKEN=zzzzz

curl -s $IDENTITY/v3/auth/catalog -X GET -H "X-Auth-Token: $TOKEN" | jq '.catalog[].endpoints[].url'
```


---


実行結果(2018年10月時点)  

- xxxxx：プロジェクトID  

```
"https://compute.jp-west-3.cloud.global.fujitsu.com/v2.1/xxxxx"
"https://keymanagement.jp-west-3.cloud.global.fujitsu.com"
"https://image.jp-west-3.cloud.global.fujitsu.com"
"https://objectstorage.jp-west-3.cloud.global.fujitsu.com/v2/AUTH_xxxxx"
"https://networking.jp-west-3.cloud.global.fujitsu.com"
"https://orchestration.jp-west-3.cloud.global.fujitsu.com/v1/xxxxx"
"https://blockstorage.jp-west-3.cloud.global.fujitsu.com/v2/xxxxx"
"https://database.jp-west-3.cloud.global.fujitsu.com/v1.0/xxxxx"
"https://blockstorage.jp-west-3.cloud.global.fujitsu.com/v3/xxxxx"
"https://identity.jp-west-3.cloud.global.fujitsu.com"
"https://compute.jp-west-3.cloud.global.fujitsu.com/v2/xxxxx"
"https://nfv.jp-west-3.cloud.global.fujitsu.com"
"https://baremetal.jp-west-3.cloud.global.fujitsu.com"
"https://telemetry.jp-west-3.cloud.global.fujitsu.com"
"https://software.jp-west-3.cloud.global.fujitsu.com"
"https://autoscale.jp-west-3.cloud.global.fujitsu.com"
"https://identity.jp-west-3.cloud.global.fujitsu.com/v3"
"https://import-export.jp-west-3.cloud.global.fujitsu.com"
```
