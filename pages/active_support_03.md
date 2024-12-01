# `ActiveSupport::ErrorReporter#report` now assigns a backtrace to unraised exceptions

* [PR](https://github.com/rails/rails/pull/52684)
* `ActiveSupport::ErrorReporter#report`メソッドでraiseされなかったexceptionに対してもbacktraceを設定するよう修正
