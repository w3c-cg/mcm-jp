# イベントとテレビ番組の同時検索

## 作成者
- 下花剛一（株式会社ジョルテ）

## 関連する産業ドメイン
事例に関連する産業を記述（複数可）
- イベント
- Web
- 地図
- 放送

## 事例概要
- 地図上でイベントを検索するサービス内で、イベント情報と一緒にテレビ番組の情報を混ぜて表示
  - [参考資料リンク](https://github.com/w3c-cg/mcm-jp/blob/main/reports/use-cases/event-metadata/%E5%8F%82%E8%80%83%E8%B3%87%E6%96%99.pdf)

## 目的
イベントと同時にテレビ番組を探す、もしくは気付くため仕組みを作る

## シナリオ

1. 放送関連事業者が、特番などの不定期で放送される番組の放送内容を選定し、提示する。
2. イベント検索サービス事業者が、放送内容をもとにイベントデータ化する。
3. イベント検索アプリ上で、地図が放送エリア内にある場合、イベント情報と一緒に表示する。

### 実装例（任意）

- イベントと一緒にテレビ番組を表示した画面

<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event1.png" alt="event1" width="400" />
<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event2.png" alt="event2" width="400" />
<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event3.png" alt="event3" width="400" />

- 日付ごとにテレビ番組を表示した画面

<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/bangumi1.png" alt="bangumi1" width="400" />
<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/bangumi2.png" alt="bangumi2" width="400" />
<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/bangumi3.png" alt="bangumi3" width="400" />

### 参照仕様など（任意）
-
<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/dataformat.png" alt="dataformat" width="400" />
- [イベントデータフォーマット](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event-data-format.xlsx)
- [イベントデータサンプル](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event-data_2025-01-14_2025-01-31.xlsx)

## CGへの課題共有
- 番組情報のデータ標準化
- 番組情報が提供されるタイミング
- 番組情報の許諾
- タグ付けと、イベント情報タグとの連動性
