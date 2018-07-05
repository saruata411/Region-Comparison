# プロジェクトIDの取得方法

APIの発行例です。トークンを取得後、以下のコマンドで取得可能です。

```
curl -k -X POST -s $TOKEN/v3/auth/tokens -H "Content-Type: application/json" -H "Accept:application/json" -d '{"auth":{"identity":{"methods":["password"],"password":{"user":{"domain":{"name":"'$DOMAIN_NAME'"}, "name": "'$USER_NAME'", "password": "'"$USER_PW"'"}}}, "scope": { "project": {"name": "'$PROJECT_NAME'", "domain":{"name":"'$DOMAIN_NAME'"}}}}}' | jq '.token.project.id'
```

- $TOKEN：トークン
- $DOMAIN_NAME：ドメイン名
- $USER_NAME：ユーザー名
- $USER_PW：パスワード

