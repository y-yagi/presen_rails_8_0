# Support use of alternative database interfaces via the `database_cli`

* [PR](https://github.com/rails/rails/pull/52656)
* `dbconsole`で使用する各RDBMSのCLIツールがコード内で固定になっていたのをconfigで使用するCLIを指定出来るよう対応
* これにより、例えば、[dbcli/pgcli](https://github.com/dbcli/pgcli)を`dbconsole`で使えるようになった

```ruby
config.active_record.database_cli = { postgresql: "pgcli" }
```