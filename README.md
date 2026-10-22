# arigatomyteam.github.io

Astro で作った個人サイト（ポートフォリオ＋ブログ）です。`main` ブランチに push すると、GitHub Actions が自動でビルドして GitHub Pages に公開します。

公開URL: https://arigatomyteam.github.io

## よく触る場所

| やりたいこと | 編集するファイル |
|---|---|
| ブログ記事を追加 | `src/content/blog/` に Markdown（`.md`）を追加 |
| 作品を追加 | `src/content/projects/` に Markdown を追加 |
| サイト名・名前・GitHub URL | `src/consts.ts` |
| ホームの紹介文 | `src/pages/index.astro` |
| 自己紹介ページ | `src/pages/about.astro` |

### ブログ記事の書き方

```markdown
---
title: '記事タイトル'
description: '一覧や検索結果に出る短い説明'
pubDate: '2026-10-22'
---

ここから本文。Markdown で書けます。
```

### 作品の書き方

```markdown
---
title: '作品名'
description: '作品の説明'
pubDate: '2026-10-22'
tags: ['Astro', 'AI']
url: 'https://...'      # 任意：公開URL
repo: 'https://...'     # 任意：ソースコード
featured: true          # 任意：ホームに表示する
---
```

## 手元で動かす

Node.js 22.23.4 以上が必要です。

```sh
npm install
npm run dev     # http://localhost:4321 で確認
npm run build   # dist/ に出力
```
