# イベントとテレビ番組の同時検索 / Joint Discovery of Events and TV Programs
イベントと同時にテレビ番組を探す、もしくは気付くためのサービス事例。
地図上でイベントを検索するサービス内において、イベント情報とテレビ番組の情報を混在させて表示する。


## 関連する産業ドメイン
事例に関連する産業を記述（複数可）
- イベント
- Web
- 地図
- 放送

## シナリオ

1. 放送関連事業者が、特番などの不定期で放送される番組の放送内容を選定し、提示する。
2. イベント検索サービス事業者が、放送内容をもとにイベントデータ化する。
3. イベント検索アプリ上で、地図が放送エリア内にある場合、イベント情報と一緒に表示する。

## 検証事例

実証実験
[イベンティア（イベント情報提供サービス）](https://github.com/w3c-cg/mcm-jp/blob/main/reports/use-cases/event-metadata/%E5%8F%82%E8%80%83%E8%B3%87%E6%96%99.pdf)に対して、


イベントと一緒にテレビ番組を混在表示させる実証実験を実施。におけるアプリ画面を示す。

イベントと一緒にテレビ番組を表示した実証実験におけるアプリ画面を示す。

<figure>
  <img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event1.png" alt="event1" width="30%" />
  <img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event2.png" alt="event2" width="30%" />
  <img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event3.png" alt="event2" width="30%" />
  <figcaption>放送番組情報とイベントの混合表示画面</figcaption>
</figure>


<figure>
  <img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/bangumi1.png" alt="bangumi1" width="30%" />
  <img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/bangumi2.png" alt="bangumi2" width="30%" />
  <img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/bangumi3.png" alt="bangumi3" width="30%" />
  <figcaption>日付ごとにテレビ番組を表示した画面</figcaption>
</figure>

<span id="ref-eventia"></span>

## 参照仕様など / Referenced Specifications and Materials

<figure>
  <img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/dataformat.png" alt="dataformat" width="80%" />
  <figcaption> イベントデータフォーマット </figcaption>
</figure>

### イベンティア運用メタデータ仕様
- [イベントデータフォーマット](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event-data-format.xlsx)
  - イベンティアで運用されているイベント情報のフォーマット（xlsxファイル）
- [イベントデータサンプル](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event-data_2025-01-14_2025-01-31.xlsx)
  - イベント情報のサンプルデータ（xlsxファイル）

## CGへの課題共有
- 番組情報のデータ標準化
- 番組情報が提供されるタイミング
- 番組情報の許諾
- タグ付けと、イベント情報タグとの連動性
