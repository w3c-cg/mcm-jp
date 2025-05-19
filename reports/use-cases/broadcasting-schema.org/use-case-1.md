# 放送実績情報による放送番組の特定とオンデマンド配信での視聴方法の取得

## 作成者
- 遠藤 大礎（NHK）

## 関連する産業ドメイン
- 放送
- OTTサービス

## 事例概要
- 放送実績情報（チャンネル、放送時刻）から放送番組を特定し、放送予定・配信情報などの番組情報を取得する

## 目的
- ユーザが既知の情報から放送番組を特定し、放送や配信で番組を視聴できるようにすること

## シナリオ

1. 放送事業者が、ある放送番組を放送し、放送実績情報を放送メタデータサーバに登録する
2. ユーザが、放送終了後に放送番組の視聴を受信機にリクエストする
3. 受信機は、当該番組の放送実績（チャンネル、放送時刻）をもとに、放送メタデータサーバで番組情報を検索する
4. 放送メタデータサーバは、受信機に対して当該番組のEPG情報に加えて、詳細情報（シリーズ、出演者など）や提供情報（放送情報、配信情報）を回答する
5. 受信機は、レスポンスを元に、当該番組を視聴する方法をユーザに提示する
6. ユーザは、視聴方法の候補をもとに、配信サービスでの視聴や、放送視聴予約・放送録画予約などを行う

### 実装例


#### 動作環境（TBD）
- 受信機: 
  - Hybridcast対応受信機
    - LG OLED42C2PJA
- 受信機アプリケーション
  - Webアプリケーションによる実装（Hybridcast）
    - HTML/CSS/JavaScript
- 放送メタデータサーバ
  - API仕様（OpenAPI仕様[TBD]）に基づく実装
    - Ubuntu 22.04
    - PostgreSQL 16
    - Flask (Python)
    - OpenAPI Generator
      - OpenAPI仕様
      - generator: python-flask 
- 放送局: 放送メタデータ登録スクリプト
  - 放送実績情報(BroadcastEvent)および、放送番組情報（TVEpisode）などのメタデータ登録
  - API仕様（OpenAPI仕様[TBD]）に基づく実装
    - OS: Ubuntu 22.04
    - Python
    - OpenAPI Generator
      - OpenAPI仕様
      - generator: python

#### 処理シーケンス（TBD）
- 放送事業者、放送メタデータサーバ、受信機、ユーザーの構成を図1に示す
- 放送メタデータサーバは、放送メタデータの登録APIと、参照APIをもつ
  - 放送メタデータサーバAPI仕様(リンク記載)
  - メタデータのデータモデル（図2）
    - Schema.orgの語彙、データ構造などのRDFスキーマに基づく記述
- 放送事業者が、放送メタデータサーバに放送実績情報を登録する。メタデータのサンプルを図3に示す
  - 放送枠（BroadcastEvent）とその番組枠で提供された放送番組（TVEpisode）の関係性を登録する
  - 放送番組（TVEpisode）に対して、詳細情報（シリーズ、出演者など）や提供情報（放送情報、配信情報）を登録する
- ユーザーが受信機に対して、放送が終了した番組の視聴をリクエストする
  - 受信機は、放送チャンネルと放送時刻の情報を検索パラメータとして、放送メタデータサーバに問合せ、番組枠（BroadcastEvent）と放送番組（TVEpisode）を特定する（図4 検索API例）
- 放送メタデータサーバは、受信機に対して、BroadcastEvent、TVEpisodeの情報を返答する
  - 図2に示すように、TVEpisodeには、オンデマンド配信枠（OnDemandEvent）の情報などが紐づいている
- 受信機は、TVEpisodeの提供方法として、現在利用可能な複数のBroadcastEventおよびOnDemandEventを視聴方法として提示する
- ユーザーは、提示された視聴方法の候補のうち、あるVODサービスを示すOnDemandEventを選択する
- 受信機は、指定されたOnDemandEventにより、番組の再生を行う

### 図
- 図1. システム構成例
<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/broadcasting-schema.org/configuration.png" alt="システム構成例" width="400" />
- 図2. データモデル
<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/broadcasting-schema.org/datamodel.png" alt="データモデル" width="400" />
- 図3. 放送メタデータサンプル
<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/broadcasting-schema.org/data_sample.png" alt="放送メタデータサンプル" width="400" />
- 図4. 検索API例
<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/broadcasting-schema.org/api_sample.png" alt="検索API例" width="700" />


### 参照仕様など
- データモデル
  - [Schema.org](https://schema.org/)
    - 構造化データの語彙や表現ルールを共有する共同コミュニティ活動
  - [Google Media Actions](https://developers.google.com/actions/media)
    - メディアコンテンツの説明をGoogleに提供するためのガイドライン
- 放送サービスのためのグローバルプラットフォームのユースケース・要求条件・技術要素
  - [Report ITU-R BT.2400 -Usage scenarios,requirements and technical elements of a global platform for the broadcasting service", ITU-R](https://www.itu.int/pub/R-REP-BT.2400)
    - 放送通信連携システムに関するユースケースや要求条件、実装事例など
  