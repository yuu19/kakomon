---
layout: default
title: Kakomon アーカイブ
---

# Kakomon

大学院入試の過去問題アーカイブに演習用コンテンツを追加しました。GitHub Pages では、下記リンクからブラウザで閲覧できます。

- [演習問題トップ `practice/`](practice/)

## 最新の演習セット

{% assign sorted = site.practice | sort: 'last_reviewed' | reverse %}
{% for page in sorted limit:5 %}
- [{{ page.title }}]({{ page.url | relative_url }}) — last reviewed {{ page.last_reviewed }} {% if page.tags %}({{ page.tags | join: ', ' }}){% endif %}
{% endfor %}

## フォルダ構成

- `practice/` — 演習問題とテンプレート
- `tohoku/`, `kyodai/`, `titech/`, `todai/`, `hitotsubashi/`, `soken/` — 各大学の PDF アーカイブ

## 更新手順メモ

1. 演習セットを追加または更新
2. `index.md` の最新リストを確認 (Liquid の自動生成で更新されます)
3. GitHub に push すると GitHub Pages が自動で再ビルドされます
