# [Merge pull request #52353 from Shopify/lazy_routes_retry](https://github.com/rails/rails/commit/9f80efc79119037fc4421d06e94a0d7e076876a4)

* `eager_load`がfalseの場合、最初のリクエストか`url_helpers`が実行されるまで、routeのdrawingを遅らせるよう対応
* drawing元々アプリケーションのload時に行われていたが、routeが大量に定義されている環境だとdrawingに時間が掛ってしまっており、ユニットテストやmigrationの実行などrouteが関係しない処理でそれらのオーバーヘッドを無くせるようにする為
* [amatsuda/routes_lazy_routes](https://github.com/amatsuda/routes_lazy_routes) gemでやっていた事を本体に導入した形
