# `ActiveSupport::TimeWithZone#inspect` now uses ISO 8601 style time like `Time#inspect`

* [PR](https://github.com/rails/rails/pull/52371)
* `ActiveSupport::TimeWithZone#inspect`で使用するTimeのフォーマットをISO 8601 style(`%F %H:%M:%S.%9N`)に変更
  * Ruby本体の`Time#inspect`のフォーマット合わせる為
