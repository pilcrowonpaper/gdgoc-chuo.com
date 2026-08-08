# gdgoc-chuo.com

GDGoC Chuo 公式サイト

## ブログを追加する流れ

1. リポジトリをフォーク
2. クローン
3. `git checkout -b docs/update-blog` でブランチを切り替え
4. `public/blog` 内に `NUMBER` ディレクトリを作成し、その中に `index.html` を追加 (詳細は[ブログファイルの書き方](#ブログファイルの書き方)に)
5. `public/blog/index.html` 内に追加したブログを記載
6. Pull Requestを送る

### ブログファイルの書き方

- `public/blog` 内に `NUMBER` フォルダを作成し `template` をコピペして `index.html` にリネーム
    - 例 (現在1-7のフォルダがあるとき): `public/blog/8/index.html` を追加


    ```html
    <head>
    	<title>ここにタイトル</title>

    	<meta charset="utf-8" />
    	<meta name="viewport" content="width=device-width" />

    	<link rel="icon" type="image/jpeg" href="https://gdgoc-chuo.com/gdg.jpeg" />

    	<meta property="og:title" content="ここにタイトル" />
    	<meta property="og:type" content="website" />
    	<meta property="og:locale" content="ja_JP" />
    	<meta property="og:site_name" content="GDGoC Chuo University" />
    	<meta property="og:url" content="https://gdgoc-chuo.com/blog/NUMBER" />
    	<meta property="og:image" content="https://gdgoc-chuo.com/gdg.jpeg" />

    	<meta name="twitter:card" content="summary_large_image" />
    	<meta name="twitter:site" content="@gdgs_chuo" />

    	<link rel="stylesheet" href="/text-page.css" />
    </head>

    <body>
    	<header>
    		<div id="header-inner">
    			<a id="header-home-link" href="/">GDGoC Chuo University</a>
    		</div>
    	</header>
    	<main>
    		<div id="main-inner" class="text-content">
    			<h1>ここにタイトル</h1>
    			<p>ここに本文を記述</p>
    		</div>
    	</main>
    </body>
    ```
