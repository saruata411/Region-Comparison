# Heatテンプレート



## はじめに

新リージョンでのHeatテンプレート利用における実機検証ノウハウ。正式な情報は公開ドキュメント機能説明書やOpenStackの公開情報を参照ください。



------



## Knowledge



### 主な注意点

| 項目           | 注意点                                                       |
| -------------- | ------------------------------------------------------------ |
| AZ数           | 新リージョンではAZ数は1です。マルチリージョンを利用するHeatテンプレートは利用できません。 |
| リソースタイプ | 利用できるリソースタイプ（resourcesに記載するtypes）に違いがありますので見直しが必要な場合があります。 |
