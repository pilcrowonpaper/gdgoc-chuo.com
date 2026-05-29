# gdgoc-chuo.com

GDGoC Chuo 公式サイト

## 実行

```bash
pnpm dev

pnpm check

pnpm build
```

## ブログを追加する流れ

1. リポジトリをフォーク
2. クローン
3. `git checkout -b docs/update-blog` でブランチを切り替え
4. `\src\pages\blog` に `NUMBER.astro` 形式でブログを追加
5. `\src\pages\blog\index.astro` 内に追加したブログを記載
6. Pull Requestを送る
