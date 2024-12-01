# SQLite on production

* 37signalsの製品である、[https://once.com/campfire](https://once.com/campfire)や[https://once.com/writebook](https://once.com/writebook)はSQLite3で提供しているとのこと
* [Ruby Video](https://www.rubyvideo.dev/)ではSQLite3を使用して、平均応答時間100ミリ秒未満で数百万件のリクエストを処理を出来ているらしい
* 先のページに記載したSQLite driver / adapterの改善をした、Stephen Margheim氏がブログに改善を行った内容や、databaseのバックアップをどうすれば良いかをまとめてくれているので、興味がある方は合わせてどうぞ
  * [Supercharge the One Person Framework with SQLite](https://fractaledmind.github.io/2024/10/16/sqlite-supercharges-rails/)
