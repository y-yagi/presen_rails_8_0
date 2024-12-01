# action_dispatch.strict_freshness

* `fresh_when`、`stale?`メソッドで、`If-Modified-Since`と`If-None-Match`の両方のヘッダーがある場合に、`If-None-Match` のみをチェックするかを指定
  * `true`(推奨値)の場合`If-None-Match` のみを満たせばOK、`false`(古いバージョンでのも挙動)の場合、両方の値を満たす必要がある
* [RFC 7232 \- Hypertext Transfer Protocol \(HTTP/1\.1\): Conditional Requests](https://datatracker.ietf.org/doc/html/rfc7232#section-6)に、`If-None-Match` のみを満たせば良いと定義されている為
