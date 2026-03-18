# 催事イベントと関連するテレビ番組・出版コンテンツのレコメンド / Recommendation of TV Programs and Published Content Related to Events

ユーザの位置情報や日時情報などを用いて、催事イベント情報、テレビ番組、出版コンテンツのレコメンドを行う。

## 試作・検証事例

### 日付から番組情報取得
- ある日時に放送されている番組を、放送編成枠情報の検索エンドポイントで検索する
- 放送編成枠情報に紐づくTVエピソードを特定する
- 番組エピソード名や、サムネイル画像などを視聴放送編成枠情報に紐づくTVエピソードを特定する
- 取得した放送関連情報を、イベント情報などと合わせて一覧表示

<figure>
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/interop1a.png" alt="interop1a" width="800" />
  <figcaption>日付から番組情報取得フロー</figcaption>
</figure>

### 日付から書籍情報取得
<figure>
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/interop1b.png" alt="interop1b" width="800" />
  <figcaption>日付から書籍情報取得</figcaption>
</figure>


### 位置情報から番組情報取得
<figure>
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/interop1c.png" alt="interop1c" width="800" />
  <figcaption>位置情報から番組情報取得</figcaption>
</figure>


### 放送番組情報から関連する関連する書誌情報の取得
<figure>
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/interop1d.png" alt="interop1d" width="800" />
  <figcaption>放送番組情報から関連する関連する書誌情報の取得</figcaption>
</figure>


## 関連メタデータ仕様

- [イベンティア： 催事イベントメタデータサンプル](#ref-eventia)


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