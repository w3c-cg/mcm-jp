# 固有名詞に関するIME辞書データの自社作成と展開 / In-house Development and Deployment of IME Dictionary Data for Proper Nouns

## 作成者
- 出野 健太郎（オムロンソフトウェア）

## 関連する産業ドメイン
- 出版
- コミュニケーションツール（IME）

## 事例概要
- メディアコンテンツに関連する固有名詞をIMEで文字変換できる
  - [参考資料](https://github.com/w3c-cg/mcm-jp/blob/main/meetings/2024-07-25/20240725_mcm-jp-cg_%E3%82%AA%E3%83%A0%E3%83%AD%E3%83%B3%E3%82%BD%E3%83%95%E3%83%88%E3%82%A6%E3%82%A7%E3%82%A2IME%E7%B4%B9%E4%BB%8B%E8%B3%87%E6%96%99.pdf)

## 目的
メディアコンテンツに関する新しい固有名詞について、ユーザが文字変換できるようにすること

## シナリオ

1. 出版社がマンガを発売する
1. IME事業者が、マンガの登場キャラクタ等の固有名詞を収集する
1. IME事業者が、市場での需要を鑑み、収集した固有名詞を選別し、IME辞書コンテンツとして収録する
1. IME事業者が、収録した辞書コンテンツをスマートフォンにインストールされているIMEに反映する
1. スマートフォンユーザは、マンガの登場キャラクタ名を文字入力する際、IMEで変換できる

### 実装例（任意）

#### スマートフォン向け IME(iWnn IME for Android)＋クラウド辞書

- 【iWnn IME for Android】
![iWnn IME for Android](https://w3c-cg.github.io/mcm-jp/reports/use-cases/IME/image.png "iWnn IME for Android")
- 【組込辞書とクラウド辞書の変換例】
![組込辞書とクラウド辞書の変換例](https://w3c-cg.github.io/mcm-jp/reports/use-cases/IME/image-1.png "組込辞書とクラウド辞書の変換例")
- 【辞書開発プロセス】
![辞書開発プロセス](https://w3c-cg.github.io/mcm-jp/reports/use-cases/IME/image-2.png "辞書開発プロセス")
- 【辞書データ構造】
![辞書データ構造](https://w3c-cg.github.io/mcm-jp/reports/use-cases/IME/image-3.png "辞書データ構造")

### 参照仕様など（任意）


## CGへの課題共有

