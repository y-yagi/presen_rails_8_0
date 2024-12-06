# Solid Queue

* RDBMSをストレージに使用したバックグラウンド処理用ライブラリ
  * Sidekiq、ResqueやGoodJobの競合
  * RailsがサポートしているRDBMSであれば何でもOK
* Solid Cache同様、Redisからの脱却が目的
* Sidekiqとの比較については、[Sidekiq vs Solid Queue](https://speakerdeck.com/willnet/sidekiq-vs-solid-queue)をご参照ください