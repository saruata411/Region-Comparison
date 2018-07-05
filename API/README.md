# API



## はじめに

新リージョンでのAPI発行における実機検証ノウハウ。正式な情報は公開ドキュメントAPIリファレンスを参照ください。

旧リージョンの[API実行サンプル](https://k5-doc.jp-east-1.paas.cloud.global.fujitsu.com/doc/jp/iaas/document/api-sample/index.html)にある機能は、後述の[変更](#主な変更内容)を加えると新リージョンでも基本的に利用可能です。（一部、新リージョンで存在しないサービスもあります）

------



## Knowledge



### 主な変更内容

旧リージョンの[API実行サンプル](https://k5-doc.jp-east-1.paas.cloud.global.fujitsu.com/doc/jp/iaas/document/api-sample/index.html)を実行し、API内容の書き換えが必要だと分かったものです。

| 変更箇所                                                 | 変更ポイント                                                 |
| -------------------------------------------------------- | ------------------------------------------------------------ |
| AZ(Availability Zone)                                    | 新リージョンはシングルAZ構成のため「AZ」の概念がありません。そのためAPIに含まれる「availability_zone」系のパラメータは不要です。 |
| [APIバージョン](knowledge/APIVersion.md)                 | API発行時のpathに含まれるバージョンが変更されています。      |
| [APIのpath](knowledge/APIPath.md)                        | pathが変更されているAPIがあります。                          |
| [computeのAPIバージョン](knowledge/ComputeAPIVersion.md) | computeのAPIバージョンとして、新リージョンでは「v2.1」が追加されています。 |



### 新リージョンでの実行例

[プロジェクトIDの取得方法](knowledge/getProjectID.md)

[APIエンドポイントの取得方法](knowledge/getAPIendpoint.md)

[リモートコンソールでのアクセス方法](knowledge/connectRemoteConsole.md)

------

