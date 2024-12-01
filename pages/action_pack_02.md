# Add `Parameters#expect` to safely filter and require params

* [PR](https://github.com/rails/rails/pull/51674)
* `ActionController::Parameters`にパラメータのfilter/requireをする為の`expect`メソッドを追加
* 元々は`require` + `permit`で行っていたが、`require` + `permit`だと不正なパラメータが送信された場合に500になってしまう、という問題があり、不正なパラメータの場合も400エラーを適切に返せるようにする為に新しいAPIが追加された


