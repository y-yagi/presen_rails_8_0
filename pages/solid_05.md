# Solid Cache

* Redisからの脱却が目的
  * メモリよりディスクの方が安いし、今だとディスクの性能もそんなに悪くないよね、というところからの発想
  * Railsアプリケーションを本番で動かすときの依存を減らしたい
* Rails 8.0で新規アプリケーションを作成した場合、データを保存するテーブルを作成するschemaファイルの追加や、デフォルトでSolid Cableを使用するようAction Cableの設定がされているようになっている
* その他詳細は、[Solid Cacheについてまなぼう](https://y-yagi-presen-solid-cache.vercel.app/)にまとめていますので、ご興味がある方はどうぞ
