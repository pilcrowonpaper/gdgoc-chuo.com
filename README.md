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
4. `\src\pages\blog` に `NUMBER.astro` 形式でブログを追加 (詳細は[ブログファイルの書き方](#ブログファイルの書き方)に)
5. `\src\pages\blog\index.astro` 内に追加したブログを記載
6. Pull Requestを送る

### ブログファイルの書き方

- `\src\pages\blog` に `NUMBER.astro` 形式でブログを追加  
    - 例 (現在1-9の `.astro` ファイルがあるとき): `10.astro` を追加

- このテンプレートをコピペして編集してください  

    ```astro
    ---
    import "@src/blog.css";
    import * as assets from "astro:assets";
    // ここにこのブログで使いたい画像を記載
    // 構文: import image1 from "@src/images/blog-4-1.png";
    import CompactLayout from "@src/layouts/compact.astro"
    ---

    <CompactLayout
        title="ここにタイトル"
    >

    {/*ここにHTMLを記載 (書き方はほかのastroファイルを確認)*/}

    </CompactLayout>
    ```
