# Add support for SQLite3 full-text-search and other virtual tables

* [PR](https://github.com/rails/rails/pull/52354)
* SQLite3でのfull-text-searchのサポート、の為のvirtual tablesのサポート
* [FTS5](https://sqlite.org/fts5.html)という全文検索のための拡張があり、それを使うにはvirtual tablesが必要だった為
* virtual tablesのためのメソッド(例：`create_virtual_table`)が追加されている