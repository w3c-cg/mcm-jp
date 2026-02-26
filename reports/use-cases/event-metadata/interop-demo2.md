# 車載インフォテインメントシステムにおける催事イベントと関連するテレビ番組・出版コンテンツのレコメンド

車載インフォテインメントシステムの現在位置情報やナビゲーション目的地情報などを用いて、
催事イベント情報、テレビ番組、出版コンテンツのレコメンドを行う。

## 試作・検証事例

### 位置情報から番組情報取得

<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/interop2a.png" alt="interop2a" width="400" />


## 関連メタデータ仕様

- イベンティア： 催事イベントメタデータサンプル
<img src="https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/dataformat.png" alt="dataformat" width="400" />

- [イベンティア参考資料](https://github.com/w3c-cg/mcm-jp/blob/main/reports/use-cases/event-metadata/%E5%8F%82%E8%80%83%E8%B3%87%E6%96%99.pdf)

- [イベントデータフォーマット](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event-data-format.xlsx)
- [イベントデータサンプル](https://w3c-cg.github.io/mcm-jp/reports/use-cases/event-metadata/event-data_2025-01-14_2025-01-31.xlsx)

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