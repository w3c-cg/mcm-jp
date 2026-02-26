# 文字入力ソフト（IME）と出版コンテンツメタデータの連携
通常の文字入力では予測変換できない出版物の固有名詞（作品名・登場人物名など）を、書誌情報を参照した情報をIME辞書に登録し、
スマートフォン上のIMEで予測変換や補完入力を行う。

## 関連する産業ドメイン
- 出版
- コミュニケーションツール（IME）

## 試作・検証事例

### 書誌情報に基づく文字入力変換

試作構成における動作フローを示す。
- 出版社が書誌情報を作成する。
- IME事業者が書誌情報の「書名」・「書名 読み」を、IME辞書コンテンツの「表記文字列」「読み文字列」として収録する。
- ユーザが、スマートフォンのIMEアプリで書名のよみがなの一部を入力する。
- IMEアプリは、ユーザが入力したテキストをIME辞書の「読み文字列」として用いて、「表記文字列」から正式な「書名」を取得する。
- IMEアプリは、取得した表記文字列を変換候補として表示する。

![alt text](https://w3c-cg.github.io/mcm-jp/reports/use-cases/IME/interop3a.png "書誌情報に基づく文字入力変換 検証フロー")


## 参考事例

- スマートフォン向け IME(iWnn IME for Android)＋クラウド辞書

    - 【iWnn IME for Android】
    ![iWnn IME for Android](https://w3c-cg.github.io/mcm-jp/reports/use-cases/IME/image.png "iWnn IME for Android")
    - 【辞書開発プロセス】
    ![辞書開発プロセス](https://w3c-cg.github.io/mcm-jp/reports/use-cases/IME/image-2.png "辞書開発プロセス")
    - 【辞書データ構造】
    ![辞書データ構造](https://w3c-cg.github.io/mcm-jp/reports/use-cases/IME/image-3.png "辞書データ構造")

### 参照仕様など（任意）


## CGへの課題共有

