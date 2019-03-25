# APIのpath変更  

## 目次  

<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. 変更ポイント](#1-変更ポイント)
- [2. 鍵管理](#2-鍵管理)

<!-- /TOC -->


---

### 1. 変更ポイント  

pathが変更されているAPIがあります。  


---

### 2. 鍵管理  

「プロジェクトID」が不要になっています。  


---

#### 変更例１  

- $KEYMANAGEMENT：鍵管理のAPIエンドポイント  
- $PROJECT_ID：プロジェクトID  
- $TOKEN：トークン  


##### 変更前  

```
curl -Ss $KEYMANAGEMENT/v1/$PROJECT_ID/secrets -X GET -H "X-Auth-Token: $TOKEN" -H "Content-Type: application/json" | jq .
```

##### 変更後  

```
curl -Ss $KEYMANAGEMENT/v1/secrets -X GET -H "X-Auth-Token: $TOKEN" -H "Content-Type: application/json" | jq .
```


---

#### 変更例２  

- $KEYMANAGEMENT：鍵管理のAPIエンドポイント  
- $PROJECT_ID：プロジェクトID  
- $TOKEN：トークン  


##### 変更前  

```
curl -Ss $KEYMANAGEMENT/v1/$PROJECT_ID/containers -X GET -H "X-Auth-Token: $TOKEN" -H "Content-Type: application/json" | jq .
```

##### 変更後  

```
curl -Ss $KEYMANAGEMENT/v1/containers -X GET -H "X-Auth-Token: $TOKEN" -H "Content-Type: application/json" | jq .
```


---
