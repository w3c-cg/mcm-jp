<h1 id="recommendation-of-tv-programs-and-published-content-related-to-events-in-in-vehicle-infotainment-systems"><span lang="ja">車載インフォテインメントシステムにおける催事イベントと関連するテレビ番組・出版コンテンツのレコメンド</span> <span lang="en">Recommendation of TV Programs and Published Content Related to Events in In‑Vehicle Infotainment Systems</span></h1>

<div lang="ja">

車載インフォテインメントシステムの現在位置情報やナビゲーション目的地情報などを用いて、イベント情報、テレビ番組、出版コンテンツのレコメンドを行う。

</div>

<div lang="en">

Recommends events, TV programs, and published content using current location and navigation destination information from in-vehicle infotainment systems.

</div>

## 試作・検証事例

車載インフォテインメントシステムの位置情報を利用して、イベンティアアプリ上でイベント情報と放送番組を混在したレコメンドを行う流れを示す。

<figure>
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/interop2a.png" alt="イベンティアアプリでのレコメンド動作の流れ" width="800" />
  <figcaption>イベンティアアプリでのレコメンド動作の流れ</figcaption>
</figure>


## 実機デモ外観

Interop Tokyo 2025で展示したデモ外観を示す。

<figure>
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/interop2-configuration.png" alt="Interop Tokyo 2025 展示デモ外観" width="800" />
  <figcaption>Interop Tokyo 2025 展示デモ外観</figcaption>
</figure>

## 実装環境・関連メタデータ仕様

- 車載インフォテインメントシステム（IVI）
  - [NetFront® Browser for Automotive（ACCESS）](https://www.access-company.com/products/browser/netfront-browser-be/)
- イベント情報メタデータ仕様
  - [イベンティア メタデータ関連事例・サンプル（ジョルテ）](#ref-eventia)
- 放送番組メタデータ仕様
  - [TVメタデータ 参照事例（エム・データ）](#ref-tv-metadata)
    - [TVメタデータサンプル（スポット関連メタデータ）](https://github.com/w3c-cg/mcm-jp/blob/main/reports/use-cases/TV-metadata/sample-data-3_spot.csv)
- 位置情報関連仕様
  - W3C Geolocation API [[geolocation]] を用いた緯度・経度情報の取得
