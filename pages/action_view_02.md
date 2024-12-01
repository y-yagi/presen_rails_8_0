# Rename `text_area` methods into `textarea`

* [PR](https://github.com/rails/rails/pull/52467)
* view helpersの`text_area`を`textarea`にリネーム
* HTMLでは`textarea`が使われており、同じ名前の方が混乱が少ないだろう、とのことで
* 同様にAction Textの`rich_text_area`も`rich_text_area`にリネーム
* 古い方の名前は互換性のために引き続き使える
