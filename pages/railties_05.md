# Defer route drawing to the first request, or when url_helpers

* [PR](https://github.com/rails/rails/pull/52353)
* `eager_load`がfalseの場合、最初のリクエストか`url_helpers`が実行されるまで、routeのdrawingを遅らせるよう対応
* 元々はアプリケーションのload時に行われていたが、routeが大量に定義されている環境だと処理に時間が掛ってしまっており、ユニットテストやmigrationの実行などrouteが関係しない処理でそれらのオーバーヘッドを無くせるようにする為
* [amatsuda/routes_lazy_routes](https://github.com/amatsuda/routes_lazy_routes) gemでやっていた事を本体に導入した形
