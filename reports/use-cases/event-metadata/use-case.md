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
  - [参考資料リンク](https://github.com/w3c-cg/mcm-jp/tree/main/reports/use-cases/event-metadata/参考情報.pdf)

## 目的
イベントと同時にテレビ番組を探す、もしくは気付くため仕組みを作る

## シナリオ

1. 放送関連事業者が、特番などの不定期で放送される番組の放送内容を選定し、提示する。
2. イベント検索サービス事業者が、放送内容をもとにイベントデータ化する。
3. イベント検索アプリ上で、地図が放送エリア内にある場合、イベント情報と一緒に表示する。

### 実装例（任意）

- イベントと一緒にテレビ番組を表示した画面

![画像貼り付け（event1）](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event1.png "event1")
![画像貼り付け（event2）](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event2.png "event2")
![画像貼り付け（event3）](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event3.png "event3")

- 日付ごとにテレビ番組を表示した画面

![画像貼り付け（bangumi1）](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/bangumi1.png "bangumi1")
![画像貼り付け（bangumi2）](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/bangumi2.png "bangumi2")
![画像貼り付け（bangumi3）](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/bangumi3.png "bangumi3")

### 参照仕様など（任意）

![画像貼り付け（dataformat）](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/format.png "dataformat")
- [イベントデータフォーマット](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event-data-format.xlsx)
- [イベントデータサンプル](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event-data_2025-01-14_2025-01-31.xlsx)

## CGへの課題共有
- 番組情報のデータ標準化
- 番組情報が提供されるタイミング
- 番組情報の許諾
- タグ付けと、イベント情報タグとの連動性
