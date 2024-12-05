# Allow async queries in transactional fixtures

* [PR](https://github.com/rails/rails/pull/52806)
* 元々はasync queriesはtransactional fixtures内では実行出来なかった(強制的に同期実行になっていた)のを、transactional fixtures内でasync queriesを実行出来るよう対応
