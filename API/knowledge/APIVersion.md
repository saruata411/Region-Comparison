# APIバージョンの変更

API発行時のpathに含まれるバージョンが変更されています。

------

## ブロックストレージ

### 概要

「v2」から「v3」へ変更されています。

### 変更例

##### 変更前

```
curl -Ss $BLOCKSTORAGE/v2/$PROJECT_ID/volumes -X GET -H "X-Auth-Token:$OS_AUTH_TOKEN" -H "Content-Type:application/json" | jq .
```

##### 変更後

```
curl -Ss $BLOCKSTORAGE/v3/$PROJECT_ID/volumes -X GET -H "X-Auth-Token:$OS_AUTH_TOKEN" -H "Content-Type:application/json" | jq .
```

------



## オブジェクトストレージ

### 概要

「v1」から「v2」へ変更されています。

### 変更例

##### 変更前

```
curl -Ss $OBJECTSTORAGE/v1/AUTH_$PROJECT_ID?format=json -X GET -H  "X-Auth-Token: $OS_AUTH_TOKEN" | jq .
```

##### 変更後

```
curl -Ss $OBJECTSTORAGE/v2/AUTH_$PROJECT_ID?format=json -X GET -H  "X-Auth-Token: $OS_AUTH_TOKEN" | jq .
```

------

