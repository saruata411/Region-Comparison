# computeのAPIバージョン追加

### 概要

computeのAPIバージョンとして、新リージョンでは「v2.1」が追加されています。旧リージョンでは「v2」のみです。

「v2.1」のエンドポイントのtypeは「compute」となっています。

「v2」のエンドポイントのtypeは「compute_legacy」となっています。

以下の両方のバージョンでAPIを試行しましたが特に差異はありません。

`curl -Ss $COMPUTE/v2.1/$PROJECT_ID/servers/detail -X GET -H "X-Auth-Token: $OS_AUTH_TOKEN" | jq .`

`curl -Ss $COMPUTE/v2/$PROJECT_ID/servers/detail -X GET -H "X-Auth-Token: $OS_AUTH_TOKEN" | jq .`

