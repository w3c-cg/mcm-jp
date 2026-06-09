# CG Final Report スナップショット

本ディレクトリは [w3c/cg-reports](https://github.com/w3c/cg-reports) リポジトリへ提出する CG Final Report のステージングです。

## ディレクトリ命名規約

W3C の [CG Report Requirements](https://www.w3.org/community/reports/reqs/) と w3c/cg-reports の慣例に従います。

```
CG-FINAL-<reportshortname>-<YYYYMMDD>/
```

- `reportshortname` は このレポートの shortName (`mcm-jp` は CG shortName と同型だが、Report 識別子としては個別に付与する。例: `media-metadata-interop`)
- `YYYYMMDD` は publishDate
- 公開後 URL: `https://www.w3.org/community/reports/mcm-jp/CG-FINAL-<reportshortname>-<YYYYMMDD>/`

## 一覧

| 公開日 | ディレクトリ |
|---|---|
| 2026-06-09 | [CG-FINAL-media-metadata-interop-20260609/](./CG-FINAL-media-metadata-interop-20260609/) |

## 構成

各スナップショットディレクトリには ReSpec で静的化済みの `index.html` と、相対参照される `assets/` 配下の画像のみを置きます。PDF / CSV / XLSX などのデータファイルは元リポジトリ (`https://w3c-cg.github.io/mcm-jp/...`) への絶対 URL を記載。
