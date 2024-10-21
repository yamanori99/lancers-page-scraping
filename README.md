作成者は, ランサーズにログインして特定の作業一覧ページをスクレイピングし、ページのテーブルから作業者 (ランサー) の承認状況やIDを取得して、CSVファイルとして保存する処理に使用した。書き換えれば, 他の用途にも使用できるだろう。

## ログインしてページをスクレイピングし, クリーニングして保存する

このコードは、ページにログインしてスクレイピングを行い、取得したデータを `/raw` にHTML形式で保存する。また、データのクリーニングを行い、結果をCSV形式で `/processed` に保存する。

以下のコマンドでquartoテンプレートが使用できる。qmdファイルのpythonチャンクからコードを抜き取るのもいいだろう。

``` terminal
quarto use template yamanori99/lancers-page-scraping
```