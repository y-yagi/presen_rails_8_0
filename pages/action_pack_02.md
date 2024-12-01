# [Add `Parameters#expect` to safely filter and require params (#51674)](https://github.com/rails/rails/commit/e1d58cfd05ae1cc0bfc1006b7ce973a7730831df)

* `ActionController::Parameters`にパラメータのfilter/requireをする為の`expect`メソッドを追加
* 元々は`require` + `permit`で行っていたが、`require` + `permit`だと不正なパラメータが送信された場合に500になってしまう、という問題があり、不正なパラメータの場合も400エラーを適切に返せるようにする為に新しいAPIが追加された


