# Rename `check_box*` methods into `checkbox*`

* [PR](https://github.com/rails/rails/pull/52432)
* view helpersの`check_box`、及び、関連メソッド(`collection_check_boxes`、`check_box_tag`等)を`checkbox`(`checkbox*`)にリネーム
* HTMLでは`checkbox`が使われており、同じ名前の方が混乱が少ないだろう、とのことで
  * HTMLのinputタグのattributeなどは`checkbox`になっている
