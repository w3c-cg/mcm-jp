# 車載インフォテインメントシステムにおける催事イベントと関連するテレビ番組・出版コンテンツのレコメンド / Recommendation of TV Programs and Published Content Related to Events in In‑Vehicle Infotainment Systems

車載インフォテインメントシステムの現在位置情報やナビゲーション目的地情報などを用いて、
催事イベント情報、テレビ番組、出版コンテンツのレコメンドを行う。

## 試作・検証事例

車載インフォテインメントシステムの位置情報を利用して、イベンティアアプリ上でイベント情報と放送番組を混在したレコメンドを行う流れを示す。

<img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/interop2a.png" alt="interop2a" width="800" />


## 実機デモ外観

Interop Tokyo 2025で展示したデモ外観を示す。

<img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/interop2-configuration.png" alt="interop2a" width="800" />

## 実装環境・関連メタデータ仕様

- 車載インフォテインメントシステム（IVI）
  - [NetFront® Browser for Automotive（ACCESS）](https://www.access-company.com/products/browser/netfront-browser-be/)
- イベント情報メタデータ仕様
  - [イベンティア メタデータ関連事例・サンプル（ジョルテ）](#ref-eventia)
- 放送番組メタデータ仕様
  - [TVメタデータ 参照事例（エム・データ）](#tv-trend-alert-service-for-potential-hit-products-using-broadcast-and-search-data)
    - [TVメタデータサンプル（スポット関連メタデータ）](https://github.com/w3c-cg/mcm-jp/blob/main/reports/use-cases/TV-metadata/sample-data-3_spot.csv)
- 位置情報関連仕様
  - W3C Geoloation API[[geolocation]]を用いた緯度・経度情報の取得


## CGへの課題共有
- 催事イベントにおいて、緯度経度など物理的情報の運用
  - 花火大会など、広いエリアのイベントにおいて、どの地点を登録するか
  - 複数地点の入力を許容するか
    - イベンティアでは実運用上1点として運用中。設計上複数地点登録が可能だが、運用が複雑化する。
- 催事イベントのスポット名など意味的情報の運用
  - 施設・エリアの名称について、正式名称が必ずしも特定できない場合あり。略称、通称などシステム間で共通の値が採用されず、検索などが意図通りできない可能性あり。
- 事業者間でイベント情報の相互運用性を確保するためには、メタデータの生成・登録におけるルールが共有されている必要がある。下記に示すように、規定や運用により様々な共有方法が想定される。
  - イベント情報について、共通のユニークなidを付与する。
  - 共通のデータベースを参照可能とする。
  - イベント情報について、既存仕様で規定されたスキーマを採用し、イベント情報がもつ属性情報などのルールを共有する。