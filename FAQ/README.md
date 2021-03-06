# FAQ

新リージョンについてよくある問い合わせ。

| QUESTION                                  | ANSWER                                                                                               |
|:------------------------------------------|:-----------------------------------------------------------------------------------------------------|
| アピールポイントは？                      | ・可用性が向上し、SLAの適用が容易になりました。                                                      |
|                                           | ・シングルAZのシンプル構成のため、設計や運用などの負担が軽減されます。                               |
|                                           | ・ベアメタルが提供されます。                                                                         |
|                                           | ・BCP対応として、ストレージをリージョン間でコピーする機能が提供されます。                            |
| 旧リージョンと何が違うの？                | ベースとなっているOpenStackのバージョンが異なります。                                                |
|                                           | 富士通独自開発を加えておらず、標準のOpenstackを使用しています。                                      |
|                                           | 標準Openstackのため、世の中で広く使われているツール（例：Ansibleなど）が利用できるようになりました。 |
| 旧リージョンに比べて何が良いの？①         | シングルAZ構成での可用性が向上し、シングルAZの利用でSLAが適用されるようになりました。                |
|                                           | 例)                                                                                                  |
|                                           | ・電源やネットワーク機器など、設備機器の多重度をアップ                                               |
|                                           | ・物理サーバ故障時の影響範囲を極小化                                                                 |
| 旧リージョンに比べて何が良いの？②         | シングルAZ構成のため、設計・構築・テスト・運用の負担が軽減されます。                                 |
| 旧リージョンに比べて何が良いの？③         | SAP HANA専用ではないベアメタルが提供されます。                                                       |
| 旧リージョンに比べて考慮が必要なことは？① | 機能や構成を改善した影響で、技術的考慮が必要になった部分があります。                                 |
|                                           | 例)                                                                                                  |
|                                           | ・シングルAZのため、データセンターダウンのような大規模災害におけるBCPやDRPの検討                     |
|                                           | ・OpenStack標準のロードバランサーはアクティブ・スタンバイ構成                                        |
| 旧リージョンに比べて考慮が必要なことは？② | サービスメニューや機能が変更された部分があります。                                                   |
|                                           | 例)                                                                                                  |
|                                           | ・プロジェクト間通信の設定は、ヘルプデスクに依頼が必要                                               |
|                                           | ・オートスケールしたVMをロードバランサー配下に入れるための作業が必要                                 |
| 旧リージョンに比べて価格は？              | 同価格帯です。                                                                                       |
| ユーザーポータルは旧リージョンと同じ？    | 変更された機能もあります。詳しくは[「ユーザーポータル」](../userportal/README.md)をご覧ください。    |
| APIは旧リージョンと同じ？                 | 変更されたAPIもあります。詳しくは[「API」](../API/README.md)をご覧ください。                         |
| 旧リージョンと同じシステム構成で良い？    | 旧リージョンと異なる点もあるため、見直しが必要です。                                                 |
|                                           | 例)                                                                                                  |
|                                           | ・１つのネットワークを２つの仮想ルータに接続できない                                                 |
|                                           | ・ネットワークコネクターの廃止                                                                       |
