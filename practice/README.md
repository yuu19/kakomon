---
layout: default
title: 演習問題トップ
---

# 問題演習ディレクトリ

このディレクトリでは、各大学・専攻ごとの過去問や参考資料をもとにした演習問題セットを Markdown 形式で管理します。GitHub Pages からは自動で HTML に変換されるため、ブラウザ上で閲覧できます。

## ディレクトリ構成

- `templates/` — 新しい演習セットを作成するときにコピーして使える雛形。
- `<university>/<subject>/<year>.md` — 大学・専攻・年度ごとの演習問題。ファイル内の Front Matter でメタ情報を管理します。

## 追加方法

1. `templates/problem-set.md` をコピーして `<university>/<subject>/` 配下に配置します。
2. Front Matter の `title` `source_url` `tags` などを更新します。
3. 問題文や解答スケッチを Markdown で追記します。

### 数式記法 (KaTeX)

- インライン: `$\alpha^2 + \beta^2$`
- ディスプレイ: `$$\int_0^1 f(x)\,dx$$`
- エスケープが必要な場合は `\(`, `\)` も使用可能です。
- LaTeX で扱えない記号は KaTeX の[サポート表](https://katex.org/docs/supported.html)を参照してください。

## GitHub Pages 上でのナビゲーション

サイトのトップページ (`index.md`) と各演習ページに自動でリンクが追加され、一覧からたどれるようになっています。必要に応じて目次やタグを拡張してください。
