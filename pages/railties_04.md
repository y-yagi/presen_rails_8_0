# [Add not-null modifier to migrations (#52327)](https://github.com/rails/rails/commit/2f92b1c94e2a080679ab0ad45abd0bdec24a5349)

* カラムのnot-null制約をgeneratorで指定出来るよう対応
* not-nullにしたい場合、型の末尾に`!`をつければOK

```bash
bin/rails generate migration CreateUsers email_address:string!:uniq password_digest:string!
```
