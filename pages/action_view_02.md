# [Rename `text_area` methods into `textarea`](https://github.com/rails/rails/commit/f9c51ec385a7b75e212954cd4b22c2da7c1d32f4)

* view helpersの`text_area`を`textarea`にリネーム
* HTMLでは`textarea`が使われており、同じ名前の方が混乱が少ないだろう、とのことで
* 同様にAction Textの`rich_text_area`も`rich_text_area`にリネーム
* 古い方の名前は互換性のために引き続き使える(が、いつまで使えるかは不明)
