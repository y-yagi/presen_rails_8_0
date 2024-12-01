# [`ActiveSupport::TimeWithZone#inspect` now uses ISO 8601 style time like `Time#inspect`](https://github.com/rails/rails/commit/0b12b98f222e6e17211f6fb22147370f5d6a0067)

* `ActiveSupport::TimeWithZone#inspect`で使用するTimeのフォーマットをISO 8601 style(`%a, %d %b %Y %H:%M:%S.%9N`)に変更
  * Ruby本体の`Time#inspect`のフォーマット合わせる為
