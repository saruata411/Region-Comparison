# APIのpathの変更

pathが変更されているAPIがあります。

------



## 鍵管理

### 概要

「プロジェクトID」が不要になっています。

### 変更例１

##### 変更前

```
curl -Ss $KEYMANAGEMENT/v1/$PROJECT_ID/secrets -X GET -H "X-Auth-Token: $OS_AUTH_TOKEN" -H "Content-Type: application/json" | jq .
```

##### 変更後

```
curl -Ss $KEYMANAGEMENT/v1/secrets -X GET -H "X-Auth-Token: $OS_AUTH_TOKEN" -H "Content-Type: application/json" | jq .
```

### 変更例２

##### 変更前

```
curl -Ss $KEYMANAGEMENT/v1/$PROJECT_ID/containers -X GET -H "X-Auth-Token: $OS_AUTH_TOKEN" -H "Content-Type: application/json" | jq .
```

##### 変更後

```
curl -Ss $KEYMANAGEMENT/v1/containers -X GET -H "X-Auth-Token: $OS_AUTH_TOKEN" -H "Content-Type: application/json" | jq .
```

