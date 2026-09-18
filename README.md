# Kshop商品台帳

Kshop 本店の商品台帳ページです。GitHub Pages で公開しています。

## ファイル構成

- `index.html` — 台帳ページ本体(このファイルがGitHub Pagesで表示されます)
- `ledger_data.js` — 商品データ(index.htmlに埋め込み済みのバックアップ)
- `ledger_master.csv` — マスターデータ(JAN・数量・原価・売価・商品名)
- `image_asset_map.csv` — 商品画像の対応表(参考用)
- `images/` — 商品画像(812枚、JANコード.jpg)

## データの更新方法

1. `ledger_master.csv` を編集(商品名・価格などを修正)
2. 更新後、`index.html` 内の `const CATS=[...]` を作り直して反映
   (Claude Codeで作業する場合は、これまでと同様にCSVを読み込んでHTMLに埋め込み直す)
3. 変更をコミットしてpush → GitHub Pagesに自動反映されます(数分かかる場合あり)

## 公開URL

GitHub Pages設定後、以下のURLで公開されます:
`https://kshop-collab.github.io/kshop-ledger/`
