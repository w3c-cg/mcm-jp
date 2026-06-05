# 放送メタデータに基づく出版プロモーション / Publishing Promotion Triggered by TV Exposure
放送メタデータの情報から、出版プロモーションで利用するトピックを検出し、
出版社サイトにトピックに基づく出版コンテンツのレコメンドが提供される事例。

## 関連する産業ドメイン
- 出版
- 放送

## シナリオ

1. 放送事業者が、書籍を紹介する番組を放送する
1. 放送メタデータ事業者が、当該番組を視聴し、EPGには含まれない書籍紹介情報（書籍タイトル・ISBN等）やシーン情報（TVクリップ：シーン概要・詳細時刻）を放送メタデータとして作成・提供する
1. 出版社サイトが、ISBNやデータ更新日時を用いて放送メタデータをモニタリングし、出版コンテンツと関連した番組が放送されたことを検出する
1. 出版社サイトが、出版コンテンツに関連する番組エピソードを特定し、番組エピソード名・サムネイル画像URL・放送局名・放送時刻を取得する
1. 出版社サイトが、TVクリップを参照し、書籍が関連するシーンの詳細時刻やシーン概要を取得する
1. 出版社サイトが、書籍のレコメンド情報を掲載する。このときレコメンドのきっかけとなった書籍を紹介した放送番組情報（番組エピソードのタイトル・サムネイル・局名・放送日時、放送・配信での視聴方法）があわせて表示される
1. ユーザは、出版社サイトを閲覧した際に、放送番組情報付きの書籍レコメンドに気づく
1. ユーザは、書籍ページから関連する放送番組へ、放送番組から関連書籍へ到達する

## 構成・動作フロー概要
<figure  width="80％">
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/tvtopic-rec-book-flow.png" alt="interop4" />
  <figcaption>構成概要・動作フロー概要</figcaption>
</figure>


## 検証イメージ外観

<figure  width="80％">
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/tvtopic-rec-book-outline.png" alt="interop4" />
  <figcaption>放送トピックによる出版プロモーションのイメージ</figcaption>
</figure>


<figure  width="80％">
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/book-landingpage.png" alt="interop4" />
  <figcaption>出版プロモーションページからの放送番組紹介イメージ</figcaption>
</figure>
