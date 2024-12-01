# [Rename `check_box*` methods into `checkbox*`.](https://github.com/rails/rails/commit/038a314ded26d399fd4b0ba25c6024dc72a5f73d)

* view helpersの`check_box`、及び、関連メソッド(`collection_check_boxes`、`check_box_tag`等)を`checkbox`(`checkbox*`)にリネーム
* 理由は`textare`と同じ
  * HTMLのinputタグのattributeなどは`checkbox`になっている
