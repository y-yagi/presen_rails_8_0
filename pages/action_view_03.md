# Rename `text_area` methods into `textarea`

* [PR](https://github.com/rails/rails/pull/52467)
* view helpersの`text_area`を`textarea`にリネーム
* 同様にAction Textの`rich_text_area`も`rich_text_area`にリネーム
* 理由は`checkbox`と同じ
* 古い方の名前は互換性のために引き続き使える
