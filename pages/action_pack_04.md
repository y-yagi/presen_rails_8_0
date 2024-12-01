# Add `Parameters#expect` to safely filter and require params

* 他にも、`expect`では`require` + `permit`より厳密にパラメータをチェックするようになっており、引数がArrayの場合、`[[]]`(e.g. `[[:name]]`)を使用しなければならない、等の違いがあり
* `require` + `permit`は引き続き使用出来るようになっているが、rails guideのサンプルコードやgeneratorが生成するコードは`expect`を使用するよう修正されており、基本的には`expect`を使用するのが推奨されるようになっている
