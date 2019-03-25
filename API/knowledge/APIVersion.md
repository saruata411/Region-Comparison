# APIバージョンの変更  

## 目次  

<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. 変更ポイント](#1-変更ポイント)
- [2. ブロックストレージ](#2-ブロックストレージ)
- [3. オブジェクトストレージ](#3-オブジェクトストレージ)
- [4. コンピュート](#4-コンピュート)

<!-- /TOC -->


---

### 1. 変更ポイント  

APIバージョンが変更されています。  


------

### 2. ブロックストレージ  

「v2」から「v3」へ変更されています。  

- $BLOCKSTORAGE：ブロックストレージのAPIエンドポイント  
- $PROJECT_ID：プロジェクトID  
- $TOKEN：トークン  


#### 変更前  

```
curl -Ss $BLOCKSTORAGE/v2/$PROJECT_ID/volumes -X GET -H "X-Auth-Token:$TOKEN" -H "Content-Type:application/json" | jq .
```

#### 変更後  

```
curl -Ss $BLOCKSTORAGE/v3/$PROJECT_ID/volumes -X GET -H "X-Auth-Token:$TOKEN" -H "Content-Type:application/json" | jq .
```


---

### 3. オブジェクトストレージ  

「v1」から「v2」へ変更されています。  

- $OBJECTSTORAGE：オブジェクトストレージのAPIエンドポイント  
- $PROJECT_ID：プロジェクトID  
- $TOKEN：トークン  

#### 変更前  

```
curl -Ss $OBJECTSTORAGE/v1/AUTH_$PROJECT_ID?format=json -X GET -H  "X-Auth-Token: $TOKEN" | jq .
```

#### 変更後  

```
curl -Ss $OBJECTSTORAGE/v2/AUTH_$PROJECT_ID?format=json -X GET -H  "X-Auth-Token: $TOKEN" | jq .
```


------

### 4. コンピュート  

新リージョンでは「v2.1」が追加されています。旧リージョンでは「v2」のみです。  
以下の両方のバージョンでAPIを試行しましたが、特に差異はありません。  

- $COMPUTE：コンピュートのAPIエンドポイント  
- $PROJECT_ID：プロジェクトID  
- $TOKEN：トークン  

#### 変更前  

```
curl -Ss $COMPUTE/v2/$PROJECT_ID/servers/detail -X GET -H "X-Auth-Token: $TOKEN" | jq .
```

#### 変更後  

```
curl -Ss $COMPUTE/v2.1/$PROJECT_ID/servers/detail -X GET -H "X-Auth-Token: $TOKEN" | jq .
```


---
