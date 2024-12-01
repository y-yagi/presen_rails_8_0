# [`ActiveSupport::ErrorReporter#report` now assigns a backtrace to unraised exceptions.](https://github.com/rails/rails/commit/b1d8cf59d9b3c51fde5dd96ceb829d36b8e28c86)

* `ActiveSupport::ErrorReporter#report`メソッドでraiseされなかったexceptionに対してもbacktraceを設定するよう修正
