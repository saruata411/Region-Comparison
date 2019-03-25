# プロジェクトIDの取得方法  

## 目次  

<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. API発行例](#1-api発行例)

<!-- /TOC -->


---

### 1. API発行例  

トークンを取得後、以下のコマンドで取得可能です。  

- $REG：リージョン  
- $IDENTITY：利用者管理のAPIエンドポイント  
- $TOKEN：取得したトークン  

```
REG=jp-west-3
IDENTITY=https://identity.$REG.cloud.global.fujitsu.com
TOKEN=zzzzz

curl -s $IDENTITY/v3/auth/projects -X GET -H  "X-Auth-Token: $TOKEN" | jq '.projects[] | {"name": .name, "id": .id, "description": .description}'
```


---
