# SQLite on production?

* 37signalsの製品である、[https://once.com/campfire](https://once.com/campfire)や[https://once.com/writebook](https://once.com/writebook)はSQLiteで提供しているとのこと
  * [Mike Dalessio](https://github.com/flavorjones)が37signalsに入ったので今後更に改善していくかも
* [Ruby Video](https://www.rubyvideo.dev/)ではSQLiteを使用して、平均応答時間100ミリ秒未満で数百万件のリクエストを処理を出来ているらしい
* 先のページに記載したSQLite driver / adapterの改善をした、Stephen Margheim氏が[ブログ](https://fractaledmind.github.io/2024/10/16/sqlite-supercharges-rails/)に改善を行った内容や、databaseのバックアップをどうすれば良いかをまとめてくれているので、興味がある方は合わせてどうぞ