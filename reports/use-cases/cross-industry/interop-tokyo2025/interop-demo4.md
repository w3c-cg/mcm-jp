# 書籍検索サイトでのタイトル補完入力 / Book title autocomplete input on a book search site
作品の検索ページで入力される固有名詞（作品名・登場人物名など）の表記揺らぎを解消し、検索精度を向上させる事例。
書籍検索サイトでのWeb埋め込み側IMEによるタイトル補完入力が提供される。

## 関連する産業ドメイン
- 出版
- コミュニケーションツール（IMEソフトウェア）

## シナリオ

1. 出版社が、書籍を発売する
1. 出版社が、書誌情報をデータベース化する
1. IME事業者が、Web埋め込み側IME（以下、Web IME）と読み揺らぎパターン自動生成機能付き辞書作成ツールを出版社に提供する
1. 出版社が、Web IMEを書籍検索サイトの検索BOXにWeb IMEを組み込む
1. 出版社が、書誌情報データベースから書籍タイトルの正しい「読み」および読み揺らぎパターンの「読み」／「表記」情報をWeb IMEの辞書データとして登録する
1. 書籍検索サイト利用ユーザは、書籍検索の際、間違えた読みを入力しても、正しい書籍タイトルの文字変換ができることで、意図した書籍検索結果が得られる

<figure>
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/interop4a.png" alt="interop4" width="800" />
  <figcaption>動作イメージ概要</figcaption>
</figure>

<figure>
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/interop4b.png" alt="interop4b" width="800" />
  <figcaption>動作フロー概要</figcaption>
</figure>


## デモ動作
Interop Tokyo 2025で展示したデモ外観を示す。

<figure>
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/ime-book-search.png" alt="interop4b" width="800" />
  <figcaption>実機デモ動作外観</figcaption>
</figure>

## 参照仕様など
- [スマートフォン向け IME(iWnn IME for Android)＋クラウド辞書 (3.2参照)](#ref-ime)


