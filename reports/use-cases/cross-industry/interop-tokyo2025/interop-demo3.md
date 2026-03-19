# 文字入力ソフト（IME）と出版コンテンツメタデータの連携 / Integration between IME and published content metadata
通常の文字入力では予測変換できない出版物の固有名詞（作品名・登場人物名など）を、書誌情報を参照した情報をIME辞書に登録し、
スマートフォン上のIMEで予測変換や補完入力を行う。

## 関連する産業ドメイン
- 出版
- コミュニケーションツール（IME）

## 書誌情報に基づく文字入力変換

試作構成における動作フローを示す。
- 出版社が書誌情報を作成する。
- IME事業者が書誌情報の「書名」・「書名 読み」を、IME辞書コンテンツの「表記文字列」「読み文字列」として収録する。
- ユーザが、スマートフォンのIMEアプリで書名のよみがなの一部を入力する。
- IMEアプリは、ユーザが入力したテキストをIME辞書の「読み文字列」として用いて、「表記文字列」から正式な「書名」を取得する。
- IMEアプリは、取得した表記文字列を変換候補として表示する。

![alt text](/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/interop3a.png "動作フロー概要")


## 実機デモの様子
Interop Tokyo 2025で展示したデモ外観を示す。

<figure>
    <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/ime-Yu-Gi-Oh!.png" alt="interop4" width ="33%" />
    <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/ime-re_zero.png" alt="interop4"  width ="33%" />
    <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/ime-taigan-no-kaji.png" alt="interop4"  width ="33%"/>
      <figcaption>Interop Tokyo 2025 デモ動作の様子</figcaption>
</figure>


## 参照仕様など
- [スマートフォン向け IME(iWnn IME for Android)＋クラウド辞書](#ref-ime)


## CGへの課題共有

