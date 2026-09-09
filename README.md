# surf90.github.io

組織 [`surf90`](https://github.com/surf90) のルートサイト（GitHub Pages 組織サイト）。
公開URL: **https://surf90.github.io/**

茅ヶ崎の海の情報サイト「ちがログ」「ちがビオ」へのハブ（一覧）ページと、
`surf90.github.io` サブドメイン全体で共有される `robots.txt` / `sitemap.xml` /
Google Search Console 検証ファイルを配信する。

## 掲載サイト

| サイト | 内容 | URL |
|---|---|---|
| ちがログ | 茅ヶ崎の海況データ（天気・波・水温・潮汐・注意報） | https://surf90.github.io/chiga-log/ |
| ちがビオ | 茅ヶ崎の生き物ガイド（砂浜・磯・海・河口・町中） | https://surf90.github.io/chiga-bio/ |

※ ハブは一般利用者向けの2サイトに絞る。印刷ユーティリティの
[tide-PDF](https://surf90.github.io/tide-PDF/) と訓練用の
[rescue-sim](https://surf90.github.io/rescue-sim/) は用途が異なるため掲載しない
（[組織プロフィール](https://github.com/surf90)には掲載）。

## 構成

- `index.html` — ハブページ（依存なしの Vanilla HTML/CSS）
- `robots.txt` — サブドメイン全体のクロール設定（ルートからのみ配信可能）。
  各サイトの `sitemap.xml` もここで宣言する。
- `sitemap.xml` — ルートページのみ。各サイトのサイトマップはそれぞれのリポジトリが持つ
  （chiga-log は `jekyll-sitemap`、chiga-bio は `scripts/build.py` が生成）。
- `googled180bd734463e748.html` — Search Console 検証ファイル

## メンテナンス

- サイトを増減したら `index.html` のカードと `robots.txt` の `Sitemap:` 宣言を更新する。
- ページを追加する場合は `sitemap.xml` にも手動で追記する。

## 注記

本組織および公開しているツールは、サーフ90茅ヶ崎ライフセービングクラブの公式な運営に
よるものではありません。メンバー個人が開発・管理しているプロジェクトです。

## ライセンス

MIT License © 2026 ISHIKAWA, Natsuki
