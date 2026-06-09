<h1 id="tv-program-recommendations-from-e-books"><span lang="ja">電子書籍からの放送番組レコメンド</span> <span lang="en">TV Program Recommendations from E-Books</span></h1>

<div lang="ja">

電子書籍内のメタデータを用いて、関連する放送番組をユーザに推薦する。メタデータの出版業界外での活用にあたる。

</div>

<div lang="en">

Recommends related broadcast programs to the user using metadata within e-books. This is a use of publishing metadata across industries.

</div>

## 関連する産業ドメイン
- 出版
- 放送
- OTTサービス


## シナリオ

1. ユーザが電子書籍リーダーで、電子書籍を閲覧する。
2. ユーザが書籍を読了する。
3. 電子書籍リーダーが、番組レコメンドスクリプトを実行し、書籍のメタデータを取得する。
4. 電子書籍リーダーが、放送番組検索サーバに対して、書籍メタデータの一部を検索条件として、書籍に関連する放送番組を要求する。
5. 放送番組検索サーバは、検索条件に合致する放送番組情報を、電子書籍リーダーに返答する。
6. 電子書籍リーダーは、放送番組情報をもとに、ユーザに番組のレコメンドを提示する。

<figure>
  <img src="/mcm-jp/reports/use-cases/cross-industry/interop-tokyo2025/images/ebook-rec-program.png" alt="interop6" />
  <figcaption>システム構成・動作フロー概要</figcaption>
</figure>

### 実装例

- 電子書籍リーダー
  - [Thorium Reader](https://www.edrlab.org/software/thorium-reader/)
- 電子書籍
  - EPUB仕様
- クライアント動作環境
  - Microsoft Surface Pro 9 (Windows11)
- 電子書籍メタデータ
  - EPUB OPFファイル


```xml
<?xml version="1.0" encoding="UTF-8"?>
<package
  xmlns="http://www.idpf.org/2007/opf"
  version="3.0"
  xml:lang="ja"
  unique-identifier="unique-id"
  prefix="ebpaj: http://www.ebpaj.jp/"
>

<metadata xmlns:dc="http://purl.org/dc/elements/1.1/">

	<!-- 作品名 -->
	<dc:title id="title">倫敦塔</dc:title>
	<meta refines="#title" property="file-as">ロンドントウ</meta>

	<!-- 著者名 -->
	<dc:creator id="creator01">夏目漱石</dc:creator>
	<meta refines="#creator01" property="role" scheme="marc:relators">aut</meta>
	<meta refines="#creator01" property="file-as">ナツメソウセキ</meta>
	<meta refines="#creator01" property="display-seq">1</meta>

	<!-- 出版社名 -->
	<dc:publisher id="publisher">青空文庫</dc:publisher>
	<meta refines="#publisher" property="file-as">アオゾラブンコ</meta>

	<!-- 言語 -->
	<dc:language>ja</dc:language>

	<!-- ファイルid -->
	<dc:identifier id="unique-id">urn:uuid:765a97cb-2094-4b94-baea-d01a2cfc85da</dc:identifier>

	<!-- 更新日 -->
	<meta property="dcterms:modified">2024-05-01T00:00:00Z</meta>

	<!-- etc. -->
	<meta property="ebpaj:guide-version">1.1.3</meta>

</metadata>

```


### 参照仕様など
- [EPUB W3C勧告](https://www.w3.org/TR/epub-33/)
- [電書連 EPUB 3 制作ガイド](https://dpfj.or.jp/counsel/guide)