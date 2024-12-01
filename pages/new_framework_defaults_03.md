# active_support.to_time_preserves_timezone

* Ruby 2.4より前のバージョン向けの、`to_time`メソッドが返すTimeオブジェクトをタイムゾーンを保持しないようにした対応が復活
  * 正しくdeprecateメッセージが表示されないケースがあり、ユーザがこの挙動の変更に気付かずbreaking changeになってしまう可能性があった為
* configで`to_time`メソッドの挙動が指定出来るようになっている
  * `:zone`(推奨値): レシーバーで設定されているタイムゾーンを使用
  * `:offset`: UTCオフセットを使用
  * `false`: ローカルシステムのUTCオフセットを使用
